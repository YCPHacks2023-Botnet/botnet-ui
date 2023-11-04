
<!-- Creates a block component of the bots name as a clickable button -->
<template>
  <p>
    <slot name="first"></slot> <!-- slot in which to send name retrieved from JSON file -->
  </p>
  <p>
    <slot name="middle"></slot> <!-- slot in which to send name retrieved from JSON file -->
  </p>
  <p>
    <slot name="last"></slot> <!-- slot in which to send name retrieved from JSON file -->
  </p>
</template>

<style scoped>
p {
  margin-top: 0px;
  margin-bottom: 0px;
  padding: 0px;
}
.BotNameButton {
  color: white;
  font-size: 14px;
  width: 100px;
  height: 100px;
}
</style>
