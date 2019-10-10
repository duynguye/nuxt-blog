<template>
  <section class="posts-list">
    <PostPreview 
      id="1" 
      :is-admin="isAdmin"
      thumbnail="https://images.pexels.com/photos/373543/pexels-photo-373543.jpeg" 
      title="Post Title" 
      preview-text="Post Content" 
    />

    <PostPreview 
      id="1"
      :is-admin="isAdmin"
      thumbnail="https://images.pexels.com/photos/373543/pexels-photo-373543.jpeg"
      title="Post Title"
      preview-text="Post Content"
    />

    <PostPreview 
      id="1"
      :is-admin="isAdmin"
      thumbnail="https://images.pexels.com/photos/373543/pexels-photo-373543.jpeg"
      title="Post Title"
      preview-text="Post Content"
    />
  </section>
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
      default: false
    }
  }
}
</script>

<style scoped>
.posts-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>