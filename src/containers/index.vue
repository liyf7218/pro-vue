<template>
  <el-container class='main-container'>
    <!-- header -->
    <el-header>
      <i-header />
    </el-header>

    <el-container class='sub-container'>
      <!-- aside -->
      <el-aside width="240px">
        <i-aside />
      </el-aside>

      <el-container class='context-container'>
        <!-- main -->
        <el-main>
          <i-main />
        </el-main>

        <!-- footer -->
        <el-footer>
          <i-footer />
        </el-footer>
      </el-container>

    </el-container>

  </el-container>
</template>

<script>
import iHeader from './header'
import iAside from './aside'
import iMain from './main'
import iFooter from './footer'
export default {
  name: 'container',
  components: {
    iHeader,
    iMain,
    iAside,
    iFooter
  }
}
</script>

<style scoped>
.main-container {
  overflow-y: hidden;
  height: 100%;
}

.el-header {
  /* 设置底部边框弧线 */
  border-bottom: 1px solid lightsteelblue;
  border-bottom-left-radius: 40px;
  border-bottom-right-radius: 40px;

  /* 固定在顶部 part 1/2 */
  position: fixed;
  height: 60px;
  width: 100%;
  left: 0;
  top: 0;
  display: block;
  z-index: 1500;
  background-color: white;
}

.sub-container {
  height: calc(100% - 80px);
  margin-top: 80px;
}

/*.sub-container .el-aside {
  width: 240px;
  position: fixed;
  top: 0;
  bottom: 0;
  margin-top: 80px;
  transition: padding-top .3s;
}*/

/*.context-container {
  padding-left: 270px;
  padding-bottom: 100px;
  box-sizing: border-box;
}*/

</style>
