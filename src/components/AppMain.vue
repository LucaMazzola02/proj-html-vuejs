<template>
    <FusionLayout />
    <CardList /> 
    <AppTutorial /> 
    <div class="spacer flex">READ OUR BLOG
        <i class="fa-solid fa-arrow-right"></i>
    </div>
    <ForumLayout />
    <div class="spacer flex">GO TO OUR FORUM
        <i class="fa-solid fa-arrow-right"></i>
    </div>
    <AppCommunity />
    <AppCta />
</template>

<script>
import FusionLayout from './FusionLayout.vue' 
import CardList from './CardList.vue' 
import ForumLayout from './ForumLayout.vue' 
import AppCommunity from './AppCommunity.vue' 
import AppCta from './AppCta.vue' 
import AppTutorial from './AppTutorial.vue' 


export default {
    name: 'AppMain',
    components:{
        FusionLayout,
        CardList,
        ForumLayout,
        AppCommunity,
        AppCta,
        AppTutorial

    }
}
</script>



<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
  
</style>

  