<template>
<ListeEmployes :employes="employes"/>
</template>
<script setup>
import { ref } from 'vue';
import ListeEmployes from './components/listeEmployes.vue';
const employes = ref([
  {id:1, prenom:"Ousmane", nom:"Ly"},
  {id:1, prenom:"Omar", nom:"Ndiaye"},
  {id:1, prenom:"Abdarahmane", nom:"Thimbo"},
  {id:1, prenom:"Assa", nom:"Bradji"},
])
</script>

<style scoped>

</style>
