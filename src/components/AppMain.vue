<template>
    <FusionLayout />
    <CardList />  
</template>

<script>
import FusionLayout from './FusionLayout.vue' 
import CardList from './CardList.vue' 


export default {
    name: 'AppMain',
    components:{
        FusionLayout,
        CardList,
    }
}
</script>



<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
  
</style>

  