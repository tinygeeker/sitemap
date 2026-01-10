<template>
  <div class="app-container">
    <!-- 星空粒子效果 -->
    <div class="starfield" ref="starfield"></div>
    <!-- 光线特效 -->
    <div class="light-effects">
      <!-- 纵向光线 -->
      <div 
        class="light-ray" 
        v-for="i in 6" 
        :key="i" 
        :style="{ 
          animationDelay: `${i * 2 + Math.random() * 3}s`,
          left: `${i * 15 + Math.random() * 10}%`
        }"
      ></div>
      <div 
        class="light-ray light-ray-2" 
        v-for="i in 4" 
        :key="`2-${i}`" 
        :style="{ 
          animationDelay: `${i * 3 + Math.random() * 2 + 1}s`,
          left: `${i * 20 + Math.random() * 15}%`
        }"
      ></div>
      <!-- 横向光线 -->
      <div 
        class="light-ray light-ray-horizontal" 
        v-for="i in 4" 
        :key="`h-${i}`" 
        :style="{ 
          animationDelay: `${i * 4 + Math.random() * 2}s`,
          top: `${i * 20 + Math.random() * 10}%`
        }"
      ></div>
      <div 
        class="light-ray light-ray-horizontal light-ray-horizontal-2" 
        v-for="i in 3" 
        :key="`h2-${i}`" 
        :style="{ 
          animationDelay: `${i * 5 + Math.random() * 3 + 1.5}s`,
          top: `${i * 25 + Math.random() * 15}%`
        }"
      ></div>
    </div>
    
    <SiteMap />

    <div id="kefu">
      <el-popover width="220" placement="left-end" trigger="hover">
        <div class="tech-popover">
          <div class="popover-header">
            <el-icon class="header-icon"><User /></el-icon>
            <h4 class="popover-title">扫一扫联系飞兔小哥</h4>
          </div>
          <div class="popover-body">
            <div class="qr-code-container">
              <img src="../assets/wechat.jpg" class="qr-code-img" />
            </div>
          </div>
          <div class="popover-footer">
            <span class="footer-text">微信扫码，随时联系</span>
          </div>
        </div>
        <template #reference>
          <div class="icon-wrapper">
            <el-icon class="tech-icon">
              <User />
            </el-icon>
          </div>
        </template>
      </el-popover>
      <el-popover width="220" placement="left-end" trigger="hover">
        <div class="tech-popover">
          <div class="popover-header">
            <el-icon class="header-icon"><ChatDotRound /></el-icon>
            <h4 class="popover-title">扫一扫关注微信公众号</h4>
          </div>
          <div class="popover-body">
            <p class="popover-desc">编程自学 技能干货 考证提升</p>
            <div class="qr-code-container">
              <img src="../assets/gzh.jpg" class="qr-code-img" />
            </div>
          </div>
          <div class="popover-footer">
            <span class="footer-text">获取更多优质内容</span>
          </div>
        </div>
        <template #reference>
          <div class="icon-wrapper">
            <el-icon class="tech-icon">
              <ChatDotRound />
            </el-icon>
          </div>
        </template>
      </el-popover>
      <el-popover width="220" placement="left-end" trigger="hover">
        <div class="tech-popover">
          <div class="popover-header">
            <el-icon class="header-icon"><Link /></el-icon>
            <h4 class="popover-title">欢迎关注小哥主页</h4>
          </div>
          <div class="popover-body">
            <div class="link-list">
              <p class="popover-link">CSDN：<el-link href="https://tinygeeker.blog.csdn.net/" target="_blank" type="primary">点击访问➢</el-link></p>
              <p class="popover-link">掘金：<el-link href="https://juejin.cn/user/2467756640574845" target="_blank" type="primary">点击访问➢</el-link></p>
              <p class="popover-link">思否：<el-link href="https://segmentfault.com/u/tinygeeker" target="_blank" type="primary">点击访问➢</el-link></p>
              <p class="popover-link">51CTO：<el-link href="https://blog.51cto.com/tinygeeker" target="_blank" type="primary">点击访问➢</el-link></p>
              <p class="popover-link">阿里云：<el-link href="https://developer.aliyun.com/profile/expert/oirrcfhlzqzko" target="_blank" type="primary">点击访问➢</el-link></p>
              <p class="popover-link">腾讯云：<el-link href="https://cloud.tencent.com/developer/user/8345747" target="_blank" type="primary">点击访问➢</el-link></p>
              <p class="popover-link">华为云：<el-link href="https://bbs.huaweicloud.com/community/usersnew/id_1677736481816497" target="_blank" type="primary">点击访问➢</el-link></p>
              <p class="popover-link">InfoQ：<el-link href="https://www.infoq.cn/u/tinygeeker/" target="_blank" type="primary">点击访问➢</el-link></p>
              <p class="popover-link">博客园：<el-link href="https://www.cnblogs.com/tinygeeker/" target="_blank" type="primary">点击访问➢</el-link></p>
            </div>
          </div>
          <div class="popover-footer">
            <span class="footer-text">多平台同步更新</span>
          </div>
        </div>
        <template #reference>
          <div class="icon-wrapper">
            <el-icon class="tech-icon">
              <Link />
            </el-icon>
          </div>
        </template>
      </el-popover>
      <!-- 打赏按钮 -->
      <el-popover width="220" placement="left-end" trigger="hover">
        <div class="tech-popover">
          <div class="popover-header">
            <el-icon class="header-icon"><Coin /></el-icon>
            <h4 class="popover-title">支持小哥创作</h4>
          </div>
          <div class="popover-body">
            <p class="popover-desc">如果觉得有用，欢迎打赏支持</p>
            <div class="donate-container">
              <img src="../assets/donate.jpg" class="donate-img" />
            </div>
          </div>
          <div class="popover-footer">
            <span class="footer-text">感谢您的支持与鼓励</span>
          </div>
        </div>
        <template #reference>
          <div class="icon-wrapper">
            <el-icon class="tech-icon">
              <Coin />
            </el-icon>
          </div>
        </template>
      </el-popover>
    </div>
  </div>
