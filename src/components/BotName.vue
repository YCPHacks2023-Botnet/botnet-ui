
<!-- Creates a block component of the bots name as a clickable button -->
<template>
  <button class="BotNameButton">
    <slot name="Name"></slot> <!-- slot in which to send name retrieved from JSON file -->
  </button>
</template>

<style scoped>
.BotNameButton {
  background-color: green;
  border: 3px solid black;
  color: white;
  font-size: 20px;
}
</style>
