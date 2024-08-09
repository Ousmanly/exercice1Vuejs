<template>
  <section>
    <h1>Liste des employes</h1>
    <ol>
      <li v-for="employe in employes" :key="employe.id" @mousemove="MouseOver" @mouseleave="MouseLeave" >
        {{ employe.prenom }} {{ employe.nom }}
      </li>
    </ol>
  </section>
</template>

<script setup>
const props = defineProps({
  employes:Array
})

function MouseOver(event) {
  event.target.style.color="blue";
  event.target.style.backgroundColor= "aliceblue";
}
function MouseLeave(event) {
  event.target.style.color="";
  event.target.style.backgroundColor= "";
}
</script>

<style scoped>
  li{
    color: rgb(108, 108, 199);
    width: 200px;
    padding: 7px;
  }
  section{
    width: fit-content;
    margin: 100px auto;
  }
</style>