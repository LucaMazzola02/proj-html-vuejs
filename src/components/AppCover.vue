<template>
    <article class="cover flex">
        <div class="cover-text">
            <h3>FEATURED ARTICLE</h3>
            <h1>Cras Malesuada Et Orci Eget Pharetra</h1>
            <p>In quis lectus sed leo elementum faucibus in dapibus dictum. Nullamolestie tortor nec lectus venenatis, sed blandit dui, dolor at bibendum sadips ets ipsums dolores ficilis uns leo lectus.</p>
            <button class="button">READ MORE ></button>
        </div>    
    </article>    
</template>

<script>



export default {
    name: 'AppCover',
    
}
</script>



<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.cover{
    height: 65vh;
    background-image: url(../assets/img/featured_article_1_bg.jpg);
    background-size: contain;
    background-repeat: no-repeat;
    color: $whiteColor;
    align-items: center;
    text-align: left;
    padding: 5rem;

    & .cover-text h3{
        margin-bottom: 1.3rem;
        font-size: 16px;
        font-weight: 600;
        letter-spacing: 4px;
    }

    & .cover-text h1{
        font-size: 45px;
    }

    & .cover-text p{
        font-size: medium;
        margin: 2.5rem 0;
    }
    .button{
        background-color: $blackColor;
        padding: 1.1rem 1.7rem;
        color: $whiteColor;
        font-size: 1.1rem;
        font-weight: bold;
        transition: $transition;

        &:hover{
            background-color: $coralColor;
        }
    }
}
  
</style>

  