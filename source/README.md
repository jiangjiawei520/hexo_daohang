- # 我的网址导航


我的个人博客：<https://dh.jiang7zzz.xyz>。

本导航是使用hexo搭建，使用中。

### 

本项目这是一个网址导航网站，内容均由[viggo](http://viggoz.com/)收集并整理。本项目前端基于bootstrap前端框架开发.

这是一个开源的公益项目，可以拿来制作自己的网址导航，也可以做与导航无关的网站。如果你有任何疑问，可以通过个人网站[viggoz.com](http://viggoz.com/)中的联系方式联系原始开发人。

## 怎么用?

你可以像我一样直接使用静态托管形式，如果你需要一个后台系统方便管理，可以参考下面的第二第三种解决方案：

#### 方法1. 使用静态托管

最简单快速上线自己的导航网站，你可以直接**下载**本项目修改内容既可部署上线。

#### 方法2. 使用基于 Laravel 搭建的后台系统![fire](https://github.githubassets.com/images/icons/emoji/unicode/1f525.png)(感谢[@hui-ho](https://github.com/hui-ho)提供)

开源地址：https://github.com/hui-ho/WebStack-Laravel

Docker部署版本:https://hub.docker.com/r/arvon2014/webstack-laravel

#### 方法3（本项目方式）. Hexo主题

开源地址： https://github.com/HCLonely/hexo-theme-webstack

#### 方法4. Hugo主题

开源地址： https://github.com/iplaycode/webstack-hugo 主题演示： https://iplaycode.github.io/nav/

#### 方法5. 基于Java开发的后台系统![fire](https://github.githubassets.com/images/icons/emoji/unicode/1f525.png)(感谢[@jsnjfz](https://github.com/jsnjfz)提供)

开源地址：https://github.com/jsnjfz/WebStack-Guns

#### 方法6. springboot后台 Nikati-WebStack-Guns ![heart](https://github.githubassets.com/images/icons/emoji/unicode/2764.png) (感谢[Nikati (Nikati)](https://github.com/Nikati)提供)

开源地址：https://github.com/Nikati/WebStack-Guns-NKT

#### 方法7.1 使用 Jekyll 版本的后台![fire](https://github.githubassets.com/images/icons/emoji/unicode/1f525.png)(感谢[@0xl2oot](https://github.com/0xl2oot)提供)

开源地址：https://github.com/0xl2oot/webstack-jekyll

#### 方法7.2 从Chrome书签生成Jekyll版本配置的工具

体验网址： https://w.hanxi.info/convert.html 开源地址： https://github.com/hanxi/webstack-jekyll

#### 方法8.1 钻芒二开Typecho主题

开源地址：https://www.zmki.cn/5366.html 比较详细的安装教程：https://www.waoww.com/typecho-theme/zmki-webstack.html 预览地址：https://tool.zmki.cn/

#### 方法8.2 SEOGO二开Typecho主题

开源地址：https://www.seogo.me/muban/webstack.html

#### 方法9. 静态博客Gridea主题

开源地址: https://github.com/lmm214/gridea-theme-webstack 在线预览: https://edui.fun/

#### 方法10. VUE版本

开源地址: https://github.com/Anjaxs/WebStack-vue/tree/master

#### 方法11. flask-blog-platform

开源地址: https://github.com/shitianfang/flask-blog-platform/tree/master

#### 方法12. 自己写后台系统

可以按照自己的喜好和框架搭建后台系统，也可以参考我设计好的后台框架自行搭建。本站设计开发过程在我的博客文章有详细讲到[《webstack | viggo》](http://blog.viggoz.com/2018/01/03/2018-01-03-webstack/)。静态源码（半成品）：https://github.com/WebStackPage/webstack-Admin

## 关于图片资源

`/assets/images/logos/default.png` 这是网站标签的默认图标

`/assets/images/logos` 这里是所有网站内的图标切图，尺寸均为120px*120px

`/assets/webstack_logos.sketch` 这是网站标签收录的所有图标设计源文件，你可以在这里[下载](https://webstackpage.github.io/assets/webstack_logos.sketch) 。打开前请确认Sketch版本高于50.2(55047)

1、新建hexo项目

```
hexo init

npm install

hexo g # 生成

hexo s #启动本地服务器,这一步之后就可以通过http://localhost:4000 查看

保存仓库后后，安装一个扩展
npm install hexo-deployer-git --save   
```

2、配置主题：

根目录下_config.yml:theme: webstack



3、配置仓库：

```
deploy:
   type: git
   repo: git@github.com:JiangJiaWei520/hexo_daohang.git
   branch: master
```



4、配置右上角导航到github主页：

```
githubCorner: '<a href="https://github.com/HCLonely/hexo-theme-webstack" class="github-corner" aria-label="View source on GitHub"><svg width="80" height="80" viewBox="0 0 250 250" style="fill:#151513; color:#fff; position: absolute; top: 0; border: 0; right: 0;" aria-hidden="true"><path d="M0,0 L115,115 L130,115 L142,142 L250,250 L250,0 Z"></path><path d="M128.3,109.0 C113.8,99.7 119.0,89.6 119.0,89.6 C122.0,82.7 120.5,78.6 120.5,78.6 C119.2,72.0 123.4,76.3 123.4,76.3 C127.3,80.9 125.5,87.3 125.5,87.3 C122.9,97.6 130.6,101.9 134.4,103.2" fill="currentColor" style="transform-origin: 130px 106px;" class="octo-arm"></path><path d="M115.0,115.0 C114.9,115.1 118.7,116.5 119.8,115.4 L133.7,101.6 C136.9,99.2 139.9,98.4 142.2,98.6 C133.8,88.0 127.5,74.4 143.8,58.0 C148.5,53.4 154.0,51.2 159.7,51.0 C160.3,49.4 163.2,43.6 171.4,40.1 C171.4,40.1 176.1,42.5 178.8,56.2 C183.1,58.6 187.2,61.8 190.9,65.4 C194.5,69.0 197.7,73.2 200.1,77.6 C213.8,80.2 216.3,84.9 216.3,84.9 C212.7,93.1 206.9,96.0 205.4,96.6 C205.1,102.4 203.0,107.8 198.3,112.5 C181.9,128.9 168.3,122.5 157.7,114.1 C157.9,116.9 156.7,120.9 152.7,124.9 L141.0,136.5 C139.8,137.7 141.6,141.9 141.8,141.8 Z" fill="currentColor" class="octo-body"></path></svg></a><style>.github-corner:hover .octo-arm{animation:octocat-wave 560ms ease-in-out}@keyframes octocat-wave{0%,100%{transform:rotate(0)}20%,60%{transform:rotate(-25deg)}40%,80%{transform:rotate(10deg)}}@media (max-width:500px){.github-corner:hover .octo-arm{animation:none}.github-corner .octo-arm{animation:octocat-wave 560ms ease-in-out}}</style>'

```



5、配置左侧菜单栏：

```
# 在\source\_data中添加devTools.yml、hotTools.yml、myBlog.yml,且必须按格式缩进,另外_data中存在对应的.yml且存在正确的数据,叶子目录必须配置config
menu:
  - name: 常用网站
    icon: far fa-star
    #config: hotTools
    submenu:
      - name: 个人网站
        icon: fas fa-tools
        config: personalWebsite
      - name: 代码托管
        icon: fas fa-tools
        config: devTools
 - name: 其他网站
   icon: fas fa-tools
   config: other
#hotTools、personalWebsite、devTools、other可配置在根目录_config.yml,或者\source\_data中
_config.yml:
devTools:
  - name: Github
    url: https://github.com/
    img: /images/logos/github.png
    description: 面向开源及私有软件项目的托管平台。
  - name: Github
    url: https://github.com/
    img: /images/logos/github.png
    description: 面向开源及私有软件项目的托管平台。
  - name: Github
    url: https://github.com/
    img: /images/logos/github.png
    description: 面向开源及私有软件项目的托管平台。
\source\_data\hotTools.yml、  \source\_data\personalWebsite.yml:
- name: xxx
  url: https://xxx
  img: /images/favicon.ico
  description: 我的个人博客hexo
```



6、关于本站内容配置在\themes\webstack下\_config.yml中的aboutPage里面



### 注意：

- **hexo 的 CNAME 文件** 需要放在source 目录下，每次运行hexo clean会清除public 目录，hexo g重新生成，hexo d发布到远程服务器。

1、准确来说 CNAME 文件是放在 hexo 项目下的 source 目录，你再运行下

```text
hexo generade
```

然后你再去 public 目录中看看就明白了

BTW，为了达到更有说服力的验证，最好在开始前先运行下

```text
hexo clean
```

这样会先删除 public 目录

- **hexo 的 README.md等文件**

  [原文]: (https://www.dazhuanlan.com/2020/03/20/5e73a3d07ebbc/)

  文件添加在 **Hexo**目录下的**source**根目录下创建**README.md**文件。并编辑保存。

  - **防止README.md被渲染**

  编辑根目录的_config.yml文件中的“skip_render”参数。
  eg：

  ```
  skip_render: [README.md]
  ```

  保存并退出。

  - **完成**

  试着命令部署，再去你的 Git仓库看看是否存在README.md文件。

  ```
  $ Hexo clean && hexo g && hexo d
  ```

- **插入网站运行时间代码**

  ```
  样例 1:
  <span>
  本站已运行
  </span>
  <span id="span_dt_dt">
  </span>
  <script>
  /*建站时间*/
  function show_date_time() {
  window.setTimeout("show_date_time()", 1e3);
  var BirthDay = new Date("2018/03/01"),
  today = new Date,
  timeold = today.getTime() - BirthDay.getTime(),
  msPerDay = 864e5,
  e_daysold = timeold / msPerDay,
  daysold = Math.floor(e_daysold),
  e_hrsold = 24 * (e_daysold - daysold),
  hrsold = Math.floor(e_hrsold),
  e_minsold = 60 * (e_hrsold - hrsold),
  minsold = Math.floor(60 * (e_hrsold - hrsold)),
  seconds = Math.floor(60 * (e_minsold - minsold));
  span_dt_dt.innerHTML = daysold + "天" + hrsold + "小时" + minsold + "分" + seconds + "秒";
  }
  show_date_time();
  </script>
  ```
  ```
  样例 2：
  当前系统时间
  <span id="nowTime"></span>
  <script type="text/javascript">
  //获取系统时间
  var newDate = '';
  getLangDate();
  //值小于10时，在前面补0
  function dateFilter(date){
  if(date < 10){return "0"+date;}
  return date;
  }
  function getLangDate(){
  var dateObj = new Date(); //表示当前系统时间的Date对象
  var year = dateObj.getFullYear(); //当前系统时间的完整年份值
  var month = dateObj.getMonth()+1; //当前系统时间的月份值
  var date = dateObj.getDate(); //当前系统时间的月份中的日
  var day = dateObj.getDay(); //当前系统时间中的星期值
  var weeks = ["星期日","星期一","星期二","星期三","星期四","星期五","星期六"];
  var week = weeks[day]; //根据星期值，从数组中获取对应的星期字符串
  var hour = dateObj.getHours(); //当前系统时间的小时值
  var minute = dateObj.getMinutes(); //当前系统时间的分钟值
  var second = dateObj.getSeconds(); //当前系统时间的秒钟值
  var timeValue = "" +((hour >= 12) ? (hour >= 18) ? "晚上" : "下午" : "上午" ); //当前时间属于上午、晚上还是下午
  newDate = dateFilter(year)+"年"+dateFilter(month)+"月"+dateFilter(date)+"日 "+" "+dateFilter(hour)+":"+dateFilter(minute)+":"+dateFilter(second);
  document.getElementById("nowTime").innerHTML = timeValue+"好！当前时间为： "+newDate+"　"+week;
  setTimeout("getLangDate()",1000);
  }
  </script>
  ```
  ```
  样例三：
  function showtime(times) { //传入时间的参数
  var time_1 = new Date(times).getTime();
  var time_2 = new Date().getTime();
  var time_3;
  var time_distance;
  //计算时间差
  if (time_1 > time_2) {
  time_distance = time_1 - time_2;
  } else {
  time_distance = time_2 - time_1;
  }
  if (time_distance > 0) {
  // 天时分秒换算
  var int_day = Math.floor(time_distance / 86400000);
  time_distance -= int_day * 86400000;
  var int_hour = Math.floor(time_distance / 3600000);
  time_distance -= int_hour * 3600000;
  var int_minute = Math.floor(time_distance / 60000);
  time_distance -= int_minute * 60000;
  var int_second = Math.floor(time_distance / 1000);
  // 时分秒为单数时、前面加零
  if (int_day < 10) {
  int_day = "0" + int_day;
  }
  if (int_hour < 10) {
  int_hour = "0" + int_hour;
  }
  if (int_minute < 10) {
  int_minute = "0" + int_minute;
  }
  ```
  
