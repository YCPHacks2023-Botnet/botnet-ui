<script setup>
import Header from './components/Header.vue'
import BotsList from './components/BotsList.vue'
import SectionTitle from './components/SectionTitle.vue'
import Count from './components/Count.vue'
import Params from './components/Params.vue'
import Queue from './components/Queue.vue'
import TaskMenu from './components/TaskMenu.vue'
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

  <div class="flex-container">
    <Count />
    <TaskMenu />
    <Params />
    <Queue />
  </div>

</template>

<style scoped>
.LeftSide {
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