</template>

<script>
import SiteMap from './components/SiteMap.vue'

export default {
  name: 'App',
  components: {
    SiteMap
  },
  mounted() {
    // 初始化星空粒子效果
    this.initStarfield()
  },
  methods: {
    initStarfield() {
      const starfield = this.$refs.starfield
      if (!starfield) return

      // 创建100个星星
      for (let i = 0; i < 100; i++) {
        const star = document.createElement('div')
        
        // 随机位置
        const x = Math.random() * 100
        const y = Math.random() * 100
        
        // 随机大小和透明度（增大星星大小）
        const size = Math.random() * 5 + 2
        const opacity = Math.random() * 0.9 + 0.3
        
        // 随机颜色（蓝色、紫色、青色系）
        const colors = ['#4299e1', '#6366f1', '#34d399', '#3498db', '#8b5cf6', '#06b6d4']
        const color = colors[Math.floor(Math.random() * colors.length)]
        
        // 设置星星样式
        star.style.position = 'absolute'
        star.style.left = `${x}%`
        star.style.top = `${y}%`
        star.style.width = `${size}px`
        star.style.height = `${size}px`
        star.style.backgroundColor = color
        star.style.borderRadius = '50%'
        star.style.opacity = opacity
        star.style.boxShadow = `0 0 ${size * 3}px ${color}`
        star.style.animation = `twinkle ${Math.random() * 3 + 2}s infinite ease-in-out`
        star.style.animationDelay = `${Math.random() * 2}s`
        
        // 添加到星空容器
        starfield.appendChild(star)
      }
    }
  }
}
</script>

