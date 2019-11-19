<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/hqdefault.jpg">
    <HelloWorld msg="Felix qui potuit rerum cognoscere causas"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'home',
  components: {
    HelloWorld
  }
}
</script>
