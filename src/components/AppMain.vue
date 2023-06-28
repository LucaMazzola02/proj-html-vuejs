<template>
    <FusionLayout />
    <CardList />  
    <div class="spacer flex">READ OUR BLOG
        <i class="fa-solid fa-arrow-right"></i>
    </div>
    <ForumLayout />
    <div class="spacer flex">GO TO OUR FORUM
        <i class="fa-solid fa-arrow-right"></i>
    </div>
    <AppCommunity />
</template>

<script>
import FusionLayout from './FusionLayout.vue' 
import CardList from './CardList.vue' 
import ForumLayout from './ForumLayout.vue' 
import AppCommunity from './AppCommunity.vue' 


export default {
    name: 'AppMain',
    components:{
        FusionLayout,
        CardList,
        ForumLayout,
        AppCommunity,
    }
}
</script>



<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
  
</style>

  