<template>
  <section class="intro-section">
    <div class="container">
      <h2 class="section-title">{{ title }}</h2>
      <div class="section-content">
        <div class="left-content">
          <img src="../assets/profile.jpg" class="profile-pic">
          <div>
            <img src="../assets/romania-flag-icon-256.png" class="flag">
            <img src="../assets/united-kingdom-flag-small.png" class="flag">
          </div>
          
        </div>
        <div class="right-content">
          <p>
            Welcome to my online portfolio, where passion meets proficiency and
            creativity merges with code. As a final year Computer Science
            student eagerly embarking on a new professional chapter, I invite
            you to explore my digital domain. Discover the captivating world of
            web development as VueJS takes center stage, transforming ideas into
            interactive and visually stunning front-end experiences. Journey
            into the realm of back-end wizardry, where .NET, Python, C++, and
            Java seamlessly harmonize to build robust and scalable solutions.
            But my learning doesn't stop there. Delve into the depths of data
            management as I explore the power of NoSQL databases like MongoDB,
            enabling flexible and efficient data storage, and SQL databases like
            SQLite, fostering structured and relational data management. With a
            strong foundation in both the art and science of programming, I am
            poised to tackle the challenges of the modern tech landscape. From
            crafting elegant code architecture to creating intuitive user
            interfaces, my portfolio is a testament to my dedication and drive.
          </p>
          <p>
            Whether you're an industry professional seeking fresh talent or a
            curious visitor eager to witness the evolution of a budding
            technologist, I invite you to immerse yourself in the diverse
            projects and accomplishments showcased here. Let's embark on this
            journey together, as I strive to contribute my skills, knowledge,
            and unyielding enthusiasm to the ever-evolving world of technology.
          </p>
        </div>
      </div>
      <div class="cta-button">
        <router-link to="/about" class="btn">Get in Touch</router-link>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "HomeComponent",
  props: {
    title: {
      type: String,
      required: true,
    },
  },
};
</script>

<style scoped>
.intro-section {
  
  padding: 40px 0;
  background-color: #f9f9f9;
  text-align: center;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
}
.left-content{
  justify-content: center;
  
}
.right-content{
  flex-grow: 1;
}
.profile-pic {
  width: 150px; /* Adjust the width as needed */
  height: 150px; /* Adjust the height as needed */
  border-radius: 50%; /* Make the image circular */
  object-fit: cover; /* Ensure the image fills the container without distortion */
  border: 3px solid #1a1b1d; /* Add a border color matching Facebook's blue */
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2); /* Add a subtle box shadow */
}
.flag{
  width: 30px;
  height: 20px;
  padding: 5px;
}
.section-title {
  font-size: 24px;
  margin-bottom: 20px;
}
.section-content {
  display: grid;
    grid-template-columns: 25% 75%;
}
p {
  font-size: 18px;
  margin-bottom: 30px;
  text-align: left;
  text-indent: 5%;
}

.cta-button {
  margin-top: 20px;
}

.btn {
  margin-left: 10px;
  padding: 10px 20px;
  background-color: #2196f3;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  text-decoration-line: none;
}
.btn:hover {
  background-color: #1976d2;
}
</style>
