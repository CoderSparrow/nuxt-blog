<template>
  <section>
    <el-row type="flex" class="post-container">
      <el-col v-for="post in 5" :xs="24" :sm="12" :md="12" :lg="8">
        <PostPreview/>
      </el-col>
    </el-row>
  </section>
</template>

<script>
import PostPreview from "@/components/main/Post/PostPreview";

export default {
  head: {
    title: 'Главная'
  },
  components: {
    PostPreview
  }
}
</script>

<style lang="scss" scoped>
  .post-container {
    flex-wrap: wrap;
  }
</style>
