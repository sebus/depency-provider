<!-- Composant HomeView.vue -->

<script setup>
// Import des fonctions
import { provide, ref } from 'vue'

// Import des composants
import ChangeMessage from '@/components/ChangeMessage.vue'
import DescriptionMessage from '@/components/DescriptionMessage.vue'

// Création de la valeur
const message = ref('Message initial Yeah !')

// Initialisation du provider
provide('Store', { message: message })
</script>

<template>
  <main>
    <h1>Page d'accueil</h1>

    <DescriptionMessage />
    <ChangeMessage />
  </main>
</template>
