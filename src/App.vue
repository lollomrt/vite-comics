<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppIconList from './components/AppIconList.vue'
import AppFooter from './components/AppFooter.vue'
export default {
  components: {
    AppHeader,
    AppMain,
    AppIconList,
    AppFooter
  }
}
</script>

<template lang="">
  <div>
    <AppHeader></AppHeader>
    <AppMain></AppMain>
    <AppIconList></AppIconList>
    <AppFooter></AppFooter>
  </div>
  
</template>

<style lang="scss">
@use './styles/generals.scss' as *;
</style>
