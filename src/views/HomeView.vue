<template>
  <div class="home">
    <Landing msg="Welcome to Your Vue.js App"/>
  </div>
  <div class="container"></div>
</template>

<script>
// @ is an alias to /src
import Landing from '@/components/Landing.vue'

export default {
  name: 'HomeView',
  components: {
    Landing
  }
}
</script>
