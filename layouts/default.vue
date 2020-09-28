<template>
  <el-container class="is-vertical container">
    <AppHeader/>

    <el-main>
      <Nuxt/>
    </el-main>

    <AppFooter/>
  </el-container>
</template>

<script>
import AppHeader from "~/components/main/layout/AppHeader";
import AppFooter from "~/components/main/layout/AppFooter";

export default {
  components: {
    AppHeader,
    AppFooter
  }
}
</script>

<style lang="scss" scoped>
  .container {
    margin: 0 auto;
    width: 1200px;
  }
</style>
