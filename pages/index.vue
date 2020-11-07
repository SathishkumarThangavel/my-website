<template>
  <div>
    <div class="container">
      <div class="hero">
        <div class="profile">
          <img src="~/assets/me.jpg">
          <h2 class="profile-name">Sathishkumar Thangavel</h2>
          <h3>Frontend Engineer</h3>
          <h3><a href="https://freshworks.com">Freshworks</a></h3>
        </div>
      </div>
    </div>
    <AboutMe/>
    <Footer/>
  </div>
</template>

<script>
import AboutMe from '~/components/AboutMe.vue';
import Footer from '~/components/Footer.vue';

export default {
  components: {
    AboutMe,
  }
}
</script>

<style scoped>
  .container {
    background: #000;
  }
  .hero {
    max-width: 80%;
    margin: auto;
    color: #fff;
  }
  .profile {
    text-align: center;
    padding: 100px 10px;
  }
  .profile-name {
    font-size: 35px;
    margin:20px 0 10px;
  }
  h3 {
    margin-bottom: 10px;
  }
  a {
    color: #409EFF;
    text-decoration: none;
  }
  img {
    width: 200px;
    height: 200px;
    border-radius: 50%;
  }
</style>
