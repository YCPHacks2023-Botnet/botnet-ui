<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>

<template>
  <!-- Definition of custom section header with styling -->
    <h3>{{ msg }}</h3>
</template>

<style scoped>
h3 {
  font-size: 26px;
  font-weight: bold;
  color: white;
  text-align: center;
}
</style>