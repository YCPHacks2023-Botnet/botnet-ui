<template>
    <div class="details">
      <h4><slot name="botname"></slot></h4>
      <p>ID:</p>
      <p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<slot name="botID"></slot></p>
      <p>CPU:</p>
      <p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<slot name="CPU"></slot></p>
      <p>RAM:</p>
      <p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<slot name="RAM"></slot></p>
      <p>Activity Status:</p>
      <p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<slot name="status"></slot></p>
      <p>Current Task:</p>
      <p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<slot name="currenttask"></slot></p>
      <p>Task Parameters:</p>
      <p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<slot name="taskparams"></slot></p>
    </div>
  </template>
  
  <style scoped>
  .details {
    width: 100%;
    height: 60%;
    padding: 20px; 
    background-color: black;
    border: 2px dotted white;
    color: white;
  }
  h4 {
    margin-bottom: 5%;
    text-align: center;
  }
  p {
    font-size: 14px;
    line-height: 0.3;
  }
  </style>
  