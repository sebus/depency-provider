<script setup>
// import de la fonction 'inject'
import { inject } from 'vue'

// Injection du provider nommé 'Store'
const Store = inject('Store')
</script>
<template>
  <div>
    <p>{{ Store.message.value }}</p>
  </div>
</template>
<style scoped>
div {
  margin: 0 auto;
  background-color: antiquewhite;
  padding: 48px;
}
</style>
