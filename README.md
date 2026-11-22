<p align="center">
  <img src="https://raw.githubusercontent.com/Xposed-Modules-Repo/io.github.yishisanren.panes/main/assets/panes-logo.png" alt="格窗图标" width="160">
</p>

<h1 align="center">格窗工作台</h1>

<p align="center">一块屏幕，同时用好几个应用。</p>

<p align="center">
  <img src="https://img.shields.io/badge/小米-supported-FF6900?style=flat" alt="小米">
  <img src="https://img.shields.io/badge/OPPO-supported-1F5CDE?style=flat" alt="OPPO">
  <img src="https://img.shields.io/badge/vivo-supported-415FFF?style=flat" alt="vivo">
  <img src="https://img.shields.io/badge/荣耀-supported-00B3A4?style=flat" alt="荣耀">
  <img src="https://img.shields.io/badge/LSPosed-Required-C62828?style=flat" alt="需要 LSPosed">
</p>

格窗是一个 LSPosed 模块，把屏幕变成一张工作台：**一个大窗做事，旁边一列小窗候着**。小窗里是真实运行的应用，画面一直在动，点一下就和大窗互换。直板手机、折叠屏、平板，竖着拿、横着拿，都是同一套用法。

不换桌面、不改系统主题。关掉工作台，手机就回到原来的样子。

<p align="center">
  <img src="https://raw.githubusercontent.com/Xposed-Modules-Repo/io.github.yishisanren.panes/main/assets/v4-01-open.gif" alt="底角斜滑打开工作台" width="300">
</p>

## 能做什么

### 一套排版，适配所有屏幕

直板手机、小折叠、大折叠、阔折叠、平板，统一成「顶部控制区 + 大窗 + 小窗列」，窗口按屏幕比例等比缩放，折叠屏、平板横着拿也是同一套用法。


### 小窗最多 12 个，随加随删

小窗列底部点「＋ 增加小窗」，多一格。在小窗里往屏幕中间滑，关掉应用、小窗留空；在空小窗上再滑一次，这一格就删掉。点小窗，它和大窗原地互换。

<p align="center">
  <img src="https://raw.githubusercontent.com/Xposed-Modules-Repo/io.github.yishisanren.panes/main/assets/v4-03-panes.gif" alt="增加小窗、删除空小窗" width="300">
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/Xposed-Modules-Repo/io.github.yishisanren.panes/main/assets/v4-02-swap.gif" alt="点小窗与大窗互换" width="300">
</p>

### 视频和游戏置顶：看到什么，置顶什么

大窗里在播视频或在玩游戏时，控制区出现置顶按钮。点一下，大窗里的画面原样挪到置顶区，下面的大窗、小窗照常用。

- 竖着拿，置顶区在屏幕顶部；横着拿（折叠屏展开、平板），置顶区在左侧。
- 画面按原比例完整放进置顶区，不裁切、不拉伸。竖着拿时，全屏的横屏视频置顶后上下不留黑边。
- 页面里的小播放器、横屏全屏、竖版全屏视频、横着玩和竖着玩的游戏，都能置顶。想只看视频画面，先在大窗里点全屏，再点置顶。
- 取消置顶：点「取消置顶」，画面原样回到大窗；或在置顶区那一侧的屏幕边缘往里划。

<p align="center">
  <img src="https://raw.githubusercontent.com/Xposed-Modules-Repo/io.github.yishisanren.panes/main/assets/v4-04-pin.gif" alt="抖音置顶到顶部，下面用京东，再取消置顶" width="300">
</p>

### 工作场景

把大窗和小窗里的一套应用存成场景，比如「工作」放钉钉、飞书、邮箱，「追剧」放视频和聊天。场景可以放进常用应用栏，点一下整套打开，需要几个小窗就自动补几个。

<p align="center">
  <img src="https://raw.githubusercontent.com/Xposed-Modules-Repo/io.github.yishisanren.panes/main/assets/v4-05-scenes.gif" alt="点场景，整套应用一起打开" width="300">
</p>

### 新应用自动进大窗

不管从通知、链接还是控制中心打开，应用都进大窗，原来的应用自动挪进空小窗，不会被关掉。

<p align="center">
  <img src="https://raw.githubusercontent.com/Xposed-Modules-Repo/io.github.yishisanren.panes/main/assets/v4-06-auto-main.gif" alt="从链接打开应用进大窗，原来的应用挪进小窗" width="300">
</p>

### 更多

| 功能 | 怎么用 |
|---|---|
| 常用应用栏 | 控制区一排常用应用和场景，点一下在大窗打开，拖到小窗就在小窗打开；分身应用可选 |
| 多种打开方式 | 左下角或右下角斜滑、双指上下滑、状态栏横滑，或控制中心「格窗」开关；游戏可设为手势不生效 |
| 拖文件进小窗 | 在大窗长按图片或文件，拖到小窗上，直接落进它当前的页面，比如正开着的微信聊天 |
| 付款与扫一扫 | 微信、支付宝的扫一扫和付款码，放在常用应用栏一点就开；只打开对应页面，不读取账户 |
| 比价 | 商品名输一次，几个外卖或购物应用同时搜，结果并排对照；只打开搜索结果，不抓价格、不下单 |
| 沉浸模式 | 大窗放大居中，四周模糊壁纸，小窗收成底部 Dock |
| 顶栏标题 | 时间、番茄钟、下一个日程、温度、充电功率、网速，点一下切到下一组 |
| 省电 | 小窗按 30 帧刷新，换到大窗立刻满帧；不常用的小窗可设「应用休眠」 |
| 自动化 | 支持 Tasker、MacroDroid，把工作台绑到侧键、悬浮球或定时任务 |

<p align="center">
  <img src="https://raw.githubusercontent.com/Xposed-Modules-Repo/io.github.yishisanren.panes/main/assets/v4-07-compare.gif" alt="比价：输入一次，几家并排出结果" width="300">
</p>

## 免费和解锁

第一次打开工作台后，所有功能免费用 1 天。

**一直免费**：大窗加最多 4 个小窗、打开方式、常用应用栏、拖文件、付款与扫一扫、2 个工作场景、自动化。

**解锁后多得到**：视频和游戏置顶、5～12 个小窗、更多工作场景、沉浸模式、多组顶栏标题、比价、应用休眠。

在格窗设置里点「解锁格窗」即可。

## 支持的系统

支持主流安卓操作系统，包含小米、OPPO、vivo、荣耀以及其他安卓类原生操作系统等（Android 15 及以上）。

系统移植版和魔改版随缘使用，有问题不修。

## 使用要求

- 已 Root，装好 Zygisk 和 LSPosed（支持 libxposed 新 API）。
- 本模块会修改系统界面、桌面和 system_server 的行为，刷之前请准备好救砖手段。

## 安装

1. 下载 APK 安装（包名 `io.github.yishisanren.panes`）。
2. 在 LSPosed 里启用「格窗工作台」，勾选推荐作用域（SystemUI、系统框架，以及你手机的桌面）。
3. 重启手机。
4. 打开「格窗」，选常用应用，选一种打开方式。

## 下载和反馈

- 下载：本页「版本」里的 APK，或 [夸克网盘](https://pan.quark.cn/s/bb615e3d0d68?pwd=X5gm#/list/share)
- 反馈：[问题与建议问卷](https://my.feishu.cn/share/base/shrcn7gYOpCevm4vjtweE4Vyywh)

## 致谢

感谢原作者 lujinxin：格窗是在他开源的 NeXtep 基础上改出来的，NeXtep 致敬锤子的 OneStep，没有 NeXtep 就没有格窗。
