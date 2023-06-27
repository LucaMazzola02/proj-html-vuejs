<template>
    <header>
        <div class="container flex">           
                <div class="logo">
                  <img src="../assets/img/logo.png" alt="Logo-image">
                </div>
                <nav class="nav-bar flex">
                    <ul class="flex">
                        <li>
                            Home
                        </li>
                        <li>
                            Apple
                        </li>
                        <li>
                            Microsoft
                        </li>
                        <li>
                            Android
                        </li>
                        <li>
                            Forums
                        </li>
                        <li>
                            Contact us
                        </li>
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
    & nav ul li{
        margin-left: 2rem;
        transition: all .5s cubic-bezier(.215, .61, .355, 1);
    }
    & nav ul li:hover{
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
        transition: all .5s cubic-bezier(.215, .61, .355, 1);


        &:hover{
            background-color: $coralColor;
        }
    }
}
    
</style>
  