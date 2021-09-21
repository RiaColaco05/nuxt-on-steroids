<template>
  <div class=" home-page">
    <!-- <nuxt-link to="/users" >Users</nuxt-link> -->
<section class="intro">
  <h1>Get the latest tech news!</h1>
</section>
<section class="featured-posts">
 <PostPreview id="1" previewImg="https://assets.thehansindia.com/h-upload/2021/07/31/1600x960_1092805-tech.jpg" title="hello there first!" previewText="This is my fisrt post!"/>
 <PostPreview id="2" previewImg="https://news.cgtn.com/news/2020-11-02/Analysis-China-is-betting-on-science-and-tech-like-never-before-V68V871ula/img/871ca9ce8b9941088260b6ed4ced4eeb/871ca9ce8b9941088260b6ed4ced4eeb.jpeg" title="hello there second!" previewText="This is my second post!"/>
 <PostPreview id="3" previewImg="https://www.hydrocarbons-technology.com/wp-content/uploads/sites/9/2020/09/shutterstock_1152185600-1440x1008-1-857x600.jpg" title="hello there third!" previewText="This is my third post!"/>
</section>

    <!-- <div>
      <Logo />
      <h1 class="title">
        nuxt-steroids
      </h1>
      <div class="links">
        <a
          href="https://nuxtjs.org/"
          target="_blank"
          rel="noopener noreferrer"
          class="button--green"
        >
          Documentation
        </a>
        <a
          href="https://github.com/nuxt/nuxt.js"
          target="_blank"
          rel="noopener noreferrer"
          class="button--grey"
        >
          GitHub
        </a>
      </div>
    </div> -->
  </div>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'
export default {
  components:{
    PostPreview
  }
}
</script>

<style scoped>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}


.intro {
  height: 300px;
  position: relative;
  padding: 30px;
  box-sizing: border-box;
  background-position: center;
  background-size: cover;
}

.intro h1 {
  position: absolute;
  top: 10%;
  left: 5%;
  width: 90%;
  font-size: 1.5rem;
  color: black;
  background-color: rgb(211, 211, 211);
  padding: 10px;
  border-radius: 10px;
  box-shadow: 3px 3px 3px black;
  box-sizing: border-box;
  border: 1px solid black;
}

@media (min-width: 768px) {
  .intro h1 {
    font-size: 2rem;
  }
}

.featured-posts {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
