<template>
    <FusionLayout />
    <CardList />  
    <div class="spacer flex">READ OUR BLOG
        <i class="fa-solid fa-arrow-right"></i>
    </div>
    <ForumLayout />
</template>

<script>
import FusionLayout from './FusionLayout.vue' 
import CardList from './CardList.vue' 
import ForumLayout from './ForumLayout.vue' 


export default {
    name: 'AppMain',
    components:{
        FusionLayout,
        CardList,
        ForumLayout
    }
}
</script>



<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
  
</style>

  