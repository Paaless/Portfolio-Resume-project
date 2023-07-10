<template>
    <header class="header">
      <h1>My Portfolio</h1>
      <div class="button-container">
        <router-link :to="button1Route" class="header-button">{{ button1Text }}</router-link>
        <router-link :to="button2Route" class="header-button">{{ button2Text }}</router-link>
      </div>
    </header>
  </template>
  
  <script>
export default {
  name: 'HeaderComponent',
  props: {
    button1Text: {
      type: String,
      default: 'Button 1',
    },
    button2Text: {
      type: String,
      default: 'Button 2',
    },
    button1Route: {
      type: String,
      default: 'Button 1',
    },
    button2Route: {
      type: String,
      default: 'Button 2',
    },
  },
  // Component options
}
</script>
  
  <style scoped>
  .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
  }
  
  .button-container {
    display: flex;
    justify-content: flex-end;
  }
  
  .header-button {
    margin-left: 10px;
    padding: 10px 20px;
    background-color: #2196F3;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    text-decoration-line: none;
  }
  
  .header-button:hover {
    
    background-color: #1976D2;
  }
  </style>