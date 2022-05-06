# 基于现代 GUI 的哔哩哔哩漫画下载器

[![GitHub release](https://img.shields.io/github/release/MOMOYATW/bilibili_manga_downloader.svg?logo=github)](https://github.com/MOMOYATW/bilibili_manga_downloader/releases/latest)
[![GitHub downloads](https://img.shields.io/github/downloads/MOMOYATW/bilibili_manga_downloader/latest/total.svg?logo=github)](https://github.com/MOMOYATW/bilibili_manga_downloader/releases/latest)
[![GitHub downloads](https://img.shields.io/github/downloads/MOMOYATW/bilibili_manga_downloader/total.svg?logo=github)](https://github.com/MOMOYATW/bilibili_manga_downloader/releases)

### 软件界面

![](README_imgs/2022-03-20-14-00-17.png)

### 使用说明

在栏中填入漫画网址，即可获取漫画信息

![](README_imgs/2022-03-20-14-00-45.png)

选中可以下载的漫画，点击开始下载即可

![](README_imgs/2022-03-20-14-01-24.png)

在更多设置中，可以将登陆后的 cookie 粘贴到此处，从而下载付费漫画，另外可以修改默认下载路径，以及每张图片的请求间隔。

![](README_imgs/2022-03-20-14-03-44.png)
![](README_imgs/2022-03-20-14-03-55.png)

直接运行项目时，在 src 目录下运行指令

```cmd
python ./download.py
```

### 项目依赖包

- requests
- pyside6

---

### 更新

#### V1.4.1

1. 修复了由于 Windows 命名限制导致的无法下载问题
