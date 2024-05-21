<script setup lang="ts">
import { ref } from 'vue'
import ModalWrapper from '@/components/ModalWrapper.vue'

const modalOpen = ref(false)
</script>

<template>
  <div class="body">
    <h1>Recursive Vue Modal Testing</h1>
    <button @click="modalOpen = !modalOpen">Launch Modal</button>
  </div>
  <ModalWrapper :modalOpen="modalOpen" />
</template>

<style scoped lang="scss">
.fade-e .body {
  width: 100%;
  height: 100%;
}
</style>
