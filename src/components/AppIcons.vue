<template>
    <div class="icon prebuilts">
        <i class="fa-solid fa-folder"></i>
        <p>Prebuilts</p>
    </div>
    <div class="icon buy-now">
        <i class="fa-solid fa-cart-shopping"></i>
        <p>Buy now</p>
    </div>

    
</template>
  
<script>
export default {
      name: 'AppIcons',
       
  }
</script>
  
<style lang="scss" scoped>
@use '../styles/partials/_variables' as *;
    

    .icon{
        position: absolute;
        padding: 14px 6px 0 6px;
        width: 80px;
        height: 80px;
        cursor: pointer;
        background-color: #fff;
        border-radius: 6px;
        box-shadow: 0 0 25px 5px rgba(0,0,0,.2);
        text-align: center;
        color: rgba(63,114,155,255);
        font-weight: bolder;
        & i{
            font-size: 1.5rem;
            margin-bottom: 8px;
            
        }
    }
    .prebuilts{
        top: 150px;
        right: 15px;
    }
    .buy-now{
        top: 240px;
        right: 15px;
    }
  
    
</style>
  