<script setup lang="ts">
import TestModal from '@/components/TestModal.vue'

interface Props {
  modalOpen: boolean
}

defineProps<Props>()
</script>

<template>
  <Transition>
    <TestModal v-if="modalOpen" />
  </Transition>
</template>

<style>
.v-enter-active {
  transition:
    width 0.35s ease,
    opacity 0.35s ease,
    height 0.5s 0.25s ease;
}

.v-leave-active {
  transition:
    width 0.35s 0.5s ease,
    opacity 0.35s 0.5s ease,
    height 0.5s ease;
}

.v-enter-from,
.v-leave-to {
  opacity: 0;
  height: 32px;
  width: 32px;
}
</style>
