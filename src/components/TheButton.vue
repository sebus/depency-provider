<!-- Composant Button.vue -->

<script setup>
// Import de la fonction 'inject'
import { inject } from 'vue'

// Injection du provider nommé 'Store'
const Store = inject('Store')

// Fonction pour modifier la valeur du message
const updateMessage = () => {
  Store.message.value = 'Ce message a été modifié'
  // 👆 Pensez au '.value' car c'est une 'ref'
}
</script>

<template>
  <div><button @click="updateMessage">Modifier le message</button></div>
</template>

<style scoped>
div {
  margin: 0 auto;
  background-color: aqua;
  padding: 48px;
}
</style>
