<template>
  <div class="app">
    <AppIcons />
    <AppHeader />
    <AppJumbotron/>
    <AppMain />
    <AppFooter />
  </div>
  
</template>

<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppJumbotron from './components/AppJumbotron.vue';
import AppIcons from './components/AppIcons.vue';


export default {
    name: 'App',
    components:{
      AppHeader,
      AppMain,
      AppFooter,  
      AppJumbotron,
      AppIcons
    }
}
</script>

<style lang="scss">
  @import './styles/general.scss';

  .app{
    position: relative;
  }
</style>
