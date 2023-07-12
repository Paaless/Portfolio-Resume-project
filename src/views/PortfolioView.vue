<template>
    <div class="portfolio-page">
      <HeaderComponent :button1Text="button1Text" :button2Text="button2Text" :button1Route="button1Route" :button2Route="button2Route"/>
      <h2 class="section-title">These are my personal projects or projects from my Computer Science classes</h2>
      <GithubProjectsContainer/>
      <FooterComponent/>
    </div>
  </template>
  
  <script>
  import HeaderComponent from '@/components/HeaderComponent.vue';
  import FooterComponent from '@/components/FooterComponent.vue';
  import GithubProjectsContainer from '@/components/GithubProjectsContainer.vue'
  export default {
    name: 'WelcomePage',
    components: {
    HeaderComponent,
    FooterComponent,
    GithubProjectsContainer,
},
    data() {
      return {
        button1Text: 'Home',
        button2Text: 'About',
        button1Route: "/",
        button2Route: "/about"
      };
    },
    // Rest of your component options
  }
  </script>
  
  <style scoped>
  .section-title{
    font-size: 24px;
    margin-bottom: 20px;
  }
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
  