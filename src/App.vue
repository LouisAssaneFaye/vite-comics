<script>
import appHeader from './components/appHeader.vue';
import appMain from './components/appMain.vue';
import appFooter from './components/appFooter.vue';

export default {
  name: 'app',
  components:{
    appHeader,
    appMain,
    appFooter
  }
}

</script>

<template>
  <appHeader />
  <appMain />
  <appFooter />
</template>

<style lang="scss">
  @import './styles/general.scss' ;

</style>
