<template>
    <div class="details">
      <h3>
        <slot name="heading"></slot>
      </h3>
      <slot></slot>
    </div>
</template>

<style scoped>
.details {
  width: 100%;
  min-height: 40%;
  max-height: 40%;
  word-wrap: break-word;
  overflow-y: auto;
  padding: 20px; 
  background-color: black;
  border: 2px dotted white;
  color: white;
  overflow-y: auto;
}
h3 {
  font-size: 16px;
  text-align: center;
}

</style>
