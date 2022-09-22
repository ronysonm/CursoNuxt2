<template>
  <div class="featured-posts">
    <PostPreview 
        id="1"
        :is-admin="isAdmin"
        thumbnail="https://img.olhardigital.com.br/wp-content/uploads/2021/12/Code-1000x450.jpg"
        title="First post!"
        previewText="This is my firts post!"
      />
      <PostPreview 
        id="2"
        :is-admin="isAdmin"
        thumbnail="https://img.olhardigital.com.br/wp-content/uploads/2021/12/Code-1000x450.jpg"
        title="Second post!"
        previewText="This is my second post!"
      />
      <PostPreview 
        id="1"
        :is-admin="isAdmin"
        thumbnail="https://img.olhardigital.com.br/wp-content/uploads/2021/12/Code-1000x450.jpg"
        title="Third post!"
        previewText="This is my third post!"
      />
  </div>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'
export default {
    components: {
        PostPreview
    },
    props: {
        isAdmin: {
            type: Boolean,
            required: false
        }
    }
}
</script>

<style>
.featured-posts {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>