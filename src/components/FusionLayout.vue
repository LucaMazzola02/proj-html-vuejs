<template>
    <article>
        <div class="container">
            <h4>AVADA FORUMS IS THE PLACE TO BE</h4>
            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Iusto doloribus eaque nihil rerum voluptas odit molestiae mollitia, minima facilis reiciendis vero soluta voluptates facere ab, delectus aliquam non, porro optio.</p>
        </div>        
    </article>
    
</template>

<script>


export default {
    name: 'FusionLayout',
    components:{
    }
}
</script>



<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

article{
    background-color: $lightgreyColor;
    text-align: center;

    & .container{
       padding:  5rem 22rem ; 
    }
    

    & h4{
        color: rgb(86, 86, 86);
        margin-bottom: 1.3rem;
        font-size: 16px;
        font-weight: 600;
        letter-spacing: 4px;
    }

    & p{
        color: $greyColor;
        line-height: 28px;
    }
}
  
</style>

  