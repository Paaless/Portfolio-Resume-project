<template>
    <div class="about-page">
  
    <HeaderComponent :button1Text="button1Text" :button2Text="button2Text" :button1Route="button1Route" :button2Route="button2Route"/>
      <h2 class="section-title">
       Here is some information about me and how you can get in touch with me
      </h2>
      <AboutComponent/>
      <FooterComponent/>
    </div>
  </template>
  
  <script>
  import HeaderComponent from '@/components/HeaderComponent.vue';
  import FooterComponent from '@/components/FooterComponent.vue';
  import AboutComponent from  '@/components/AboutComponent.vue'
  export default {
    name: 'WelcomePage',
    components: {
    HeaderComponent,
    AboutComponent,
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
  .section-title {
  font-size: 24px;
  margin-bottom: 20px;
}
  </style>
  