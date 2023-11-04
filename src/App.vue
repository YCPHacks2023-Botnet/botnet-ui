<script setup>
import Header from './components/general/Header.vue'
import BotsList from './components/botslistsection/BotsList.vue'
import SectionTitle from './components/botslistsection/SectionTitle.vue'
import Count from './components/bottom/count/Count.vue'
import Params from './components/bottom/params/Params.vue'
import Queue from './components/bottom/queue/Queue.vue'
import TaskMenu from './components/bottom/tasks/TaskMenu.vue'
import BotTermOutput from './components/botslistinfosection/BotTermOutput.vue'
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

  <!-- <div class="details-terms">
    <BotTermOutput />
  </div> -->

  <div class="flex-container">
    <div>
      <Count />
      <TaskMenu />
    </div>
    <Params />
    <Queue />
  </div>

</template>

<style scoped>
.botlistsection {
  max-width: 30%;
  min-width: 30%;
  margin-left: 1%;
  max-height: 100%;
  min-height: 100%;
}
.details-terms {
  position: absolute;
  top: 0;
  display: flex;
  flex-direction: row;
  justify-content: right;
  align-items: flex-end;
  margin: 1%;
  height: 60%;
}
.flex-container{
  position: absolute;
  bottom: 0;
  right: 0;
  display: flex;
  flex-direction: row;
  justify-content: right;
  align-items: flex-end;
  margin: 1%;
  height: 30%;
}
</style>
