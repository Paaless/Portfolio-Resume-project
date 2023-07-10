<template>
  <section class="intro-section">
    <div class="container">
      <h2 class="section-title">{{ title }}</h2>
      <p>
        Welcome to my online portfolio, where passion meets proficiency and
        creativity merges with code. As a final year Computer Science student
        eagerly embarking on a new professional chapter, I invite you to explore
        my digital domain. Discover the captivating world of web development as
        VueJS takes center stage, transforming ideas into interactive and
        visually stunning front-end experiences. Journey into the realm of
        back-end wizardry, where .NET, Python, C++, and Java seamlessly
        harmonize to build robust and scalable solutions. But my learning
        doesn't stop there. Delve into the depths of data management as I
        explore the power of NoSQL databases like MongoDB, enabling flexible and
        efficient data storage, and SQL databases like SQLite, fostering
        structured and relational data management. With a strong foundation in
        both the art and science of programming, I am poised to tackle the
        challenges of the modern tech landscape. From crafting elegant code
        architecture to creating intuitive user interfaces, my portfolio is a
        testament to my dedication and drive.
      </p>
      <p>
        Whether you're an industry professional seeking fresh talent or a
        curious visitor eager to witness the evolution of a budding
        technologist, I invite you to immerse yourself in the diverse projects
        and accomplishments showcased here. Let's embark on this journey
        together, as I strive to contribute my skills, knowledge, and unyielding
        enthusiasm to the ever-evolving world of technology.
      </p>
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

.section-title {
  font-size: 24px;
  margin-bottom: 20px;
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
.btn:hover{
    background-color: #1976D2;
  }

</style>
