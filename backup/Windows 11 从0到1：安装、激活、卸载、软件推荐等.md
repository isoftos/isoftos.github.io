#Windows #激活 #软件分享 #软件列表 #系统设置

> 更新与：2024-05-20，[首发和后续更新](https://isoftos.github.io)

## 一、下载安装

- win11 系统镜像下载
  - <https://www.microsoft.com/zh-cn/software-download/windows11>
- 官方下载：Windows 11 安装助手
  - <https://go.microsoft.com/fwlink/?linkid=2171764>
  - 自测
- PE安装：有可能 有自带程序！
  - <http://www.wepe.com.cn/>
    - 比较精简纯净的PE，很多假站，小心
  - <http://www.sysceo.com/>
    - 现在安装后会给你装一些东西：驱动总裁什么的
- [rufus](https://rufus.ie/downloads/)
  - 很多人推荐，自搜自测

## 二、更新系统

> 安装完成后，立马更新2~3次 重启，更新到检查没有更新为止。

原因：

1. 发现 Win11 23H2，有些版本安装后，没有不休眠选项，无法待机远程。
2. 驱动建议更新成最新，避免奇怪问题。

### 安装驱动

- 驱动软件：360驱动、驱动精灵、各种厂商官网下载对应驱动
- MSI 主板 会在第一次检查更新的时候弹窗给你，让你下载驱动和一些软件，去掉除驱动外的其他所有软件。
- AMD、Intel等CPU官网可以下载一些驱动，有需要自己下载
- 笔记本官网也有驱动下载

## 三、系统设置

### 3.0 激活Windows 11(建议先激活)

- 不激活，专业版功能会用不了
- 激活好后，修改电脑名称、设置默认本地用户的 密码，方便远程访问
- [Microsoft-Activation-Scripts](https://github.com/massgravel/Microsoft-Activation-Scripts)
  - 一个Windows和Office激活器，使用HWID / Ohook / KMS38 / Online KMS激活方法，专注于开源代码和较少的反病毒检测。
  - 右键单击Windows开始菜单，选择“PowerShell”或“Terminal (Not CMD)” 执行下面代码自动弹窗让你输入选项
    - `irm https://massgrave.dev/get | iex`
  - permanent = 永久，也有 180 天的，自己选择

### 3.1 修改电源计划，不休眠

- 控制面板 - 电源
  - 设置成 3min关屏、永不休眠，休眠后无法唤醒 远程访问。

### 3.2 开启远程访问

1. 激活才能用这个功能、用户有密码才能使用
2. 不用远程的跳过此项
3. 个人需要内网访问远程操控(摸鱼)，自己想办法打通内网，可以：`ZeroTier`、TeamViewer、ToDesk。

### 3.3 关闭防火墙

一直关闭防火墙，不会有奇奇怪怪的弹窗，被拦截问题，可自行下载火绒或裸奔，安全自负。

### 3.4 开机自启软件

1. 任务管理器 - 启动 - 把不需要的软件禁用自启
2. 设置 ZeroTier 等软件开机自启，方便远程控制等

### 3.5 其他设置

1. 任务栏 自动透明背景：[TranslucentTB](https://github.com/TranslucentTB/TranslucentTB)，商店也有个汉化版。
2. 任务栏 搜索改成只显示图标、靠左、取消小组件等
3. 修改开始菜单为 win 10 等风格，自己下载 Start11 等软件

## 四、卸载软件

- [卸载 windows defender](https://github.com/ionuttbara/windows-defender-remover/)
- <https://geekuninstaller.com/>
  - 特点：卸载完后会自动扫描残留 注册表和 文件。
  - 免费版够用，专业版是支持批量卸载，还有些省事的操作。
- 卸载列表
  - win 自带应用、商店应用等
  - pe 给你装的无用软件
  - 刚组装电脑后，测试性能和硬件的软件、跑分软件等

## 五、安装软件

### 搜文件

- [Maye 一个简洁小巧的快速启动工具](https://github.com/25H/Maya)
  - 不要用新版。
- [Everything](https://www.voidtools.com/downloads/)
- [Listary 6 pro](https://www.listary.com/download)
  - 双击ctrl

### [windows-apps](windows-apps.md)

- [window-terminal](window-terminal.md)
- wget
- [wsl](wsl.md)
  - 子系统等可以直接在商店搜

### 上网冲浪

#### 下载

- [Neat-Download-Manager](https://github.com/Neatdownloadmanager/Neat-Download-Manager)
  - 不用 IDM，这个就好用，有民间汉化版 自己搜

#### 穿越

- [gh加速](https://gh.22016.xyz)
- 要上gh什么的，你懂的
- <https://github.com/clash-verge-rev/clash-verge-rev>

### 浏览器

- <https://chrome.google.com/>
  - 记得修改默认浏览器，Edge 大把捆绑，个人喜好，自行抉择
- <https://www.runningcheese.com/>
  - 绿化版的开箱即用的 各种浏览器
- [TrafficMonitor: 显示网速、CPU、内存悬浮窗软件，支持任务栏显示、更换皮肤](https://github.com/zhongyang219/TrafficMonitor)

#### 书签、导航页

- Raindrop.io

#### 浏览器插件

- 扩展管理器（Extension Manager）
- 篡改猴
- 沉浸式翻译
- uBlock Origin
- uBlacklist
- Web Clipper
- SingleFile
- FeHelper(前端助手)

#### 油猴脚本

- <https://greasyfork.org/zh-CN/scripts>

### 图片

- 图片管理器
  - FastStone Image Viewer
- 截图、滚动截图
  - PixPin
  - Snipaste

### 视频

- potplayer

### 文档、文本

- [office](office.md)
- pdf： SumatraPDF
- 建议替换自带文本编辑器：[notepad2](https://github.com/zufuliu/notepad2)
- [sublime-text](../../3-leaning/350-dev-tools/sublime-text.md)

### 开发相关

- [[git]]
  - 命令行
    - <https://git-scm.com/downloads>
  - 下面的是可视化git
  - <https://desktop.github.com/>
    - 什么项目都能用，有绿色汉化版。
  - <https://git-fork.com/>
  - 用 IDEA 自带的也行
- [IntelliJ IDEA Ultimate](../../3-leaning/350-dev-tools/idea.md)
- [docker](../../3-leaning/300-program-note/docker.md)

## FAQ

### win11文件管理器，打开非C盘文件夹后正在处理中，CPU飙升卡住很久才响应

问题原因：windows defender 会扫描目录，我的是 softs目录，里面很多软件，每次打开此文件夹都会扫，cpu直接从2%->30%

解决方案：

1. 用工具 [卸载 windows defender](https://github.com/ionuttbara/windows-defender-remover/)，我是已经关闭所有防火墙了，无效，没有试 添加安全文件夹，有问题的可以试试排除文件夹
2. 网友说是因为：固态分区了引起，我重装只有一个分区后确实不卡，但是感觉不是分区问题，是扫描问题
3. 不用自带的管理器，网友说：用 `360文件管理` 替代，下载记得选最后面的 直接下载，不要下到全家桶，个人体验感觉还行
4. 其他的修改注册表 block、改主文件夹、不勾导航窗格…… 各种都试了，无效，别试、浪费时间。

---

大佬可补充，最近在组装电脑，弄NAS，简单汇总下win下的设置。