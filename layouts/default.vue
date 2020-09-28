<template>
  <el-container class="is-vertical">
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

<style>

</style>
