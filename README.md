<p align="center">
  <img src="https://raw.githubusercontent.com/Xposed-Modules-Repo/io.github.yishisanren.panes/main/assets/panes-logo.png" alt="格窗图标" width="160">
</p>

<h1 align="center">格窗工作台</h1>

<p align="center">一个大窗做事，四个小窗随时切换。</p>

<p align="center">
  <img src="https://img.shields.io/badge/HyperOS-supported-FF6900?style=flat" alt="小米澎湃 OS">
  <img src="https://img.shields.io/badge/ColorOS-16%20%7C%2017-1F5CDE?style=flat" alt="ColorOS 16 | 17">
  <img src="https://img.shields.io/badge/AOSP--based-installable-3DDC84?style=flat" alt="类原生">
  <img src="https://img.shields.io/badge/LSPosed-Required-C62828?style=flat" alt="需要 LSPosed">
</p>

格窗工作台是一个 LSPosed 模块，给手机原生桌面加一个侧边工作台：一个大窗做事，旁边四个小窗都是真实运行的应用，点一下就和大窗互换。不换桌面，不改主题，关掉工作台，手机就回到原样。

## 支持的系统

- **小米澎湃 OS**：重点适配。大小窗交换、状态栏、桌面和最近任务、负一屏、横屏视频圆角都做了专门处理。
- **ColorOS 16、17**（OPPO、一加、realme）：一直在用的主力平台，流畅好用。
- **其他类原生 ROM**：Android 15 及以上、有 LSPosed 就能装。一大四小、横屏视频、工作场景这些核心功能可以用，桌面相关的动画不一定生效。目前已收到 Flyme、努比亚等机型可以完美使用的反馈，欢迎告诉我你的机型和效果。

## 能做什么

### 一大四小，点一下就换

大窗是你正在用的应用，侧栏四个小窗是四个真实运行的应用，不是截图。点小窗，它和大窗原地对调。

<p align="center">
  <img src="https://raw.githubusercontent.com/Xposed-Modules-Repo/io.github.yishisanren.panes/main/assets/02-swap.gif" alt="点小窗与大窗互换" width="300">
</p>

### 多种打开方式

屏幕左右底角斜滑、双指上滑/下滑、状态栏左右横滑、控制中心开关，选一种顺手的。还支持配合 Tasker 这类工具自动打开、关闭工作台。

玩游戏时不想误触，可以把应用加进手势黑名单：打开格窗，在「管理应用」里找到「手势黑名单」。

<p align="center">
  <img src="https://raw.githubusercontent.com/Xposed-Modules-Repo/io.github.yishisanren.panes/main/assets/01-gestures.gif" alt="打开方式设置、底角斜滑和状态栏横滑" width="300">
</p>

### 快捷关闭和暂停小窗应用

在任意一个小窗上往上滑，直接关掉里面的应用。长按小窗，可以选择暂停应用（省电、不卡顿）、保持实时（部分游戏、视频需要一直运行）或关闭应用。

<p align="center">
  <img src="https://raw.githubusercontent.com/Xposed-Modules-Repo/io.github.yishisanren.panes/main/assets/03-longpress.gif" alt="上滑关闭小窗应用，长按小窗选择暂停或关闭" width="300">
</p>

### 横屏视频置顶或全屏播放

视频点全屏，放到屏幕顶部播放，下面照样换窗、回消息；也可以选在大窗里横过来播放，或者关闭工作台全屏看。

<p align="center">
  <img src="https://raw.githubusercontent.com/Xposed-Modules-Repo/io.github.yishisanren.panes/main/assets/04-video.gif" alt="横屏视频放到顶部播放，下面照常使用" width="300">
</p>

### 常用应用栏

点图标在大窗打开，拖进小窗就在小窗打开；装了分身的可以选开哪个。在任何应用里分享链接或文字，也能直接发到大窗或小窗。

<p align="center">
  <img src="https://raw.githubusercontent.com/Xposed-Modules-Repo/io.github.yishisanren.panes/main/assets/05-favorites.gif" alt="点常用应用在大窗打开，拖进小窗在小窗打开" width="300">
</p>

### 工作场景

把大窗和四个小窗存成一组，点一下整套打开，也能把某个场景添加到桌面快捷方式。

<p align="center">
  <img src="https://raw.githubusercontent.com/Xposed-Modules-Repo/io.github.yishisanren.panes/main/assets/06-scenes.gif" alt="点场景按钮，整套应用一起打开" width="300">
</p>

### 比价

商品名输入一次，拼多多、抖音商城、京东、淘宝同时搜，各开一个窗口并排看；也支持外卖。只帮你打开搜索结果，不抓价格、不下单。

<p align="center">
  <img src="https://raw.githubusercontent.com/Xposed-Modules-Repo/io.github.yishisanren.panes/main/assets/07-compare.gif" alt="输入一次商品名，四个购物应用同时搜索" width="300">
</p>

### 付款与扫一扫

微信、支付宝的扫一扫和付款码放在一个面板里，一键打开。只负责打开对应页面，不读取账户，也不会替你确认付款。

<p align="center">
  <img src="https://raw.githubusercontent.com/Xposed-Modules-Repo/io.github.yishisanren.panes/main/assets/08-pay.gif" alt="付款与扫一扫面板" width="300">
</p>

### 外观

小窗放左边或右边、控制区放顶部或底部、小窗圆角或直角，都可以调；浅色深色跟随系统。

## 免费和解锁

大部分功能一直免费：一大四小、打开方式、常用应用、发到格窗、付款与扫一扫、2 个工作场景、外观设置、上滑关闭、自动化命令。

第一次打开工作台后，所有功能免费用 1 天。之后横屏视频留在工作台、第 3 个及以上的工作场景、比价、小窗暂停这几项需要解锁：¥6.6，一次付费，永久使用，换手机可以免费迁移一次。购买前请充分试用，购买后不退款。在格窗设置里点「解锁格窗」即可。

## 使用要求

- Android 15 及以上，需要 Root 和 LSPosed（支持 libxposed 新 API）。
- 本模块会修改系统界面、桌面和 system_server 的行为，刷之前请准备好救砖手段。
- 以前装过 NeXtep（包名 `io.github.lujinxin.nextep`）的，先在 LSPosed 里停用并卸载，两个模块不能同时用。

## 安装

1. 下载 APK 安装（包名 `io.github.yishisanren.panes`）。
2. 在 LSPosed 里启用「格窗工作台」，作用域按机型勾选：
   - 小米：SystemUI、系统框架、系统桌面、智能助理
   - OPPO、一加、realme：SystemUI、系统框架、桌面、应用分身服务、负一屏
   - 类原生：SystemUI、系统框架
3. 重启手机。
4. 打开「格窗」，选常用应用，选一种打开方式。

## 下载和反馈

- 下载：本页「版本」里的 APK，或 [夸克网盘](https://pan.quark.cn/s/bb615e3d0d68?pwd=X5gm#/list/share)
- 反馈：[问题与建议问卷](https://my.feishu.cn/share/base/shrcn7gYOpCevm4vjtweE4Vyywh)

## 致谢

感谢原作者 lujinxin：格窗是在他开源的 NeXtep 基础上改出来的，NeXtep 致敬锤子的 OneStep，没有 NeXtep 就没有格窗。
