<template>
  <div class="jumbotron flex">
    <div class="container">
      <h1>Tech Forum! </h1>
      <p>Discuss all the latest technology news and trends </p>
      <button class="button">GET AVADA NOW!></button>
    </div>
  </div>
    
</template>
  
<script>

  
export default {
      name: 'AppJumbotron',
      components:{
      }
  }
</script>
  

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.jumbotron{
  height: 100vh;
  background-image: url(../assets/img/home_slider_bg.jpg);
  background-size: cover;
  color: $whiteColor;
  align-items: center;

  & h1{
    font-size: 10rem;
  }
  & p{
    font-size: 1.3rem;
    margin: 1rem 0 2rem;
  }
  .button{
    background-color: $skyblueColor;
    color: $whiteColor;
    font-weight: bold;
    font-size: 1.15rem;
    padding: 1rem 1.8rem;
    transition: $transition;

    &:hover{
      background-color: $coralColor;
    }
  }

}
    
</style>
  