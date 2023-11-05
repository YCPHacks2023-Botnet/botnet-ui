<template>
    <div class="details">
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
    width: 100%;
    height: 50%;
    padding: 20px; 
    background-color: rgb(102, 134, 102);
  }
  </style>
  