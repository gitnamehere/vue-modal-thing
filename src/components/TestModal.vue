<script setup lang="ts">
import App from '@/App.vue'
</script>

<template>
  <div class="modal">
    <div class="modal__header">Header</div>
    <div class="modal__body">
      <App />
    </div>
  </div>
</template>

<style lang="scss">
.modal {
  position: absolute;
  display: flex;
  flex-direction: column;
  overflow: hidden;
  inset: 0;
  margin: auto;
  width: 95%;
  height: 95%;
  background-color: white;
  border: 4px solid black;
  border-radius: 16px;

  &__header {
    display: flex;
    width: 100%;
    min-height: 32px;
    align-items: center;
    justify-content: center;
    background-color: #333;
    border-radius: 12px 12px 0 0;
    border-bottom: 4px solid black;
    color: white;
  }

  &__body {
    display: flex;
    flex: 1;
    padding: 0;
    box-sizing: border-box;
  }
}
</style>
