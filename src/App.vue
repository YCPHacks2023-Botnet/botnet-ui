<script setup>
import Header from './components/general/Header.vue'
import BotsList from './components/botslistsection/BotsList.vue'
import SectionTitle from './components/botslistsection/SectionTitle.vue'
</script>

<template>
  <!-- Header of the page -->
  <div class="wrapper">
    <Header msg="Dotnetbotnet Overview" />
  </div>

  <!-- Main content section -->
  <div class="botlistsection">
    <SectionTitle msg="List of Connected Bots"/>
    <BotsList></BotsList>
  </div>

</template>

<style scoped>
.botlistsection {
  max-width: 40%;
  min-width: 40%;
  margin-left: 1%;
}
</style>
