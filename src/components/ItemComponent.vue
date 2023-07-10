<template> 
    <div>
  
      <a :href="urlLink">
          <img :src="imageSrc" class="item-image" alt="Placeholder image">
      </a>
  
      <div>    
        <p><a :href="urlLink">{{title}}</a></p>
        <div>
          <span v-for="tag in tags" v-bind:key="tag">{{tag}} <br> </span>
        </div>
        <p>{{ description }}</p>
      </div>
  
    </div>
  </template>
  
  <script>
  export default {
    name: 'ItemComponent',
    props: {
      title: String,
      urlLink: String,
      imageSrc: String,
      tags: Array,
      description: String
    }
  }
  </script>
  
  <style>
  .item-image{
      width: 150px;
  }
  </style>