<template>
    <article class="single-forum-card">
        <div class="card-body flex">
            <div class="card-image">                  
                <i :class="`${forumCard.image}`"></i>    
            </div>                     
            <h2 class="card-title">
                {{ forumCard.title }}                
            </h2>                
        </div>
      </article>
</template>

<script>



export default {
    name: 'ForumCard',
    props :{
        forumCard : Array
    },
}
</script>



<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.single-forum-card{
    background-color: $whiteColor;
    width: calc((100% / 4) - 2rem);
    height: 250px;
    padding: 3rem 2rem;
    border-top: 5px solid $skyblueColor;
    margin: 1.7rem 0;

    .card-body{
        flex-direction: column; 
    }
    

    .card-image{
        background-color: $coralColor;
        width: 80px;
        height: 80px;
        padding: 10px;
        border-radius: 50%;
        margin: auto;
        margin-bottom: 1.5rem;
        position: relative;
        transition: $transition;

        &:hover{
            box-shadow: 0 0 20px 20px $coralColor;
        }

    }
    .card-image i{
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        font-size: 3rem;
        color: $whiteColor;

    }

    .card-title{
        font-weight: bolder;       
    }
}


  
</style>

  