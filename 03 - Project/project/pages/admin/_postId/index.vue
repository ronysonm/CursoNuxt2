<template>
   <div class="admin-new-post-page">
    <section class="new-post-form">
        <AdminPostForm  :post="loadedPost" />
    </section>
   </div>
</template>

<script>
import AdminPostForm from '@/components/Admin/AdminPostForm'

export default {
    components: {
        AdminPostForm
    },
    data() {
         return {
            loadedPost: {
                author: 'Ronyson',
                title: 'My great post!',
                thumbnailLink: 'https://img.olhardigital.com.br/wp-content/uploads/2021/12/Code-1000x450.jpg',
                content: 'This is my greatest post on the blog!'
            }
         }
    },
    layout: 'admin'
}
</script>

<style>

</style>