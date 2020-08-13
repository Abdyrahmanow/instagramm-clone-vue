<template>
  <div id="app">
    <MainHeader />
    <router-view />
  </div>
</template>

<script>
import MainHeader from '@/components/Header'
export default {
  name: 'App',
  components: {
    MainHeader
  }
}
</script>

<style scoped></style>
