<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppMainBottom from './components/AppMainBottom.vue';
import AppFooterAllLinks from './components/AppFooterAllLinks.vue';
import AppFooterSocial from './components/AppFooterSocial.vue';
export default{
    components:{
        AppHeader,
        AppMain,
        AppMainBottom,
        AppFooterAllLinks,
        AppFooterSocial,
    }
}
</script>

<template lang="">
  <header>
    <AppHeader />
  </header>
  <main>
    <AppMain />
    <AppMainBottom />
  </main>
  <footer>
    <AppFooterAllLinks />
    <AppFooterSocial />
  </footer>
</template>

<style lang="scss" >
@use './styles/generals.scss';
</style>
