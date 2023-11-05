<template>
    <div class="list">
      <h3>
        <slot name="heading"></slot>
      </h3>
      <slot></slot>
    </div>
</template>

<style scoped>
.list {
  width: 100%;
  height: 80%;
  word-wrap: break-word;
  overflow-y: auto;
  padding: 20px; 
  background-color: black;
    border: 2px dotted white;
  color: white;
}
h3 {
  font-size: 16px;
  color: white;
}

</style>
