<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>

<template>
  <div class="greetings">
    <h1 class="blue">{{ msg }}</h1>
  </div>
</template>

<style scoped>
h1 {
  
}

h3 {
  
}

.greetings h1,
.greetings h3 {
  
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    
  }
}
</style>
