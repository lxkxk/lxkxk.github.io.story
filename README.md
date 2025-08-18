# lxkxk.github.io.story

- 音乐插件 - 胶囊播放器

1. 注掉 Meting.min.js 放开 Meting2.min.js
2. 放开 inject bottom 下边的这三个

- <script async data-pjax src="/js/anzhiyu.js"></script>
- <script async data-pjax src="/js/anzhiyufunction.js"></script>
- <script async src="/js/anzhiyuOnlyOne.js"></script>
  这三个是 胶囊播放器的依赖
  并注释
- <div class="aplayer no-destroy" data-id="14044452884" data-server="netease" data-type="playlist" data-fixed="true" data-autoplay="true"> </div>
  这个是原有样式

3. custom.css 中 搜索 胶囊播放器样式 start 把样式放开
4. 在 layout.pug 文件中把
   include ./music.pug
   这一行代码放开
5. hexo clean && hexo g && hexo s
   查看页面就可以了
6. 现在的胶囊音乐是随机播放用的 meting2.min.js 和菜单里的音乐界面用的同一个依赖，最好不要随便变
7. meting2.min.js
   备用地址 1：https://api.i-meto.com/meting/api?server=:server&type=:type&id=:id&r=:r
   备用地址 2：https://api.injahow.cn/meting/?server=:server&type=:type&id=:id&auth=:auth&r=:r"

8. 自我介绍备份之前的
<!-- ---
title: 关于
date: 2025-07-01 03:05:11
--- -->

<!-- {% note warning modern %}<b>正在玩命开发中~~~{% endnote %} -->

<!-- {% note warning modern %}<b>非商免字体、网图</b>等资源未经授权仅限个人使用，不得用于商业用途。本站平时仅用于交流和学习，如涉及侵权请联系站长删除对应资源，谢谢！ —— 致版权方{% endnote %} -->

<!-- ## 0.网站自述 🎬 -->

<!-- - 开发中~
- 本站由 hexo 搭建,使用 butterfly 主题
- 搭配 vue+elementUI 及各种第三方库组件成
- 包括用到了阿里的 icon 图标库及免费图床
- 还有国内 jsdelivr 免费 cdn 加速等
- 除了域名能白嫖的就不花钱
- 所以速度上可能会慢一些,会慢慢优化
- 一名熬夜型选手
- 但有时打游戏打到半夜就不太想写代码了
- 目前网站已完成 1/3,还在开发中~
- 想用小破站用来记录自己的生活
- 记录一些难忘的故事、音乐、摄影等
- 我靠,网站只能添加免费音乐,vip 不行
- 要记录的东西还有很多
- 网站的评论功能是我一直想做的
- 需要数据库和服务器以及一名后端
- 还在寻找和学习中
- 所以会持续更新！
- 对了 电脑网页版和手机版看到的效果是不一样的哦~ -->
  <!-- <div align=left class="aspect-ratio"> -->

   <!-- <iframe src=""
   scrolling="no"
   border="0"
   frameborder="no"
   framespacing="0"
   high_quality=1
   danmaku=1
   allowfullscreen="true">
   </iframe> -->

  <!--<div class="about_page">
    <div align=left class="aspect-ratio">
         <iframe src="https://player.bilibili.com/player.html?aid=474023258&&page=1&as_wide=1&high_quality=1&danmaku=0"
        scrolling="no"
        border="0"
        frameborder="no"
        framespacing="0"
        high_quality=1
        danmaku=1
        allowfullscreen="true">
        </iframe>


    </div>
  </div>-->
