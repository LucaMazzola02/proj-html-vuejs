<template>
  <div class="jumbotron flex">
    <div class="container">
      <h1>Tech Forum </h1>
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
  height: calc(100vh - 100px);
  background-image: url(../assets/img/home_slider_bg.jpg);
  background-size: cover;
  color: $whiteColor;
  align-items: center;

  & h1{
    font-size: 10rem;
  }
  & p{
    font-size: 1.2rem;
    margin: 1rem 0 2rem;
  }
  .button{
    background-color: $skyblueColor;
    color: $whiteColor;
    padding: .8rem 1.7rem;
    transition: $transition;

    &:hover{
      background-color: $coralColor;
    }
  }

}
    
</style>
  