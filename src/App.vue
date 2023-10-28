<script setup>
import TheWelcome from './components/TheWelcome.vue'
import Loadding from './components/Loadding.vue'
import { ref,onMounted } from 'vue';
const show = ref(false)

onMounted(()=>{
  setTimeout(()=>{
    show.value = true
  },2000)
})
</script>

<template>
  <main>
    <TheWelcome v-if="show"/>
    <Loadding v-else/>
  </main>
</template>

<style scoped>
</style>
