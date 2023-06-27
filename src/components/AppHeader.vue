<template>
    <header>
        <div class="container flex">           
                <div class="logo">
                  <img src="../assets/img/logo.png" alt="Logo-image">
                </div>
                <nav class="nav-bar flex">
                    <ul class="flex">
                        <a href=""><li>Home</li></a> 
                        <a href=""><li>Apple</li></a> 
                        <a href=""><li>Microsoft</li></a> 
                        <a href=""><li>Android</li></a> 
                        <a href=""><li>Forums</li></a> 
                        <a href=""><li>Contact us</li></a> 
                    </ul>
                    <button class="button">Join us</button>
                    <i class="fa-solid fa-magnifying-glass"></i>
                </nav>             
        </div> 
    </header>
    
</template>
  
<script>
export default {
      name: 'AppHeader',
      components:{
      }
  }
</script>
  
  
  
<style lang="scss" scoped>
@use '../styles/partials/_variables' as *;

header{
    background-color: $skyblueColor;

    & .container{
        height: 100px;
        justify-content: space-between;
        align-items: center;
    }
    .nav-bar{
        align-items: center;
    }
    & nav ul a li{
        margin-left: 2rem;
        transition:$transition;
        color: $lightgreyColor;
    }
    & nav ul a li:hover{
        color: $whiteColor;
    }
    button{
        margin: 0 2rem ;
        padding: .6rem 1.2rem;
        background-color: $blackColor;
        color: $whiteColor;
        border-radius: 3px;
        font-size: 1.05rem;
        font-weight: bold;
        transition: $transition;


        &:hover{
            background-color: $coralColor;
        }
    }
    & i{color: $lightgreyColor;}
}
    
</style>
  