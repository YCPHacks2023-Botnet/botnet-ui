<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>

<template>
  <!-- Definition of custome page header with styling -->
  <div>
    <h1 class="customHeader">{{ msg }}</h1>
  </div>
</template>

<style scoped>
h1 {
  font-size: 40px;
  font-weight: bold;
  color: lightblue;
  margin-left: 1%;
}
</style>