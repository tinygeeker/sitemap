<template>
  <SiteMap />

  <div id="kefu">
    <el-popover width="200" placement="left-end" trigger="hover">
      <p style="text-align: center;"><b>扫一扫联系飞兔小哥</b></p>
      <img src="../assets/wechat.jpg" style="width: 200px;height: 100%;" />
      <template #reference>
        <el-icon>
          <User />
        </el-icon> 常用网址
      </template>
    </el-popover>
    <el-popover width="200" placement="left-end" trigger="hover">
      <p style="text-align: center;"><b>扫一扫关注微信公众号</b></p>
      <p style="text-align: center;">编程自学 技能干货 考证提升</p>
      <img src="../assets/gzh.jpg" style="width: 200px;height: 100%;" />
      <template #reference>
        <el-icon>
          <ChatDotRound />
        </el-icon> 常用网址
      </template>
    </el-popover>
  </div>
</template>

<script>
import SiteMap from './components/SiteMap.vue'

export default {
  name: 'App',
  components: {
    SiteMap
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

#kefu .el-icon {
  width: 40px;
  height: 40px;
  color: #E65A65;
  border: 1px gray dashed;
  border-radius: 50%;
  margin: 0.3rem 0;
  cursor: pointer;
}

#kefu {
  position: fixed;
  right: 10px;
  bottom: 100px;
  z-index: 999;
  width: 60px;
  height: 60px;
}
</style>
