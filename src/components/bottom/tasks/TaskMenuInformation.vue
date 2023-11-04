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
  padding: 15px; 
  margin-left: 5px;
  margin-right: 5px; 
  margin-top: 5px;
  margin-bottom: 5px;
  text-align: center;
  background-color: lightblue;
}
</style>
