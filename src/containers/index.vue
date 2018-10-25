<template>
  <el-container class='container'>
    <!-- header -->
    <el-header>
      <i-header />
    </el-header>

    <!-- main -->
    <el-main>
      <i-main />
    </el-main>

  </el-container>
</template>

<script>
import iHeader from './header'
import iMain from './main'
export default {
  name: 'container',
  components: {
    iHeader,
    iMain
  }
}
</script>

<style scoped>
.el-header {
  border-bottom: 1px solid lightsteelblue;
  border-bottom-left-radius: 40px;
  border-bottom-right-radius: 40px;
}
</style>
