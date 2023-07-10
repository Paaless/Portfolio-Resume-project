<template>
    <div class="about-page">
  
    <HeaderComponent :button1Text="button1Text" :button2Text="button2Text" :button1Route="button1Route" :button2Route="button2Route"/>
      <p>
       ABOUT PAGE
      </p>
      <FooterComponent/>
    </div>
  </template>
  
  <script>
  import HeaderComponent from '@/components/HeaderComponent.vue';
  import FooterComponent from '@/components/FooterComponent.vue';
  export default {
    name: 'WelcomePage',
    components: {
    HeaderComponent,
    FooterComponent
},
    data() {
      return {
        button1Text: 'Home',
        button2Text: 'Portfolio',
        button1Route: "/",
        button2Route: "/portfolio"
      };
    },
    // Rest of your component options
  }
  </script>
  
  <style scoped>
  .welcome-page {
    text-align: center;
    padding: 20px;
  }
  .btn {
    display: inline-block;
    margin: 10px;
    padding: 10px 20px;
    background-color: #2196f3;
    color: white;
    text-decoration: none;
    border-radius: 5px;
    transition: background-color 0.3s;
  }
  .btn:hover {
    background-color: #1976d2;
  }
  </style>
  