<template>
  <section>
    <el-row type="flex" justify="center">
      <el-col :xs="24" :sm="18" :md="12" :lg="10">
        <Post v-for="post in 5"/>
      </el-col>
    </el-row>
  </section>
</template>

<script>
import Post from "@/components/main/Post";

export default {
  head: {
    title: 'Главная'
  },
  components: {
    Post
  }
}
</script>

<style>

</style>
