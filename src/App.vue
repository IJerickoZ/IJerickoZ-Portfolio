<template>
    <div id="app">
        <Introduce />
        <Skills/>
        

  </div>
</template>

<script>
import Introduce from './sections/Introduce.vue'
import Skills from './sections/Skills.vue'
export default {
  name: 'App',
  components: { Introduce, Skills }
}
</script>

<style>
</style>
