<template>
  <el-card
    shadow="hover"
    class="post"
  >
    <header slot="header" class="post__header">
      <el-button round @click="back">
        <i class="el-icon-back"></i>
      </el-button>
      <h3>Post Title</h3>
      <small>
        <i class="el-icon-time"></i>
        {{ currentDate }}
      </small>
    </header>

    <section class="post__body">
      <img src="@/assets/img/animal.png" alt="post image" class="post__img">
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Animi assumenda consectetur consequatur dolores ea nam nemo nobis optio, quasi temporibus.</p>
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Animi assumenda consectetur consequatur dolores ea nam nemo nobis optio, quasi temporibus.</p>
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Animi assumenda consectetur consequatur dolores ea nam nemo nobis optio, quasi temporibus.</p>
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Animi assumenda consectetur consequatur dolores ea nam nemo nobis optio, quasi temporibus.</p>
    </section>

    <footer class="post__footer">

      <span class="post__count-comment">
        <i class="el-icon-message"></i>
        12
      </span>
    </footer>
  </el-card>
</template>

<script>
export default {
  name: "Post",
  computed: {
    currentDate () {
      return new Date().toLocaleString()
    }
  },
  methods: {
    back () {
      this.$router.back()
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
      width: 400px;
    }

    &__footer {
      margin-top: 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
  }
</style>
