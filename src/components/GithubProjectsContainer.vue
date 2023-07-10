<template>    
  <div>
    <div v-if="isLoading">
      Loading...
    </div>
    <div v-else-if="hasError">
      Error
    </div>
    <div v-else>
      <div class="grid">
        <div class="col" v-for="project in data" :key="project.id">
          <Item 
            :title="project.name" 
            :urlLink="project.html_url" 
            :imageSrc="require('@/assets/logo.png')"
            :tags="project.topics"
            :description="project.description"
          ></Item>
        </div>
      </div>  
    </div>
  </div>
</template>

<script>
import Item from './ItemComponent.vue';
import axios from 'axios';

export default {
  name: 'GithubProjectsContainer',
  components: {
    Item
  },
  data() {
    return {
      data: null,
      isLoading: true,
      hasError: false
    };
  },
  mounted() {
    axios
      .get('https://api.github.com/users/Paaless/repos', {
        headers: {
          'Accept': 'application/vnd.github.mercy-preview+json'
        }
      })
      .then(response => {
        this.data = response.data;
      })
      .catch(error => {
        console.log(error);
        this.hasError = true;
      })
      .finally(() => {
        this.isLoading = false;
      });
  }
};
</script>

<style>
.grid {
  display: flex;
}
.col {
  flex: 1;
}
</style>
