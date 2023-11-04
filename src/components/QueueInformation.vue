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
.item {
 
}

.details {
  width: 300px;
  margin: 0 auto; 
  padding: 20px; 
  background-color: pink;
}
i {
  
}

h3 {
  
}
</style>
