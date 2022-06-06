# 基于现代 GUI 的哔哩哔哩漫画下载器

[![GitHub release](https://img.shields.io/github/release/MOMOYATW/bilibili_manga_downloader.svg?logo=github)](https://github.com/MOMOYATW/bilibili_manga_downloader/releases/latest)
[![GitHub downloads](https://img.shields.io/github/downloads/MOMOYATW/bilibili_manga_downloader/latest/total.svg?logo=github)](https://github.com/MOMOYATW/bilibili_manga_downloader/releases/latest)
[![GitHub downloads](https://img.shields.io/github/downloads/MOMOYATW/bilibili_manga_downloader/total.svg?logo=github)](https://github.com/MOMOYATW/bilibili_manga_downloader/releases)

## 2.0 版本大升级

### 软件界面

<img src="README_imgs/2022-06-04-19-01-12.png" width="500px">

### 使用说明

在栏中填入漫画网址进行搜索，即可获取漫画信息

目前仅支持漫画详细页面网址，形如`https://manga.bilibili.com/detail/mc28528?from=manga_person`

未来计划追加支持根据某话网址进行下载以及关键词搜索

<img src="README_imgs/2022-06-04-19-04-16.png" width="500px">

选中可以下载的漫画，点击开始下载即可添加到下载列表中

<img src="README_imgs/2022-06-04-19-05-13.png" width="500px">

<img src="README_imgs/2022-06-04-19-05-38.png" width="500px">

<img src="README_imgs/2022-06-04-19-05-44.png" width="500px">

对于有**特典**的漫画，其特典信息将被追加到列表的末尾，请留意。

<img src="README_imgs/2022-06-04-19-14-00.png" width="500px">

> #### 关于特典
>
> 按照官方介绍，目前特典有三种形式：视频、动图、图片。目前已经对视频和图片都进行了支持，但是动图由于暂时还没有遇到，因此也无法测试。
>
> 我推测动图就是没有声音的视频，因此理论上当前版本也可以下载。不过如果有人遇到了问题欢迎在 issue 中提出。

下载过程中可以双击任务，从而打开详情窗口。

<img src="README_imgs/2022-06-05-19-01-36.png" width="500px">

下一个版本将实现对任务的开始停止控制~

在设置中，可以将登陆后的 cookie 粘贴到此处，从而下载付费漫画，另外可以修改默认下载路径，下载最大线程数，是否启动时检查更新以及每张图片的请求间隔。

<img src="README_imgs/2022-06-06-00-17-56.png" width="500px">

> #### 有关于登录 cookie 的获取
>
> 在网页上登录后，对于 edge 浏览器，进行如下操作
> <img src="README_imgs/2022-06-04-19-41-46.png" width="500px">
>
> <img src="README_imgs/2022-06-04-19-42-22.png" width="500px">
>
> <img src="README_imgs/2022-06-04-19-44-12.png" width="500px">
>
> 将得到的 SESSDATA 值以`{"SESSDATA":"你的SESSDATA值"}`的形式填入设置中即可
>
> 请注意该值切不可泄露

注意：多线程下载容易导致请求过于频繁，进而导致下载失败，因此谨慎选择。

### 项目依赖包

- requests
- pyside6

---

### 更新

#### V2.1.1

1. 优化代码结构
2. 修改解析页面 ui 全选/全不选 按钮逻辑
3. 解决了打开代理时会导致查询失败的 bug，支持用户自定义 HTTPS 代理
4. 增加对单话网页的支持
5. 增加亮色主题
   需要手动修改配置文件中的 style, 有"dark.qss"和"light.qss"两种选项
6. 增加了自动获取 cookie 的方式，用户通过 web 界面登录
   在程序中登录会导致 PC 端账号被挤下线，请注意

### 开发计划

1. 实现对下载任务的控制
2. 实现自动兑换特典项目
3. 实现漫画的购买功能（主要针对已下架漫画）
4. 自动下载更新功能
5. 修改设置页面 ui
6. 制作成电子书
