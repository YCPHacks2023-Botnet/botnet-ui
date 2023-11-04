<template>
  <div class="item">
    <div class="details">
      <h3>
        <slot name="heading"></slot>
      </h3>
      <slot></slot>
    </div>
  </div>
</template>

<style scoped>
.details {
  width: 100px;
  margin: 0 auto;
  margin-left: 5px;
  margin-right: 5px; 
  padding: 20px; 
  background-color: lightblue;
}
</style>
