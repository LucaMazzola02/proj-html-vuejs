<template>
    <article class="single-card">
        <div class="card-body">
            <div class="card-image">
              <img class="big-image" :src="getImagePath(card.bigImage)" alt="big-image">
            </div>
            <div class="description">            
                <h2 class="card-title">
                  {{ card.title }}
                </h2>
                <div class="date" >
                  {{ card.date }}                   
                </div>
                <p class="text">
                    {{ card.text }}                  
                </p>
            </div>
        </div>
      </article>
   
</template>

<script>

export default {
    name: 'SingleCard',
    props :{
        card : Array
    },
    methods :{
      getImagePath(img){
        return new URL(`../assets/img/${img}.jpg`, import.meta.url).href;
      },
    },
    
}
</script>



<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.single-card{
    width: calc((100% / 3) - 4rem);
}

.card-image .big-image{
    width: 100%;
    height: 100%;
    transition: $transition;
    &:hover{
        transform: scale(.85);
    }
    
}  
.card-title{
    margin-top: 0.8rem;
    font-size: 1.2rem;
    font-weight: bold;
}

.date{
    margin: .6rem 0 1.5rem 0;
}

.text{
    line-height: 25px;
    margin-bottom: 2rem;
}

  
</style>

  