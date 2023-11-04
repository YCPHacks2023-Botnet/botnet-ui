<script setup>
import BotName from './BotName.vue'
</script>

<!-- This will create the table to pupulate with selectable BotName blocks -->
<!-- shitty placeholder for the time to get the rest of the page laid out -->
<template>
  <div class="container">
    <table>
      <tr>
        <td>
          <!-- an instance of a selectable bot name block-->
          <BotName>
            <template #Name>From JSON</template>
          </BotName>
        </td>
        <td>
          <!-- an instance of a selectable bot name block-->
          <BotName>
            <template #Name>From JSON</template>
          </BotName>
        </td>
        <td>
          <!-- an instance of a selectable bot name block-->
          <BotName>
            <template #Name>From JSON</template>
          </BotName>
        </td> 
      </tr>
    </table>
  </div>
</template>

<style scoped>
.container {
  max-height: 50%;
  min-height: 50%;
  margin-top: 0%;
  margin-bottom: auto;
  max-width: 100%;
  min-width: 100%;
}
table {
  display: flex;
  flex-wrap: wrap;
  padding: 1%;
  border: 2px solid white;
  max-width: 100%;
  min-width: 100%;
}
thead, tr, tbody {
  display:block;
}
</style>