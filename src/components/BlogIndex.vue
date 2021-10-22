<template>
     <BlogTopHeader/>
    <main>
        <BlogAside/>
       <BlogList/>
    </main>
</template>

<script>
import BlogAside from './BlogAside.vue'
import BlogList from './BlogList.vue'
import BlogTopHeader from './BlogTopHeader.vue'
export default {
  components: { BlogList, BlogAside, BlogTopHeader },
    
}
</script>

<style scoped>

</style>