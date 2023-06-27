<template>
    <article>
        <div class="container">
            <h3>PHASELLUS EGET METUS</h3>
            <h1>All The Latest News</h1>
            <div class="separator"></div>
            <div class="layout-cards flex">
                <SingleCard  v-for="card in TopCards" :card="card" />
            </div>           
            <AppCover />
            <div class="layout-cards flex">
                <SingleCard  v-for="card in BottomCards" :card="card" />
            </div> 
        </div>
    </article>
   
</template>

<script>
import SingleCard from './SingleCard.vue' 
import AppCover from './AppCover.vue' 


export default {
    name: 'CardList',
    components:{
        SingleCard,
        AppCover
    },
    data(){
        return {
            TopCards : [
                {
                    bigImage : 'post_feat_img_25-700x441',
                    title : 'Morbi vitae dui euismod vulputate sollicitudin',
                    date : 'October 11th, 2015|  2 Comments',
                    text : 'Donec finibus sit amet orci eget ultricies. Praesent posuere ante ut erat fringilla, vestibulum placerat metus mattis. Aenean dictum vitae nisl'
                },
                {
                    bigImage : 'post_feat_img_24-700x441',
                    title : 'Vivamus pellenteque, felis quis varius',
                    date : 'October 11th, 2015|  Comments Off',
                    text : 'Donec finibus sit amet orci eget ultricies. Praesent posuere ante ut erat fringilla, vestibulum placerat metus mattis. Aenean dictum vitae nisl'
                },
                {
                    bigImage : 'post_feat_img_23-700x441',
                    title : 'Donec ornare pretium eget scelisque justo',
                    date : 'October 11th, 2015|  Comments Off',
                    text : 'Donec finibus sit amet orci eget ultricies. Praesent posuere ante ut erat fringilla, vestibulum placerat metus mattis. Aenean dictum vitae nisl'
                }
            ],
            BottomCards : [
                {
                    bigImage : 'post_feat_img_22-700x441',
                    title : 'Fusce sollicitudin nunc sed placerat varius',
                    date : 'October 11th, 2015|  Comments Off',
                    text : 'Donec finibus sit amet orci eget ultricies. Praesent posuere ante ut erat fringilla, vestibulum placerat metus mattis. Aenean dictum vitae nisl'
                },
                {
                    bigImage : 'post_feat_img_21-700x441',
                    title : 'Donec facilis sodales leo sit amet laoreet',
                    date : 'October 11th, 2015|  Comments Off',
                    text : 'Donec finibus sit amet orci eget ultricies. Praesent posuere ante ut erat fringilla, vestibulum placerat metus mattis. Aenean dictum vitae nisl'
                },
                {
                    bigImage : 'post_feat_img_20-700x441',
                    title : 'Proin eu purus sed aru aliquet curabir vens',
                    date : 'October 11th, 2015|  Comments Off',
                    text : 'Donec finibus sit amet orci eget ultricies. Praesent posuere ante ut erat fringilla, vestibulum placerat metus mattis. Aenean dictum vitae nisl'
                }
            ]
        
        }
      },
}
</script>



<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

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
        font-size: 36px;
        font-weight: bolder;
        margin: 1.5rem 0;
    }
    .layout-cards{
        justify-content: space-between;
        text-align: left;
        margin-top: 3.5rem;

    }

}

  
</style>

  