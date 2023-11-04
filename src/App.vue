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

  <SectionTitle class="listofbots" msg="List of Connected Bots"/>
  <!-- Main content section -->
  <div class="botlistsection">
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
.listofbots {
  margin: 1% 2% 0% 2%;
  width: 20%;
}
.botlistsection {
  width: 20%;
  margin: 1% 2%;
  background-color: rgba(0, 8, 42, 0.612);
  padding: 1%;
  max-height: 80%;
  min-height: 80%;
  border: 2px dotted white;
  overflow-y: auto;
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
