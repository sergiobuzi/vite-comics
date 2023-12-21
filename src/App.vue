<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppShop from './components/AppShop.vue';

export default {
  components:{
    AppHeader,
    AppMain,
    AppShop
  }
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppShop />
</template>

<style lang="scss">
  @use './styles/general.scss' as *;
  @use './styles/partials/variables' as *;
</style>
