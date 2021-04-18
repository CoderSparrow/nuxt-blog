<template>
  <div>
    <Post/>
  </div>
</template>

<script>
import Post from "@/components/main/Post/Post";

export default {
  components: {
    Post
  },
  validate({ params }) {
    return !!params.id
  }
}
</script>

<style scoped>

</style>

