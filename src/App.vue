<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooterBlueLinks from './components/AppFooterBlueLinks.vue';
import AppFooterAllLinks from './components/AppFooterAllLinks.vue';
export default{
    components:{
        AppHeader,
        AppMain,
        AppFooterBlueLinks,
        AppFooterAllLinks,
        
    }
}
</script>

<template lang="">
  <header>
    <AppHeader />
  </header>
  <main>
    <AppMain />
  </main>
  <footer>
    <AppFooterBlueLinks />
    <AppFooterAllLinks />
  </footer>
</template>

<style lang="scss" >
@use './styles/generals.scss';
</style>
