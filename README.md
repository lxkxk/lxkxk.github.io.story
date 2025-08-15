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
