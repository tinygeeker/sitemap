<template>
  <div>
    <h2>极客飞兔 网站导航 <sub><el-link href="https://tinygeeker.gitee.io/menu/sitemap/?from=https://tinygeeker.github.io/menu/sitemap/" target="_blank" type="primary">国内版>></el-link></sub></h2>
    <el-row type="flex" justify="center" align="middle">
      <el-card shadow="hover" style="width: 80%; border-radius: 4px">
        <el-collapse v-model="activeNames" accordion>
          <el-collapse-item name="1" align="left">
            <template #title>
              <el-icon><Operation /></el-icon> 常用网址
            </template>
            <div>
              <el-link :underline="false" style="font-weight:bold;">推荐：</el-link>
              <el-link href="http://www.xiaozhongai.top/?code=lMaCoXNBPv" target="_blank" type="danger">国内版ChatGPT</el-link>
              <el-link href="https://www.logosc.cn/?coupon=tinygeeker" target="_blank" type="danger">标小智Logo生成器</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">搜索：</el-link>
              <el-link href="https://www.baidu.com/" target="_blank" type="danger">百度一下</el-link>
              <el-link href="https://www.wuzhuiso.com/" target="_blank" type="danger">无追搜索</el-link>
              <el-link href="https://www.gobaidugle.com/" target="_blank" type="danger">联合搜索</el-link>
              <el-link href="https://www.google.com/" target="_blank" type="danger">谷歌搜索「墙」</el-link>
              <el-link href="https://www.bing.com/" target="_blank" type="primary">必应搜索</el-link>
              <el-link href="https://www.sogou.com/" target="_blank" type="primary">搜狗搜索</el-link>
              <el-link href="https://www.so.com/" target="_blank" type="primary">360搜索</el-link>
              <el-link href="https://www.soso.com/" target="_blank" type="primary">搜搜</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">热门：</el-link>
              <el-link href="https://s.weibo.com/top/summary" target="_blank" type="danger">微博热搜</el-link>
              <el-link href="https://www.toutiao.com/" target="_blank" type="danger">今日头条</el-link>
              <el-link href="https://www.bilibili.com/" target="_blank" type="danger">哔哩哔哩</el-link>
              <el-link href="https://www.douyin.com/" target="_blank" type="danger">抖音</el-link>
              <el-link href="https://www.douban.com/" target="_blank" type="primary">豆瓣</el-link>
              <el-link href="https://www.zhihu.com/" target="_blank" type="primary">知乎</el-link>
              <el-link href="https://www.jd.com/" target="_blank" type="primary">京东</el-link>
              <el-link href="https://www.taobao.com/" target="_blank" type="primary">淘宝</el-link>
              <el-link href="https://www.mafengwo.cn/" target="_blank" type="primary">马蜂窝</el-link>
              <el-link href="http://www.3hk.cn/" target="_blank" type="primary">香港自由行</el-link>
              <el-link href="https://www.pc6.com/" target="_blank" type="primary">PC6下载站</el-link>
            </div>
          </el-collapse-item>
          <el-collapse-item name="2" align="left">
            <template #title>
              <el-icon><Headset /></el-icon> 在线娱乐
            </template>
            <div>
              <el-link :underline="false" style="font-weight:bold;">音乐：</el-link>
              <el-link href="http://www.ihaoge.net/" target="_blank" type="danger">爱好歌音乐网</el-link>
              <el-link href="https://www.hifini.com/" target="_blank" type="danger">音乐磁场</el-link>
              <el-link href="https://tools.liumingye.cn/music/#/" target="_blank" type="danger">MyFreeMp3</el-link>
              <el-link href="http://qingyinyue.club/" target="_blank" type="danger">轻音乐俱乐部</el-link>
              <el-link href="https://music.ghxi.com/" target="_blank" type="danger">果核音乐</el-link>
              <el-link href="https://music.163.com/" target="_blank" type="danger">网易云音乐</el-link>
              <el-link href="https://y.qq.com/" target="_blank" type="danger">QQ音乐</el-link>
              <el-link href="https://www.kugou.com/" target="_blank" type="primary">酷狗音乐</el-link>
              <el-link href="http://www.kuwo.cn/" target="_blank" type="primary">酷我音乐</el-link>
              <el-link href="https://www.9ku.com/" target="_blank" type="primary">九酷音乐</el-link>
              <el-link href="https://music.91q.com/" target="_blank" type="primary">千千音乐</el-link>
              <el-link href="https://www.1ting.com/" target="_blank" type="primary">一听音乐</el-link>
              <el-link href="https://music.douban.com/" target="_blank" type="primary">豆瓣音乐</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">游戏：</el-link>
              <el-link href="https://www.668play.com/" target="_blank" type="danger">668游戏仓库</el-link>
              <el-link href="https://www.crazygames.com/" target="_blank" type="danger">CrazyGames</el-link>
              <el-link href="https://www.yikm.net/" target="_blank" type="danger">千米娱乐</el-link>
              <el-link href="http://www.4399.com/" target="_blank" type="danger">4399</el-link>
              <el-link href="https://cg.163.com/" target="_blank" type="primary">网易云游戏</el-link>
              <el-link href="https://cloudgame.douyu.com/" target="_blank" type="primary">斗鱼云游戏</el-link>
              <el-link href="https://yowa.huya.com/" target="_blank" type="primary">虎牙云游戏</el-link>
              <el-link href="https://www.migufun.com/" target="_blank" type="primary">咪咕云游戏</el-link>
              <el-link href="http://xiataya.top/nes/#/" target="_blank" type="primary">NES在线</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">追剧：</el-link>
              <el-link href="https://cupfox.app/" target="_blank" type="danger">茶杯狐</el-link>
              <el-link href="https://www.6080yy3.com/" target="_blank" type="danger">6080</el-link>
              <el-link href="https://www.hdmoli.com/" target="_blank" type="danger">HDmoli</el-link>
              <el-link href="https://www.qiuxia360.com/" target="_blank" type="danger">秋霞影视</el-link>
              <el-link href="https://www.333ys.tv/" target="_blank" type="danger">333影视</el-link>
              <el-link href="https://www.netfly.tv/" target="_blank" type="danger">奈飞中文影视</el-link>
              <el-link href="https://www.subaibaiys.com/" target="_blank" type="danger">素白白</el-link>
              <el-link href="https://tkznp.com/" target="_blank" type="danger">天空影视</el-link>
              <el-link href="https://www.zxzjhd.com/" target="_blank" type="danger">在线之家</el-link>
              <el-link href="https://www.cz4k.com/" target="_blank" type="danger">厂长资源</el-link>
              <el-link href="https://ddys.art/" target="_blank" type="danger">低端影视</el-link>
              <el-link href="https://55dy9.vip/" target="_blank" type="danger">555电影</el-link>
              <el-link href="https://www.mjw6.cc/" target="_blank" type="danger">美剧窝</el-link>
              <el-link href="https://www.mayiyahu.com/" target="_blank" type="primary">麻衣呼呀</el-link>
              <el-link href="https://www.dianyinggou.com/" target="_blank" type="primary">电影狗</el-link>
              <el-link href="https://www.zjtu.tv/" target="_blank" type="primary">追剧兔</el-link>
              <el-link href="https://www.freeok.vip/" target="_blank" type="primary">FreeOK</el-link>
              <el-link href="https://www.3wyy.com/" target="_blank" type="primary">爱看影院</el-link>
              <el-link href="https://dadagui.me/" target="_blank" type="primary">达达龟</el-link>
              <el-link href="https://www.pipiya.cc/" target="_blank" type="primary">皮皮鸭</el-link>
              <el-link href="https://www.dandanju.cc/" target="_blank" type="primary">蛋蛋剧</el-link>
              <el-link href="https://www.kkw361.com/" target="_blank" type="primary">看看屋</el-link>
              <el-link href="https://www.dm718.com/" target="_blank" type="primary">大米星球</el-link>
              <el-link href="https://zhaotaici.cn/" target="_blank" type="primary">找台词</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">动漫：</el-link>
              <el-link href="http://www.nicotv.biz/" target="_blank" type="danger">妮可动漫</el-link>
              <el-link href="https://www.bimiacg4.net/" target="_blank" type="danger">哔咪动漫</el-link>
              <el-link href="http://www.995dm.com/" target="_blank" type="danger">久久动漫</el-link>
              <el-link href="https://www.agedm.tv/" target="_blank" type="primary">AGE动漫</el-link>
              <el-link href="http://halihali1.com/" target="_blank" type="primary">哈里哈里</el-link>
              <el-link href="http://www.fengchedm.com/" target="_blank" type="primary">风车动漫</el-link>
              <el-link href="https://www.36dm.com/" target="_blank" type="primary">动漫下载</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">磁力：</el-link>
              <el-link href="https://cursor.vip/vip" target="_blank" type="danger">吃力网</el-link>
              <el-link href="https://bt1207dizhi.icu/" target="_blank" type="primary">BT1207</el-link>
              <el-link href="https://skrbtra.top/" target="_blank" type="primary">SKRBT</el-link>
              <el-link href="https://www.yuhuage.art/" target="_blank" type="primary">雨花阁</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">壁纸：</el-link>
              <el-link href="https://www.gamewallpapers.com/" target="_blank" type="danger">游戏CG图</el-link>
              <el-link href="https://bz.zzzmh.cn/" target="_blank" type="danger">极简壁纸</el-link>
              <el-link href="https://desk.zol.com.cn/" target="_blank" type="danger">中关村壁纸</el-link>
              <el-link href="https://bing.ioliu.cn/" target="_blank" type="danger">必应壁纸</el-link>
              <el-link href="https://www.dpm.org.cn/lights/royal.html" target="_blank" type="danger">故宫壁纸</el-link>
              <el-link href="https://wallhaven.cc/" target="_blank" type="danger">Wallhaven</el-link>
              <el-link href="https://alphacoders.com/" target="_blank" type="danger">Alpha Coders</el-link>
              <el-link href="https://wallpaperscraft.com/" target="_blank" type="danger">wallpaperscraft</el-link>
              <el-link href="https://www.10wallpaper.com/" target="_blank" type="danger">10wallpaper</el-link>
              <el-link href="https://wallpapershome.com/" target="_blank" type="danger">Wallpapershome</el-link>
              <el-link href="https://www.foodiesfeed.com/" target="_blank" type="primary">Foodiesfeed</el-link>
              <el-link href="https://www.wallpaperfusion.com/" target="_blank" type="primary">4K壁纸</el-link>
              <el-link href="https://10wallpaper.com/cn" target="_blank" type="primary">高清壁纸</el-link>
              <el-link href="https://wallroom.io" target="_blank" type="primary">插画风</el-link>
              <el-link href="https://gratisography.com/" target="_blank" type="primary">脑洞壁纸</el-link>
              <el-link href="http://www.facets.la" target="_blank" type="primary">矢量插画</el-link>
            </div> 
            <div>
              <el-link :underline="false" style="font-weight:bold;">资源：</el-link>
              <el-link href="https://www.niceso.fun" target="_blank" type="danger">奈斯</el-link>
              <el-link href="https://www.panpanr.com/" target="_blank" type="danger">阿里盘盘</el-link>
              <el-link href="https://pan666.cn/" target="_blank" type="primary">阿里小站</el-link>
              <el-link href="https://www.xuesousou.com/" target="_blank" type="primary">学搜搜</el-link>
              <el-link href="https://www.dalipan.com/" target="_blank" type="primary">大力盘</el-link>
              <el-link href="https://www.iizhi.cn/" target="_blank" type="primary">毕方铺</el-link>
              <el-link href="https://panother.com/" target="_blank" type="primary">盘他</el-link>
              <el-link href="https://feiyu100.cn/" target="_blank" type="primary">飞鱼盘搜</el-link>
              <el-link href="https://www.woxiangsou.com/" target="_blank" type="primary">口袋云盘</el-link>
              <el-link href="https://www.upyunso.com/" target="_blank" type="primary">UP云搜</el-link>
              <el-link href="https://www.tianyiso.com/" target="_blank" type="primary">天逸搜</el-link>
              <el-link href="https://ali.gitcafe.ink/" target="_blank" type="primary">小纸条</el-link>
              <el-link href="https://www.alipansou.com/" target="_blank" type="primary">喵狸盘搜</el-link>
              <el-link href="https://www.luomapan.com/" target="_blank" type="primary">罗马盘</el-link>
              <el-link href="https://www.chaonengso.com/" target="_blank" type="primary">超能搜</el-link>
              <el-link href="https://www.dalipan.com/" target="_blank" type="primary">大力盘</el-link>
              <el-link href="https://www.feifeipan.com/" target="_blank" type="primary">飞飞盘</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">直播：</el-link>
              <el-link href="https://tv.cctv.com/live/" target="_blank" type="danger">CCTV直播</el-link>
              <el-link href="http://iptv.xiner.store" target="_blank" type="danger">电视直播</el-link>
              <el-link href="http://www.zyz98.com/" target="_blank" type="primary">看全球</el-link>
              <el-link href="http://www.qm5.cc/" target="_blank" type="primary">球迷网</el-link>
              <el-link href="https://www.luxiangwu.com/nbaluxiang/" target="_blank" type="primary">NBA录像吧</el-link>
              <el-link href="http://www.qwzb.me/" target="_blank" type="primary">球王直播</el-link>
              <el-link href="http://www.qm5.cc/" target="_blank" type="primary">柠檬直播</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">学习：</el-link>
              <el-link href="https://rjzxw.com/" target="_blank" type="danger">软件自学网</el-link>
              <el-link href="https://www.51zxw.net/" target="_blank" type="danger">我要自学网</el-link>
              <el-link href="http://www.52zxw.com/" target="_blank" type="danger">我爱自学网</el-link>
              <el-link href="http://v.dxsbb.com/" target="_blank" type="danger">大学生自学网</el-link>
              <el-link href="https://www.ted.com/" target="_blank" type="danger">TED</el-link>
              <el-link href="https://www.smartedu.cn/" target="_blank" type="danger">国家智慧教育平台</el-link>
              <el-link href="https://www.icourses.cn/home/" target="_blank" type="primary">爱课程</el-link>
              <el-link href="http://open.sina.com.cn/" target="_blank" type="primary">新浪公开课</el-link>
              <el-link href="https://www.cmooc.com/" target="_blank" type="primary">MOOC中国</el-link>
              <el-link href="https://open.163.com/" target="_blank" type="primary">网易公开课</el-link>
              <el-link href="https://www.icourse163.org/" target="_blank" type="primary">中国大学MOOC</el-link>
              <el-link href="https://www.xuetangx.com/search" target="_blank" type="primary">学堂在线</el-link>
              <el-link href="https://www.nhk.or.jp/lesson/zh/" target="_blank" type="primary">简明日语</el-link>
            </div>
          </el-collapse-item>
          <el-collapse-item name="3" align="left">
            <template #title>
              <el-icon><Document /></el-icon> 在线考证
            </template>
            <div>
              <el-link :underline="false" style="font-weight:bold;">考公：</el-link>
              <el-link href="http://gongkao6688.edudisk.cn/" target="_blank" type="primary">教育网盘</el-link>
              <el-link href="http://qq351605872.ysepan.com/" target="_blank" type="primary">记忆力网盘</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">证书：</el-link>
              <el-link href="https://bkfeng.top/study" target="_blank" type="primary">四六级</el-link>
              <el-link href="http://axky.ysepan.com/" target="_blank" type="primary">四六级/考研</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">考研：</el-link>
              <el-link href="http://www.cskaoyan.com/" target="_blank" type="danger">王道论坛</el-link>
              <el-link href="http://bbs.bbs.kaoyan.com/" target="_blank" type="primary">考研论坛</el-link>
              <el-link href="http://www.chinakaoyan.com/club/" target="_blank" type="primary">中国考研网</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">官网：</el-link>
              <el-link href="https://www.chsi.com.cn/" target="_blank" type="danger">学信网</el-link>
              <el-link href="https://www.chinadegrees.cn/cqva/gateway.html" target="_blank" type="danger">学位网</el-link>
              <el-link href="http://www.scs.gov.cn/" target="_blank" type="danger">国家公务员局</el-link>
              <el-link href="https://ntce.neea.edu.cn/" target="_blank" type="primary">中国教育考试网</el-link>
              <el-link href="https://bm.ruankao.org.cn/sign/welcome" target="_blank" type="primary">软件考试网</el-link>
              <el-link href="http://exam.chinapmp.cn/" target="_blank" type="primary">项目管理职业资格认证（PMP）</el-link>
              <el-link href="http://www.cltt.org/" target="_blank" type="primary">全国普通话报名系统</el-link>
              <el-link href="https://passport.neea.edu.cn/CETLogin/" target="_blank" type="primary">四六级/GET</el-link>
              <el-link href="https://www.syt126.com/shouyi/baoming/" target="_blank" type="primary">兽易通/职业兽医</el-link>
              <el-link href="https://www.cfa.cn/" target="_blank" type="primary">中国CFA考试网</el-link>
            </div>
          </el-collapse-item>
          <el-collapse-item name="4" align="left">
            <template #title>
              <el-icon><Mouse /></el-icon> 效率工具
            </template>
            <div>
              <el-link :underline="false" style="font-weight:bold;">导航：</el-link>
              <el-link href="https://shadiao.app/" target="_blank" type="danger">沙雕导航</el-link>
              <el-link href="https://www.xue8nav.com/" target="_blank" type="danger">学吧导航</el-link>
              <el-link href="https://www.91sotu.com/" target="_blank" type="danger">搜图导航</el-link>
              <el-link href="https://ai-bot.cn/" target="_blank" type="danger">AI工具集</el-link>
              <el-link href="https://hao.uisdc.com/" target="_blank" type="danger">优设导航</el-link>
              <el-link href="http://hao.shejidaren.com/" target="_blank" type="danger">设计导航</el-link>
              <el-link href="https://tool.lu/" target="_blank" type="primary">程序员工具箱</el-link>
              <el-link href="https://www.iamwawa.cn/" target="_blank" type="primary">蛙蛙工具</el-link>
              <el-link href="https://xmrth.net/" target="_blank" type="primary">XMRth</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">效率：</el-link>
              <el-link href="https://tinypng.com/" target="_blank" type="danger">图片无损压缩</el-link>
              <el-link href="https://bigjpg.com/" target="_blank" type="danger">图片无损放大</el-link>
              <el-link href="http://www.yalijuda.com/" target="_blank" type="danger">图片视频压缩</el-link>
              <el-link href="https://www.zhihuilib.com/general/gifcompress" target="_blank" type="primary">GIF压缩</el-link>
              <el-link href="http://www.topdf.cn/" target="_blank" type="primary">TOPDF转换器</el-link>
              <el-link href="https://ps.gaoding.com/" target="_blank" type="primary">在线PS</el-link>
              <el-link href="https://www.apowersoft.cn/free-audio-recorder-online" target="_blank" type="primary">在线录音</el-link>
              <el-link href="https://www.greatdreams.com.cn/" target="_blank" type="primary">房贷计算器</el-link>
              <el-link href="https://sina.lt/" target="_blank" type="primary">新浪短链</el-link>
              <el-link href="https://cli.im/" target="_blank" type="primary">草料二维码</el-link>
              <el-link href="http://24mail.chacuo.net/" target="_blank" type="primary">临时邮箱</el-link>
              <el-link href="https://www.aoqiv.com/" target="_blank" type="primary">在线音频剪辑</el-link>
              <el-link href="https://www.kapwing.com/" target="_blank" type="primary">在线视频剪辑</el-link>
              <el-link href="https://suulnnka.github.io/BullshitGenerator/index.html" target="_blank" type="primary">文章生成器</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">识图：</el-link>
              <el-link href="https://gfsoso.soik.top/image.html" target="_blank" type="danger">谷歌识图</el-link>
              <el-link href="https://yandex.com/images" target="_blank" type="primary">yandex识图</el-link>
              <el-link href="https://cn.bing.com/visualsearch" target="_blank" type="primary">必应识图</el-link>
              <el-link href="https://pic.sogou.com/" target="_blank" type="primary">搜狗识图</el-link>
              <el-link href="https://trace.moe/" target="_blank" type="primary">识别动漫</el-link>
              <el-link href="https://image.baidu.com/" target="_blank" type="primary">百度识图</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">报告：</el-link>
              <el-link href="https://www.iresearch.com.cn/report.shtml" target="_blank" type="danger">艾瑞咨询</el-link>
              <el-link href="https://www.iimedia.cn/" target="_blank" type="danger">艾媒网</el-link>
              <el-link href="http://www.aliresearch.com/cn/index" target="_blank" type="primary">阿里研究院</el-link>
              <el-link href="https://c.wanfangdata.com.cn/nstr" target="_blank" type="primary">万方数据</el-link>
              <el-link href="http://www.767stock.com/" target="_blank" type="primary">乐晴智库</el-link>
              <el-link href="https://mtj.baidu.com/" target="_blank" type="primary">百度数据</el-link>
              <el-link href="https://www.chinaventure.com.cn/" target="_blank" type="primary">投中研究院</el-link>
              <el-link href="https://www.caasdata.com/" target="_blank" type="primary">卡思数据</el-link>
              <el-link href="http://data.stats.gov.cn/" target="_blank" type="primary">国家数据</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">模板：</el-link>
              <el-link href="http://www.hippter.com/" target="_blank" type="danger">Hippter</el-link>
              <el-link href="http://www.tretars.com/" target="_blank" type="danger">比格PPT</el-link>
              <el-link href="http://www.51pptmoban.com/" target="_blank" type="primary">51PPT</el-link>
              <el-link href="https://www.ypppt.com/" target="_blank" type="primary">优品PPT</el-link>
              <el-link href="https://www.1ppt.com/" target="_blank" type="primary">第一PPT</el-link>
              <el-link href="https://www.officeplus.cn/Template/Home.shtml" target="_blank" type="primary">微软官方PPT</el-link>
              <el-link href="https://slidemodel.com/" target="_blank" type="primary">SlideModel</el-link>
              <el-link href="https://www.woodo.cn/template" target="_blank" type="primary">吾道</el-link>
              <el-link href="https://www.docer.com/" target="_blank" type="primary">稻壳儿</el-link>
              <el-link href="http://www.yanj.cn/" target="_blank" type="primary">演界网</el-link>
              <el-link href="https://www.pptstore.net/" target="_blank" type="primary">PPTStore</el-link>
              <el-link href="https://hislide.io" target="_blank" type="primary">HISLIDE</el-link>
              <el-link href="https://www.presentationload.com/" target="_blank" type="primary">Presentationload</el-link>
              <el-link href="https://creativemarket.com/" target="_blank" type="primary">Creativemarket</el-link>
              <el-link href="https://graphicriver.net/" target="_blank" type="primary">Graphics</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">仓库：</el-link>
              <el-link href="https://github.com/" target="_blank" type="danger">Github</el-link>
              <el-link href="https://gitlab.com/" target="_blank" type="danger">Gitlab</el-link>
              <el-link href="https://gitee.com/enterprises?invite_code=Z2l0ZWUtMTc0NDMzOQ%3D%3D" target="_blank" type="danger">Gitee</el-link>
              <el-link href="https://github.welab.eu.org/" target="_blank" type="primary">Github加速器</el-link>
            </div>
          </el-collapse-item>
          <el-collapse-item name="5" align="left">
            <template #title>
              <el-icon><Guide /></el-icon> 冷门网站
            </template>
            <div>
             <el-link :underline="false" style="font-weight:bold;">推荐：</el-link>
              <el-link href="https://ym.today/" target="_blank" type="danger">羊毛日报</el-link>
            </div>
            <div>
             <el-link :underline="false" style="font-weight:bold;">表情：</el-link>
              <el-link href="http://pdan.com.cn/" target="_blank" type="danger">皮蛋表情</el-link>
              <el-link href="https://www.diydoutu.com/" target="_blank" type="danger">斗图</el-link>
              <el-link href="https://fabiaoqing.com/" target="_blank" type="primary">发表情</el-link>
              <el-link href="https://www.pkdoutu.com/" target="_blank" type="primary">斗图啦</el-link>
            </div>
            <div>
             <el-link :underline="false" style="font-weight:bold;">地图：</el-link>
              <el-link href="http://www.onegreen.net/" target="_blank" type="danger">地图窝</el-link>
              <el-link href="https://www.webmap.cn/main.do?method=index" target="_blank" type="primary">地理系统</el-link>
              <el-link href="http://www.chinageoss.cn/dsp/home/index.jsp" target="_blank" type="primary">国家数据观测平台</el-link>
              <el-link href="http://bzdt.ch.mnr.gov.cn/" target="_blank" type="primary">标准地图服务</el-link>
              <el-link href="https://www.ageeye.cn/" target="_blank" type="primary">中国古地图</el-link>
            </div>
            <div>
             <el-link :underline="false" style="font-weight:bold;">榜单：</el-link>
              <el-link href="https://www.newrank.cn/" target="_blank" type="danger">新榜排行</el-link>
              <el-link href="https://www.bilibili.com/v/popular/rank/all" target="_blank" type="primary">哔哩哔哩排行</el-link>
              <el-link href="https://www.qian-gua.com/rank/category/" target="_blank" type="primary">小红书榜单</el-link>
              <el-link href="http://rank.uuu9.com/" target="_blank" type="primary">电竞排行</el-link>
              <el-link href="https://www.qimai.cn/rank" target="_blank" type="primary">七麦数据</el-link>
              <el-link href="https://ys.endata.cn/BoxOffice/Movie" target="_blank" type="primary">艺恩娱数</el-link>
              <el-link href="https://piaofang.maoyan.com/dashboard" target="_blank" type="primary">猫眼票房</el-link>
              <el-link href="https://www.doseeing.com/" target="_blank" type="primary">斗鱼直播排行</el-link>
              <el-link href="https://www.doseeing.com/huya" target="_blank" type="primary">虎牙直播排行</el-link>
              <el-link href="http://www.tvtv.hk/archives/category/dianshiju" target="_blank" type="primary">收视率</el-link>
              <el-link href="https://www.chandashi.com/ranking/index.html" target="_blank" type="primary">蝉大师</el-link>
            </div>
          </el-collapse-item>
          <el-collapse-item name="6" align="left">
            <template #title>
              <el-icon><Download /></el-icon> 实用下载
            </template>
            <div>
             <el-link :underline="false" style="font-weight:bold;">推荐：</el-link>
              <el-link href="http://www.12z.cn/index.html" target="_blank" type="danger">免费小说网</el-link>
              <el-link href="http://www.dzkbw.com/" target="_blank" type="danger">电子课本</el-link>
              <el-link href="https://www.fx361.com/" target="_blank" type="danger">期刊杂志</el-link>
            </div>
            <div>
             <el-link :underline="false" style="font-weight:bold;">影视：</el-link>
              <el-link href="https://ppxzy.net/" target="_blank" type="danger">皮皮虾资源</el-link>
              <el-link href="https://www.dyg5.com/" target="_blank" type="danger">电影港网</el-link>
              <el-link href="https://www.rrdynb.com/index.html" target="_blank" type="primary">人人电影网</el-link>
              <el-link href="https://mp4fan.org/" target="_blank" type="primary">高清MP4</el-link>
              <el-link href="https://www.mp4us.com/" target="_blank" type="primary">MP4电影</el-link>
              <el-link href="https://www.hao6v.tv/" target="_blank" type="primary">6V电影网</el-link>
            </div>
            <div>
             <el-link :underline="false" style="font-weight:bold;">字幕：</el-link>
              <el-link href="https://zimuku.org/" target="_blank" type="danger">字幕库</el-link>
              <el-link href="https://subhd.tv/" target="_blank" type="primary">SubHD</el-link>
            </div>
            <div>
             <el-link :underline="false" style="font-weight:bold;">小说：</el-link>
              <el-link href="https://noveless.com/" target="_blank" type="danger">书荒部落</el-link>
              <el-link href="https://www.zei8.vip/" target="_blank" type="primary">贼吧网</el-link>
              <el-link href="https://zbook.eu.org/" target="_blank" type="primary">zbook</el-link>
            </div>
          </el-collapse-item>
        </el-collapse>
      </el-card>
    </el-row>
  </div>
</template>

<script>
export default {
  name: "SiteMap",
  data() {
    return {
      activeNames: ["1"]
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
.el-collapse-item__header {
  font-size: 15px !important;
  font-weight: bold !important;
}

.el-collapse {
  border-top: 0 !important;
}

.el-link__inner {
  margin: 1vh;
}

.el-icon {
  margin-right: 1vh;
}
</style>
