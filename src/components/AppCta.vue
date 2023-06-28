<template>
    <article>
        <div class="container">
            <h4>Subscribe To Our Newsletter</h4>
            <div class="cta flex">
                <input type="email" placeholder="insert your email*">
                <button class="button">SEND</button>
            </div>
        </div>
    </article>
    
</template>

<script>



export default {
    name: 'AppCta',
    components:{
        
    }
}
</script>



<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

article{
    background-color: $lightgreyColor;
    & .container{
        padding: 7.5rem 20rem;
        text-align: center;
        & h4{
            margin-bottom: 1.8rem;
            color: $blackColor;
            font-size: 2rem;
        }
    }
    & .cta{
        align-items: center;
        justify-content: space-between;
    }
    & input{
        width: 550px;
        padding: 1rem .6rem;
        font-size: 1.1rem;
    }
    & .button{
        background-color: $blackColor;
        padding: 1rem 6rem;
        transition: $transition;
        color: $whiteColor;
        font-size: 1.3rem;
        font-weight: bolder;
        border-radius: 4px;
        &:hover{
            background-color: $coralColor;
        }
    }
}
  
</style>

  