<style>
/* 重置所有元素的默认样式 */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* 重置body样式，消除默认边距和背景 */
body {
  margin: 0;
  padding: 0;
  background: linear-gradient(135deg, #0f172a 0%, #1e293b 50%, #334155 100%);
  background-attachment: fixed;
  overflow-x: hidden;
}

/* 主容器样式 */
.app-container {
  min-height: 100vh;
  background: linear-gradient(135deg, #0f172a 0%, #1e293b 50%, #334155 100%);
  background-attachment: fixed;
  position: relative;
  overflow: hidden;
  padding: 0;
  margin: 0;
}

/* 星空粒子效果容器 */
.starfield {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  z-index: 0;
}

/* 流星雨容器 */
.meteor-shower {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  z-index: 0;
  overflow: hidden;
}

/* 光线特效容器 */
.light-effects {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  z-index: 0;
  overflow: hidden;
}

/* 光线样式 */
.light-ray {
  position: absolute;
  width: 2px;
  height: 100%;
  background: linear-gradient(to bottom, transparent, rgba(66, 153, 225, 0.3), transparent);
  animation: lightRay 8s ease-in-out infinite;
  opacity: 0;
  top: -10%;
}

/* 第二种光线样式 */
.light-ray-2 {
  background: linear-gradient(to bottom, transparent, rgba(139, 92, 246, 0.3), transparent);
  animation: lightRay2 10s ease-in-out infinite;
}

/* 光线动画 */
@keyframes lightRay {
  0% {
    opacity: 0;
    transform: scaleY(0);
  }
  20% {
    opacity: 1;
    transform: scaleY(1);
  }
  80% {
    opacity: 1;
    transform: scaleY(1);
  }
  100% {
    opacity: 0;
    transform: scaleY(0);
  }
}

/* 第二种光线动画 */
@keyframes lightRay2 {
  0% {
    opacity: 0;
    transform: scaleY(0);
  }
  15% {
    opacity: 1;
    transform: scaleY(1);
  }
  85% {
    opacity: 1;
    transform: scaleY(1);
  }
  100% {
    opacity: 0;
    transform: scaleY(0);
  }
}

/* 横向光线样式 */
.light-ray-horizontal {
  width: 100%;
  height: 2px;
  background: linear-gradient(to right, transparent, rgba(34, 211, 238, 0.3), transparent);
  animation: lightRayHorizontal 10s ease-in-out infinite;
  top: 50%;
  left: -10%;
}

/* 第二种横向光线样式 */
.light-ray-horizontal-2 {
  background: linear-gradient(to right, transparent, rgba(66, 153, 225, 0.3), transparent);
  animation: lightRayHorizontal2 12s ease-in-out infinite;
}

/* 横向光线动画 */
@keyframes lightRayHorizontal {
  0% {
    opacity: 0;
    transform: scaleX(0);
  }
  20% {
    opacity: 1;
    transform: scaleX(1);
  }
  80% {
    opacity: 1;
    transform: scaleX(1);
  }
  100% {
    opacity: 0;
    transform: scaleX(0);
  }
}

/* 第二种横向光线动画 */
@keyframes lightRayHorizontal2 {
  0% {
    opacity: 0;
    transform: scaleX(0);
  }
  15% {
    opacity: 1;
    transform: scaleX(1);
  }
  85% {
    opacity: 1;
    transform: scaleX(1);
  }
  100% {
    opacity: 0;
    transform: scaleX(0);
  }
}

/* 科技感背景光效 */
.app-container::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: 
    radial-gradient(circle at 20% 30%, rgba(66, 153, 225, 0.15) 0%, transparent 50%),
    radial-gradient(circle at 80% 70%, rgba(139, 92, 246, 0.15) 0%, transparent 50%),
    radial-gradient(circle at 50% 50%, rgba(34, 211, 238, 0.1) 0%, transparent 70%);
  pointer-events: none;
  z-index: 0;
}

/* 彩色光线特效 */
.app-container::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: 
    linear-gradient(45deg, transparent 0%, rgba(66, 153, 225, 0.1) 25%, transparent 50%, rgba(139, 92, 246, 0.1) 75%, transparent 100%),
    linear-gradient(-45deg, transparent 0%, rgba(34, 211, 238, 0.1) 25%, transparent 50%, rgba(66, 153, 225, 0.1) 75%, transparent 100%);
  background-size: 200% 200%;
  animation: lightShift 15s ease infinite;
  pointer-events: none;
  z-index: 0;
}

/* 光线移动动画 */
@keyframes lightShift {
  0% {
    background-position: 0% 0%;
  }
  50% {
    background-position: 100% 100%;
  }
  100% {
    background-position: 0% 0%;
  }
}

/* 星星闪烁动画 */
@keyframes twinkle {
  0%, 100% {
    opacity: 0.2;
    transform: scale(1);
  }
  50% {
    opacity: 0.8;
    transform: scale(1.2);
  }
}

/* 确保#app元素继承主容器样式 */
#app {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #e2e8f0;
  position: relative;
  z-index: 1;
  margin: 0;
  padding: 0;
  min-height: 100vh;
}

/* 科技感悬浮窗口样式 */
.tech-popover {
  background: rgba(15, 23, 42, 0.95);
  border-radius: 10px;
  padding: 0;
  border: 1px solid rgba(66, 153, 225, 0.3);
  box-shadow: 
    0 5px 15px rgba(0, 0, 0, 0.3),
    0 0 20px rgba(66, 153, 225, 0.2);
  overflow: hidden;
  backdrop-filter: blur(10px);
}

/* 悬浮窗口头部 */
.popover-header {
  display: flex;
  align-items: center;
  padding: 15px;
  background: linear-gradient(135deg, rgba(66, 153, 225, 0.1), rgba(88, 28, 135, 0.1));
  border-bottom: 1px solid rgba(66, 153, 225, 0.2);
}

/* 头部图标 */
.header-icon {
  color: #4299e1;
  margin-right: 10px;
  font-size: 18px;
}

