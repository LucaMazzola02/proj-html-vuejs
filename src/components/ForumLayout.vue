<template>
    <article>
        <div class="container">
            <h3>PHASELLUS EGET METUS</h3>
            <h1>Forum Sections</h1>
            <div class="separator"></div>
            <div class="forum-layout flex">
                <ForumCard v-for="forumCard in cards" :forumCard="forumCard"/>    
            </div>                   
        </div>
    </article>
</template>

<script>
import ForumCard from './ForumCard.vue' 

export default {
    name: 'ForumLayout',
    components:{
        ForumCard,       
    },
    data(){
        return {
            cards : [
                {
                    image : 'fa-solid fa-file-lines',
                    title : 'News & Community',                 
                },               
                {
                    image : 'fa-brands fa-apple',
                    title : 'Apple Forum',                 
                }, 
                {
                    image : 'fa-brands fa-windows',
                    title : 'Microsoft Forum',                 
                }, 
                {
                    image : 'fa-brands fa-android',
                    title : 'Android Forum',                 
                }, 
                {
                    image : 'fa-solid fa-mug-hot',
                    title : 'General Discussion',                 
                }, 
                {
                    image : 'fa-solid fa-cubes',
                    title : 'App & Software',                 
                },               
                {
                    image : 'fa-solid fa-laptop',
                    title : 'Gadgets & Stuff',                 
                }, 
                {
                    image : 'fa-solid fa-wrench',
                    title : 'Tutorials & Guides',                 
                }, 
            ],
                   
        }
      },
}
</script>



<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

article{
    background-color: $lightgreyColor;
}

article .container{
    padding: 7rem 0 ;
    text-align: center;

    & h3{
        color: rgb(86, 86, 86);
        font-size: 16px;
        font-weight: 600;
        letter-spacing: 4px;
    }

    & h1{
        font-size: 4rem;
        font-weight: bolder;
        margin: 1.5rem 0;
    }

    .forum-layout{
        justify-content: space-between;
        flex-wrap: wrap;
        margin-top: 4rem;

    }
} 
</style>
