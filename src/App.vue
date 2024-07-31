<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppMainBottom from './components/AppMainBottom.vue';
import AppFooterTop from './components/AppFooterTop.vue';
import AppFooterBottom from './components/AppFooterBottom.vue';
import AppCards from './components/AppCards.vue';
export default{
    components:{
        AppHeader,
        AppMain,
        AppMainBottom,
        AppFooterTop,
        AppFooterBottom,
        AppCards,
    }
}
</script>

<template>
  <header>
    <AppHeader />
  </header>
  <main>
    <AppMain/>
  </main>
  <footer>
    <AppFooterTop />
    <AppFooterBottom />
  </footer>
</template>

<style lang="scss" >
@import './styles/generals.scss';
</style>
