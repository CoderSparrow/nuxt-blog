<template>
  <el-card
    shadow="hover"
    class="post"
  >
    <header slot="header" class="post__header">
      <h3>Post Title</h3>
      <small>
        <i class="el-icon-time"></i>
        {{ currentDate }}
      </small>
    </header>

    <section class="post__body">
      <img src="@/assets/img/animal.png" alt="post image" class="post__img">
    </section>

    <footer class="post__footer">
      <el-button round @click="openPost">Открыть</el-button>
      <span class="post__count-comment">
        <i class="el-icon-message"></i>
        12
      </span>
    </footer>
  </el-card>
</template>

<script>
export default {
  name: "PostPreview",
  computed: {
    currentDate () {
      return new Date().toLocaleString()
    }
  },
  methods: {
    openPost () {
      this.$router.push('/post/1')
    }
  }
}
</script>

<style lang="scss" scoped>
.post {
  margin: 10px;

  &__header {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  &__img {
    width: 100%;
  }

  &__footer {
    margin-top: 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
}
</style>
