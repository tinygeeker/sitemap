<template>
  <div>
    <h2>极客飞兔 网站导航</h2>
    <el-row type="flex" justify="center" align="middle">
      <el-card shadow="hover" style="width: 80%; border-radius: 4px">
        <el-collapse v-model="activeNames" accordion>
          <el-collapse-item name="1" align="left">
            <template #title>
              <el-icon><Operation /></el-icon> 常用网址
            </template>
            <div>
              <el-link :underline="false" style="font-weight:bold;">搜索：</el-link>
              <el-link href="https://www.baidu.com/" target="_blank" type="danger">百度一下</el-link>
              <el-link href="https://www.google.com/" target="_blank" type="danger">谷歌搜索</el-link>
              <el-link href="https://www.bing.com/" target="_blank" type="primary">必应搜索</el-link>
              <el-link href="https://www.sogou.com/" target="_blank" type="primary">搜狗搜索</el-link>
              <el-link href="https://www.so.com/" target="_blank" type="primary">360搜索</el-link>
              <el-link href="http://www.soso.com/" target="_blank" type="primary">搜搜</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">热门：</el-link>
              <el-link href="https://www.bilibili.com/" target="_blank" type="danger">哔哩哔哩</el-link>
              <el-link href="https://s.weibo.com/top/summary" target="_blank" type="danger">微博热搜</el-link>
              <el-link href="https://www.douyin.com/" target="_blank" type="danger">抖音</el-link>
              <el-link href="https://www.douban.com/" target="_blank" type="primary">豆瓣</el-link>
              <el-link href="https://www.zhihu.com/" target="_blank" type="primary">知乎</el-link>
              <el-link href="https://www.toutiao.com/" target="_blank" type="primary">今日头条</el-link>
              <el-link href="https://www.jd.com/" target="_blank" type="primary">京东</el-link>
              <el-link href="https://www.taobao.com/" target="_blank" type="primary">淘宝</el-link>
              <el-link href="http://www.mafengwo.cn/" target="_blank" type="primary">马蜂窝</el-link>
              <el-link href="http://www.3hk.cn/" target="_blank" type="primary">香港自由行</el-link>
              <el-link href="http://www.pc6.com/" target="_blank" type="primary">PC6下载站</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">社区：</el-link>
              <el-link href="https://juejin.cn/" target="_blank" type="danger">掘金</el-link>
              <el-link href="https://blog.csdn.net/" target="_blank" type="danger">CSDN</el-link>
              <el-link href="https://www.cnblogs.com/" target="_blank" type="danger">博客园</el-link>
              <el-link href="https://blog.51cto.com/" target="_blank" type="primary">51CTO</el-link>
              <el-link href="https://developer.aliyun.com/" target="_blank" type="primary">阿里云社区</el-link>
              <el-link href="https://bbs.huaweicloud.com/" target="_blank" type="primary">华为云社区</el-link>
              <el-link href="https://cloud.tencent.com/developer" target="_blank" type="primary">腾讯云社区</el-link>
              <el-link href="https://xie.infoq.cn/" target="_blank" type="primary">InfoQ</el-link>
              <el-link href="https://segmentfault.com/" target="_blank" type="primary">思否</el-link>
              <el-link href="https://www.oschina.net/" target="_blank" type="primary">开源中国</el-link>
              <el-link href="http://blog.chinaunix.net/" target="_blank" type="primary">ChinaUnix</el-link>
              <el-link href="https://developer.huawei.com/consumer/cn/forum/" target="_blank" type="primary">华为开发者论坛</el-link>
            </div>
          </el-collapse-item>
          <el-collapse-item name="2" align="left">
            <template #title>
              <el-icon><Headset /></el-icon> 在线娱乐
            </template>
            <div>
              <el-link :underline="false" style="font-weight:bold;">音乐：</el-link>
              <el-link href="https://music.163.com/" target="_blank" type="danger">网易云音乐</el-link>
              <el-link href="https://y.qq.com/" target="_blank" type="danger">QQ音乐</el-link>
              <el-link href="https://www.kugou.com/" target="_blank" type="primary">酷狗音乐</el-link>
              <el-link href="http://www.kuwo.cn/" target="_blank" type="primary">酷我音乐</el-link>
              <el-link href="https://www.9ku.com/" target="_blank" type="primary">九酷音乐</el-link>
              <el-link href="https://music.91q.com/" target="_blank" type="primary">千千音乐</el-link>
              <el-link href="https://www.1ting.com/" target="_blank" type="primary">一听音乐</el-link>
              <el-link href="https://music.douban.com/" target="_blank" type="primary">豆瓣音乐</el-link>
              <el-link href="https://www.hifini.com/" target="_blank" type="primary">音乐磁场</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">磁力：</el-link>
              <el-link href="https://cursor.vip/vip" target="_blank" type="danger">吃力网</el-link>
              <el-link href="https://bt1207dizhi.icu/" target="_blank" type="primary">BT1207</el-link>
              <el-link href="https://skrbtra.top/" target="_blank" type="primary">SKRBT</el-link>
              <el-link href="http://www.be52.xyz/" target="_blank" type="primary">磁力湾</el-link>
              <el-link href="https://www.yuhuage.art/" target="_blank" type="primary">雨花阁</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">游戏：</el-link>
              <el-link href="http://www.4399.com/" target="_blank" type="danger">4399</el-link>
              <el-link href="https://www.yikm.net/" target="_blank" type="danger">千米娱乐</el-link>
              <el-link href="http://www.pc6.com/h5/soft_487_1.html" target="_blank" type="primary">网页游戏</el-link>
              <el-link href="https://cg.163.com/" target="_blank" type="primary">网易云游戏</el-link>
              <el-link href="https://cloudgame.douyu.com/" target="_blank" type="primary">斗鱼云游戏</el-link>
              <el-link href="https://yowa.huya.com/" target="_blank" type="primary">虎牙云游戏</el-link>
              <el-link href="https://www.migufun.com/" target="_blank" type="primary">咪咕云游戏</el-link>
              <el-link href="http://xiataya.top/nes/#/" target="_blank" type="primary">NES在线</el-link>
              <el-link href="https://bbs.3dmgame.com/" target="_blank" type="primary">游戏下载</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">追剧：</el-link>
              <el-link href="https://www.xdwdn.com/" target="_blank" type="danger">剧知晓</el-link>
              <el-link href="https://cupfox.app/" target="_blank" type="danger">茶杯狐</el-link>
              <el-link href="https://www.dianyinggou.com/" target="_blank" type="danger">电影狗</el-link>
              <el-link href="https://www.rrdynb.com/" target="_blank" type="primary">人人电影网</el-link>
              <el-link href="https://7080.wang/" target="_blank" type="primary">影视搜</el-link>
              <el-link href="https://www.jiujiukanpian.com/" target="_blank" type="primary">久久影视</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">动漫：</el-link>
              <el-link href="http://www.nicotv.biz/" target="_blank" type="danger">妮可动漫</el-link>
              <el-link href="https://www.agemys.com/" target="_blank" type="primary">Age动漫</el-link>
              <el-link href="http://halihali1.com/" target="_blank" type="primary">哈里哈里</el-link>
              <el-link href="http://www.fengchedm.com/" target="_blank" type="primary">风车动漫</el-link>
              <el-link href="https://www.soman.com/" target="_blank" type="primary">搜漫</el-link>
              <el-link href="http://www.995dm.com/" target="_blank" type="primary">久久动漫</el-link>
              <el-link href="https://www.36dm.com/" target="_blank" type="primary">动漫下载</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">直播：</el-link>
              <el-link href="http://iptv.xiner.store" target="_blank" type="danger">电视直播</el-link>
              <el-link href="http://www.zyz98.com/" target="_blank" type="primary">看全球</el-link>
              <el-link href="http://www.qm5.cc/" target="_blank" type="primary">球迷网</el-link>
            </div> 
            <div>
              <el-link :underline="false" style="font-weight:bold;">壁纸：</el-link>
              <el-link href="https://www.gamewallpapers.com/" target="_blank" type="danger">游戏CG图</el-link>
              <el-link href="https://desk.zol.com.cn/" target="_blank" type="danger">中关村壁纸</el-link>
              <el-link href="https://bing.ioliu.cn/" target="_blank" type="primary">必应壁纸</el-link>
              <el-link href="https://bz.zzzmh.cn/" target="_blank" type="primary">极简壁纸</el-link>
              <el-link href="https://wallroom.io" target="_blank" type="primary">插画风</el-link>
              <el-link href="https://gratisography.com/" target="_blank" type="primary">脑洞壁纸</el-link>
              <el-link href="https://www.wallpaperfusion.com/" target="_blank" type="primary">4K壁纸</el-link>
              <el-link href="http://www.facets.la" target="_blank" type="primary">矢量插画</el-link>
              <el-link href="https://10wallpaper.com/cn" target="_blank" type="primary">高清壁纸</el-link>
            </div> 
            <div>
              <el-link :underline="false" style="font-weight:bold;">资源：</el-link>
              <el-link href="https://www.niceso.fun" target="_blank" type="danger">奈斯</el-link>
              <el-link href="https://www.panpanr.com/" target="_blank" type="danger">阿里盘盘</el-link>
              <el-link href="https://pan666.cn/" target="_blank" type="primary">阿里小站</el-link>
              <el-link href="https://www.panjd.com/" target="_blank" type="primary">盘基地</el-link>
              <el-link href="https://www.xuesousou.com/" target="_blank" type="primary">学搜搜</el-link>
              <el-link href="https://www.dalipan.com/" target="_blank" type="primary">大力盘</el-link>
              <el-link href="https://www.iizhi.cn/" target="_blank" type="primary">毕方铺</el-link>
              <el-link href="https://panother.com/" target="_blank" type="primary">盘他</el-link>
              <el-link href="https://feiyu100.cn/" target="_blank" type="primary">飞鱼盘搜</el-link>
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
              <el-link :underline="false" style="font-weight:bold;">以图搜图：</el-link>
              <el-link href="https://gfsoso.soik.top/image.html" target="_blank" type="danger">谷歌识图</el-link>
              <el-link href="https://yandex.com/images" target="_blank" type="primary">yandex识图</el-link>
              <el-link href="https://cn.bing.com/visualsearch" target="_blank" type="primary">必应识图</el-link>
              <el-link href="https://pic.sogou.com/" target="_blank" type="primary">搜狗识图</el-link>
              <el-link href="https://trace.moe/" target="_blank" type="primary">识别动漫</el-link>
              <el-link href="https://image.baidu.com/" target="_blank" type="primary">百度识图</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">行业报告：</el-link>
              <el-link href="https://www.iresearch.com.cn/report.shtml" target="_blank" type="danger">艾瑞咨询</el-link>
              <el-link href="https://www.iimedia.cn/" target="_blank" type="danger">艾媒网</el-link>
              <el-link href="http://www.aliresearch.com/cn/index" target="_blank" type="primary">阿里研究院</el-link>
              <el-link href="https://c.wanfangdata.com.cn/nstr" target="_blank" type="primary">万方数据</el-link>
              <el-link href="http://www.767stock.com/" target="_blank" type="primary">乐晴智库</el-link>
              <el-link href="https://mtj.baidu.com/" target="_blank" type="primary">百度数据</el-link>
              <el-link href="https://www.chinaventure.com.cn/" target="_blank" type="primary">投中研究院</el-link>
              <el-link href="https://www.caasdata.com/" target="_blank" type="primary">卡思数据</el-link>
              <el-link href="https://data.stats.gov.cn/" target="_blank" type="primary">国家数据</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">PPT模板：</el-link>
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
              <el-link :underline="false" style="font-weight:bold;">工作高效：</el-link>
              <el-link href="https://shadiao.app/" target="_blank" type="danger">沙雕导航</el-link>
              <el-link href="https://sina.lt/" target="_blank" type="danger">新浪短链</el-link>
              <el-link href="https://cli.im/" target="_blank" type="danger">草料二维码</el-link>
              <el-link href="http://24mail.chacuo.net/" target="_blank" type="primary">临时邮箱</el-link>
              <el-link href="https://ps.gaoding.com/" target="_blank" type="primary">在线PS</el-link>
              <el-link href="https://www.aoqiv.com/" target="_blank" type="primary">在线音频剪辑</el-link>
              <el-link href="https://www.kapwing.com/" target="_blank" type="primary">在线视频剪辑</el-link>
              <el-link href="https://tool.lu/" target="_blank" type="primary">程序员工具箱</el-link>
              <el-link href="https://www.iamwawa.cn/" target="_blank" type="primary">蛙蛙工具</el-link>
              <el-link href="https://suulnnka.github.io/BullshitGenerator/index.html" target="_blank" type="primary">文章生成器</el-link>
            </div>
          </el-collapse-item>
          <el-collapse-item name="5" align="left">
            <template #title>
              <el-icon><Guide /></el-icon> 冷门网站
            </template>
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
              <el-icon><Download /></el-icon> 软件下载
            </template>
            <div>
              <el-link :underline="false" style="font-weight:bold;">云盘：</el-link>
              <el-link href="https://pan.baidu.com/" target="_blank" type="danger">百度网盘</el-link>
              <el-link href="https://pan.quark.cn/" target="_blank" type="danger">夸克网盘</el-link>
              <el-link href="https://www.aliyundrive.com/" target="_blank" type="danger">阿里云盘</el-link>
              <el-link href="https://www.jianguoyun.com/" target="_blank" type="primary">坚果云盘</el-link>
              <el-link href="https://www.weiyun.com/" target="_blank" type="primary">腾讯微云</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">远程：</el-link>
              <el-link href="https://www.todesk.com/" target="_blank" type="danger">ToDesk</el-link>
              <el-link href="https://www.teamviewer.cn/cn/download/" target="_blank" type="danger">TeamViewer</el-link>
              <el-link href="https://sunlogin.oray.com/" target="_blank" type="danger">向日葵</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">媒体：</el-link>
              <el-link href="https://gifcam.en.softonic.com/" target="_blank" type="danger">录制Gif</el-link>
              <el-link href="http://www.pcfreetime.com/formatfactory/CN/index.html" target="_blank" type="primary">格式工厂</el-link>
              <el-link href="http://www.xfplay.com/" target="_blank" type="primary">影音先锋</el-link>
              <el-link href="http://www.qvevideo.com/ad/record" target="_blank" type="primary">电脑录音</el-link>
              <el-link href="https://www.apowersoft.cn/record-all-screen/" target="_blank" type="primary">傲软录屏</el-link>
              <el-link href="https://lv.ulikecam.com/" target="_blank" type="primary">剪映</el-link>
              <el-link href="https://www.douwan.video/index_ch.html" target="_blank" type="primary">都玩投屏</el-link>
            </div>
            <div>
              <el-link :underline="false" style="font-weight:bold;">安全：</el-link>
              <el-link href="http://www.360.cn/index.html" target="_blank" type="danger">360安全卫士</el-link>
              <el-link href="https://guanjia.qq.com/" target="_blank" type="primary">QQ电脑管家</el-link>
              <el-link href="https://yunsuo.qianxin.com/" target="_blank" type="primary">云锁</el-link>
              <el-link href="https://www.yunjiemi.net/pdf-password-recovery.html" target="_blank" type="primary">Pdf解密</el-link>
              <el-link href="http://www.coobar.com/" target="_blank" type="primary">网吧营销大师</el-link>
              <el-link href="https://www.duba.net/" target="_blank" type="primary">金山毒霸</el-link>
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
