<script setup>
import Header from './components/Header.vue'
import BotsList from './components/BotsList.vue'
import SectionTitle from './components/SectionTitle.vue'
</script>

<template>
  <!-- Header of the page -->
  <div class="wrapper">
    <Header msg="Dotnetbotnet Overview" />
  </div>

  <!-- Main content section -->
  <div class="LeftSide">
    <SectionTitle msg="List of Connected Bots"/>
    <BotsList></BotsList>
  </div>

</template>

<style scoped>
.LeftSide {
  max-width: 40%;
  min-width: 40%;
  margin-left: 1%;
}
</style>
