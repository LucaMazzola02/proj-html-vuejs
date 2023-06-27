<template>
    <article>
        <div class="container">
            <h3>PHASELLUS EGET METUS</h3>
            <h1>All The Latest News</h1>
            <div class="separator"></div>
            <SingleCard v-for="card in cards" />
            <AppCover />
        </div>
    </article>
   
</template>

<script>
import SingleCard from './SingleCard.vue' 
import AppCover from './AppCover.vue' 


export default {
    name: 'CardList',
    props :{
        cards : Array

    },
    components:{
        SingleCard,
        AppCover
    }
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
}
  
</style>

  