/* 悬浮窗口标题 */
.popover-title {
  color: #4299e1;
  margin: 0;
  font-size: 14px;
  font-weight: bold;
  flex: 1;
}

/* 悬浮窗口主体 */
.popover-body {
  padding: 15px;
}

/* 描述文本 */
.popover-desc {
  color: #94a3b8;
  margin-bottom: 15px;
  font-size: 12px;
  text-align: center;
}

/* 二维码容器 */
.qr-code-container {
  width: 100%;
  height: 180px;
  display: flex;
  align-items: center;
  justify-content: center;
  background: rgba(255, 255, 255, 0.05);
  border-radius: 6px;
  padding: 10px;
  margin: 0 auto;
}

/* 二维码图片 */
.qr-code-img {
  width: 160px;
  height: 160px;
  object-fit: cover;
  border-radius: 4px;
  border: 1px solid rgba(66, 153, 225, 0.2);
}

/* 打赏图片容器 */
.donate-container {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  background: rgba(255, 255, 255, 0.05);
  border-radius: 6px;
  padding: 10px;
  margin: 0 auto;
}

/* 打赏图片 */
.donate-img {
  max-width: 100%;
  max-height: 200px;
  object-fit: contain;
  border-radius: 4px;
  border: 1px solid rgba(66, 153, 225, 0.2);
}

/* 链接列表 */
.link-list {
  background: rgba(255, 255, 255, 0.03);
  border-radius: 6px;
  padding: 10px;
}



/* 链接样式 */
.popover-link {
  margin: 6px 0;
  font-size: 13px;
  text-align: left;
  color: #cbd5e1;
  transition: all 0.3s ease;
  padding: 6px 10px;
  border-radius: 4px;
  background: rgba(66, 153, 225, 0.05);
  border-left: 2px solid transparent;
}

/* 链接悬停效果 */
.popover-link:hover {
  color: #4299e1;
  transform: translateX(5px);
  background: rgba(66, 153, 225, 0.1);
  border-left: 2px solid rgba(66, 153, 225, 0.8);
  box-shadow: 0 2px 4px rgba(66, 153, 225, 0.2);
}

/* 平台名称样式 */
.popover-link::before {
  content: '';
  display: inline-block;
  width: 6px;
  height: 6px;
  background: #4299e1;
  border-radius: 50%;
  margin-right: 8px;
  animation: pulse 2s infinite ease-in-out;
}

/* 平台名称样式 */
.popover-link span:first-child {
  font-weight: bold;
  color: #94a3b8;
  margin-right: 5px;
}

/* 链接文本样式 */
.popover-link .el-link {
  font-size: 12px;
  transition: all 0.3s ease;
}

/* 链接文本悬停效果 */
.popover-link .el-link:hover {
  color: #60a5fa !important;
}

/* 悬浮窗口底部 */
.popover-footer {
  padding: 10px 15px;
  background: linear-gradient(135deg, rgba(66, 153, 225, 0.1), rgba(88, 28, 135, 0.1));
  border-top: 1px solid rgba(66, 153, 225, 0.2);
  text-align: center;
}

/* 底部文本 */
.footer-text {
  color: #94a3b8;
  font-size: 11px;
  font-style: italic;
}

.icon-wrapper {
  position: relative;
  margin: 10px 0;
}

.tech-icon {
  width: 45px;
  height: 45px;
  color: #4299e1;
  background: rgba(66, 153, 225, 0.1);
  border: 1px solid rgba(66, 153, 225, 0.3);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  transition: all 0.3s ease;
  position: relative;
  overflow: hidden;
}

.tech-icon:hover {
  background: rgba(66, 153, 225, 0.2);
  transform: translateY(-2px);
  box-shadow: 0 0 15px rgba(66, 153, 225, 0.4);
}

.tech-icon::before {
  content: '';
  position: absolute;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  background: linear-gradient(
    to bottom right,
    transparent,
    rgba(66, 153, 225, 0.2),
    transparent
  );
  transform: rotate(45deg);
  animation: shine 3s infinite;
}

@keyframes shine {
  0% {
    transform: translateX(-100%) rotate(45deg);
  }
  100% {
    transform: translateX(100%) rotate(45deg);
  }
}

#kefu {
  position: fixed;
  right: 20px;
  bottom: 50%;
  transform: translateY(50%);
  z-index: 999;
  display: flex;
  flex-direction: column;
  align-items: center;
  background: rgba(15, 23, 42, 0.8);
  padding: 10px;
  border-radius: 10px;
  backdrop-filter: blur(10px);
  border: 1px solid rgba(66, 153, 225, 0.3);
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
}
</style>
