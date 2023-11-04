<template>
  <div class="item">
    <i>
      <slot name="icon"></slot>
    </i>
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
  
}

i {
  
}

h3 {
  
}

@media (min-width: 1024px) {
  .item {
    
  }

  i {
    
  }

  .item:before {
   
  }

  .item:after {
   
  }

  .item:first-of-type:before {
  
  }

  .item:last-of-type:after {
   
  }
}
</style>
