<template>
  <div class="admin-post-page">
    <section class="update-form">
      <AdminPostForm :post="loadedPost" />
    </section>
  </div>
</template>

<script>
import AdminPostForm from '@/components/Admin/AdminPostForm'

export default {
  layout: 'admin',
  components: {
    AdminPostForm
  },

  data() {
    return {
      loadedPost: {
        author: 'Andy Nguyen',
        title: 'This Post',
        content: 'Super Amazing content.',
        thumbnailLink: 'https://images.pexels.com/photos/373543/pexels-photo-373543.jpeg'
      }
    }
  }
}
</script>

<style scoped>
.update-form {
  width: 90%;
  margin: 20px auto;
}

@media (min-width: 768px) {
  .update-form {
    width: 500px;
  }
}
</style>
