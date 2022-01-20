<template>
  <div class="home">
    <z_header :unitid="unitid" />
    <el-container :direction="horizontal">
      <div class="container_body">
        <el-aside width="276px">
          <main-left />
        </el-aside>
        <el-main height="100%"><main-right /></el-main>
      </div>
    </el-container>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";
import z_header from '@/components/header.vue'
import MainLeft from '@/components/main_left.vue'
import MainRight from '@/components/main_right.vue'

export default {
  name: 'Home',
  components: {
    // HelloWorld,
    z_header,
    MainLeft,
    MainRight
  },
  data() {
    return {
      unitid: 6,
      horizontal: 'horizontal'
    }
  }
}
</script>

<style>
.home {
  background: url('../assets/xxgkbodybg.jpg') center 0 no-repeat #fff !important;
}
.el-container {
  width: 1100px;
  margin: 0 auto;
}
.container_body {
  background-color: rgb(242, 242, 242);
  display: flex;
  flex-wrap: wrap;
}
.el-aside {
  background-color: rgb(242, 242, 242);
}
.el-main {
  background-color: rgb(242, 242, 242);
  width: 824px;
  padding-left: 0;
}
</style>
