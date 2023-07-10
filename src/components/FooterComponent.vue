<template>
    <footer class="footer">
      <div class="container">
        <div class="footer-content">
          <div class="footer-links">
            <router-link to="/" class="footer-link">Home</router-link>
            <router-link to="/about" class="footer-link">About</router-link>
            <router-link to="/portfolio" class="footer-link">Portfolio</router-link>
          </div>
          <div class="footer-social">
            <a href="https://github.com/Paaless" target="_blank" rel="noopener noreferrer" class="social-link">
              <i class="fab fa-github"></i>
            </a>
            <a href="https://www.linkedin.com/in/razvan-aviv-palie-32b2b7212/" target="_blank" rel="noopener noreferrer" class="social-link">
              <i class="fab fa-linkedin"></i>
            </a>
          </div>
        </div>
        <div class="footer-text">
          <p>&copy; 2023 My Portfolio. All rights reserved.</p>
        </div>
      </div>
    </footer>
  </template>
  
  <script>
  import '@fortawesome/fontawesome-free/css/all.css'
  export default {
    name: 'FooterComponent',
    // Component options
  }
  </script>
  
  <style scoped>
  .footer {
    background-color: #f8f8f8;
    padding: 20px 0;
    text-align: center;
  }
  
  .footer-content {
    max-width: 1200px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  
  .footer-links {
    display: flex;
  }
  
  .footer-link {
    margin-right: 10px;
    color: #333;
    text-decoration: none;
  }
  
  .footer-link:hover {
    text-decoration: underline;
  }
  
  .footer-social {
    display: flex;
  }
  
  .social-link {
    margin-right: 10px;
    color: #333;
    font-size: 24px;
    text-decoration: none;
  }
  
  .social-link:hover {
    color: #0077B5;
  }
  
  .footer-text {
    font-size: 14px;
    color: #666;
  }
  </style>
  