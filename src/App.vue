<template>
  <div id="app">
    <Header />
    <router-view></router-view>
  </div>
</template>

<script>
import './assets/css/style.css'
import Header from './components/ui/Header.vue'

export default {
  components: {Header}
}
</script>
