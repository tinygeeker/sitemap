<template>
  <SiteMap />

  <div id="kefu">
    <el-popover width="200" placement="left-end" trigger="hover">
      <p style="text-align: center;"><b>扫一扫联系飞兔小哥</b></p>
      <img src="../assets/wechat.jpg" style="width: 200px;height: 100%;" />
      <template #reference>
        <el-icon>
          <User />
        </el-icon>
      </template>
    </el-popover>
    <el-popover width="200" placement="left-end" trigger="hover">
      <p style="text-align: center;"><b>扫一扫关注微信公众号</b></p>
      <p style="text-align: center;">编程自学 技能干货 考证提升</p>
      <img src="../assets/gzh.jpg" style="width: 200px;height: 100%;" />
      <template #reference>
        <el-icon>
          <ChatDotRound />
        </el-icon>
      </template>
    </el-popover>
    <el-popover width="200" placement="left-end" trigger="hover">
      <p style="text-align: center;"><b>欢迎关注小哥主页</b></p>
      <p style="text-align: center; margin: 0;padding: 0;">CSDN:<el-link href="https://tinygeeker.blog.csdn.net/" target="_blank" type="primary">点击访问➢</el-link></p>
      <p style="text-align: center; margin: 0;padding: 0;">掘金:<el-link href="https://juejin.cn/user/2467756640574845" target="_blank" type="primary">点击访问➢</el-link></p>
      <p style="text-align: center; margin: 0;padding: 0;">思否:<el-link href="https://segmentfault.com/u/tinygeeker" target="_blank" type="primary">点击访问➢</el-link></p>
      <p style="text-align: center; margin: 0;padding: 0;">51CTO:<el-link href="https://blog.51cto.com/tinygeeker" target="_blank" type="primary">点击访问➢</el-link></p>
      <p style="text-align: center; margin: 0;padding: 0;">阿里云:<el-link href="https://developer.aliyun.com/profile/expert/oirrcfhlzqzko" target="_blank" type="primary">点击访问➢</el-link></p>
      <p style="text-align: center; margin: 0;padding: 0;">腾讯云:<el-link href="https://cloud.tencent.com/developer/user/8345747" target="_blank" type="primary">点击访问➢</el-link></p>
      <p style="text-align: center; margin: 0;padding: 0;">华为云:<el-link href="https://bbs.huaweicloud.com/community/usersnew/id_1677736481816497" target="_blank" type="primary">点击访问➢</el-link></p>
      <p style="text-align: center; margin: 0;padding: 0;">InfoQ:<el-link href="https://www.infoq.cn/u/tinygeeker/" target="_blank" type="primary">点击访问➢</el-link></p>
      <p style="text-align: center; margin: 0;padding: 0;">博客园:<el-link href="https://www.cnblogs.com/tinygeeker/" target="_blank" type="primary">点击访问➢</el-link></p>
      <template #reference>
        <el-icon>
          <Link />
        </el-icon>
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
  bottom: 50%;
  z-index: 999;
  width: 60px;
  height: 60px;
}
</style>
