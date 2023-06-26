<template>
  <AppHeader />
  <AppJumbotron/>
  <AppMain />
  <AppFooter />
</template>

<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppJumbotron from './components/Appjumbotron.vue';


export default {
    name: 'App',
    components:{
      AppHeader,
      AppMain,
      AppFooter,  
      AppJumbotron
    }
}
</script>

<style lang="scss">
  @import './styles/general.scss';
</style>
