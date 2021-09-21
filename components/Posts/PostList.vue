<template>
            <section class="featured-posts">
 <PostPreview id="1" previewImg="https://assets.thehansindia.com/h-upload/2021/07/31/1600x960_1092805-tech.jpg" title="hello there first!" previewText="This is my fisrt post!"/>
 <PostPreview id="2" previewImg="https://news.cgtn.com/news/2020-11-02/Analysis-China-is-betting-on-science-and-tech-like-never-before-V68V871ula/img/871ca9ce8b9941088260b6ed4ced4eeb/871ca9ce8b9941088260b6ed4ced4eeb.jpeg" title="hello there second!" previewText="This is my second post!"/>
 <PostPreview id="3" previewImg="https://www.hydrocarbons-technology.com/wp-content/uploads/sites/9/2020/09/shutterstock_1152185600-1440x1008-1-857x600.jpg" title="hello there third!" previewText="This is my third post!"/>
</section>
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


.featured-posts {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}

</style>