<template>
  <h1 class="text-center">{{ msg }}</h1>

  <p class="text-center">
    <a href="https://vitejs.dev/guide/features.html" target="_blank">
      Vite Documentation
    </a>
    |
    <a href="https://v3.vuejs.org/" target="_blank">Vue 3 Documentation</a>
  </p>

  <button type="button" @click="state.count++">count is: {{ state.count }}</button>
  <p class="text-center">
    Edit
    <code>components/HelloWorld.vue</code> to test hot module replacement.
  </p>

  <p class="text-center">Using vue to do this</p>

</template>

<script setup>
import { defineProps, reactive } from 'vue'

defineProps({
  msg: String
})

const state = reactive({ count: 0 })
</script>

<style scoped>
a {
  color: #000;
}
</style>
