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
  min-height: 50%;
  max-height: 50%;
  word-wrap: break-word;
  overflow-y: auto;
  padding: 20px; 
  background-color: rgb(0, 0, 0);
  color: white;
}
h3 {
  font-size: 16px;
}

</style>
