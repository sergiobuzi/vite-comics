<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppShopp from './components/AppShopp.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  components:{
    AppHeader,
    AppMain,
    AppShopp,
    AppFooter

  }
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppShopp />
  <AppFooter />
</template>

<style lang="scss">
  @use './styles/general.scss' as *;
  @use './styles/partials/variables' as *;
</style>
