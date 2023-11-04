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
  font-size: 24px;
  font-weight: none;
  color: orange;
  text-align: center;
  border: 2px solid white;
}
</style>