<template>
    <article>
        <div class="container">
            <h1>Hey! Join To Our Community</h1>
            <p>Nulla molestie tortor nec lectus venenatis, sed blandit dui finibus. Curabitur feugiat vulputate purus ipsums dolores ficilis uns etra.</p>
            <button class="button">SIGN UP > </button>

        </div>
    </article>
    
</template>

<script>
 


export default {
    name: 'AppCommunity',

}
</script>



<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

article{
    height: 75vh;
    background-image: url(../assets/img/join_now_cta_bg.jpg);
    & .container{
        flex-direction: column;
        justify-content: center;
        text-align: center;
        color: $whiteColor;
        padding: 15rem 25rem;
        & h1{
            font-size: 4rem;
            font-weight: bolder;
        }
        & p{
            margin: 1.7rem 0;
            line-height: 2rem;
        }
        .button{
            background-color: $skyblueColor;
            padding: 1.4rem 3rem;
            border-radius: 4px;
            font-size: 1.3rem;
            font-weight: bolder;
            color: $whiteColor;
            transition: $transition;
            &:hover{
                background-color: $coralColor;
            }
        }
    }
}
  
</style>

  