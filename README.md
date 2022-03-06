# 基于现代 GUI 的哔哩哔哩漫画下载器

[![GitHub release](https://img.shields.io/github/release/MOMOYATW/bilibili_manga_downloader.svg?logo=github)](https://github.com/MOMOYATW/bilibili_manga_downloader/releases/latest)
[![GitHub downloads](https://img.shields.io/github/downloads/MOMOYATW/bilibili_manga_downloader/latest/total.svg?logo=github)](https://github.com/MOMOYATW/bilibili_manga_downloader/releases/latest)
[![GitHub downloads](https://img.shields.io/github/downloads/MOMOYATW/bilibili_manga_downloader/total.svg?logo=github)](https://github.com/MOMOYATW/bilibili_manga_downloader/releases)

### 软件界面

![](README_imgs/2022-02-23-00-03-58.png)

### 使用说明

在栏中填入漫画网址，即可获取漫画信息

![](README_imgs/2022-02-23-00-05-22.png)

选中可以下载的漫画，点击开始下载即可

![](README_imgs/2022-02-23-00-05-53.png)

在更多设置中，可以将登陆后的 cookie 粘贴到此处，从而下载付费漫画，另外可以修改默认下载路径，以及每张图片的请求间隔。

![](README_imgs/2022-02-26-00-29-13.png)

直接运行项目时，在 src 目录下运行指令

```cmd
python ./download.py
```

### 项目依赖包

- requests
- pyside6

---

### 更新

#### V1.1.0

1. 添加 requirements.txt
2. 调整代码文件结构
3. 增加了终止下载功能
4. 增加了简易的提示窗口

#### V1.1.1

1. 修复了异常弹窗导致程序崩溃的 bug

#### V1.1.2

1. 修复了部分漫画无标题导致创建路径非法的 bug

#### V1.2.0

1. 重构了代码结构
2. 增加了更加详细的下载进度展示功能
3. 调整了漫画下载顺序
4. 调整了图片下载时间间隔，从原来的 0-99s 改为了 0-5000ms

#### V1.2.1

1. 修复了详细进度显示错位的 bug

#### V1.2.2

1. 修补了选择路径功能

#### V1.2.3

1. 增加了窗口阴影以增强观感
2. 修复了关闭主窗口，子窗口仍未关闭的 bug
3. 修复了关闭主窗口时正在下载，则不会保存用户设置的 bug

#### V1.2.4

1. 修改了关闭设置窗口的逻辑，增加了保存按钮
2. 调整了按钮的 qss

#### V1.2.5

1. 修复了用任务栏关闭窗口时不执行关闭逻辑的 bug
2. 修复了点击任务栏窗口无法最小化/恢复的 bug

#### V1.2.6

1. 修复了滚动条样式失效的 bug
2. 更新了资源文件的打包方式
3. 增加了下载完成的提示音

#### V1.2.7

1. 重构代码
2. 将样式提取到单独的样式文件
3. 修复了没有 settings.json 便无法启动程序的 bug

#### V1.2.8

1. 最大化/窗口化图标修正
