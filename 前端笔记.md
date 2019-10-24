# 面试部分:
## 浏览器内核 
**浏览器内核分为两部分: 渲染引擎, JS引擎**
- 渲染引擎 ( layout engineer  或者rendering  Engine)
	- 负责取得网页的内容 ( HTML, XML, 图像等等), 整理讯息( 例如加入 CSS 等), 以及计算网页的显示方式, 然后会输出到显示器或者打印机.
- JS 引擎
	- 解析 javascript 语言, 执行 javascript 语言来实现页面的动态效果.

#### Trident( IE内核)
国内很多的双核浏览器的其中一个核 便是 Trident, 美其名曰 `"兼容模式"`.
代表:  IE, 遨游, 世界之窗, Avant,  腾讯TT , 猎豹安全浏览器, 360极速浏览器, 百度浏览器...
Windows10 发布后, IE 将其内置浏览器命名为 **`Edge`**,   Edge最显著的特点就是新内核  **`EdgeHTML`**.

#### Gecko (firefox)

Mozilla FireFox(火狐浏览器)采用该内核,Gecko 特点是代码完全公开.

#### WebKit (Safari)
Safari 是苹果公司开发的浏览器,  所用的浏览器内核是 WebKit
代表浏览器:  遨游浏览器3,  Apple Safari(Win/Mac/IPhone/iPad) ,symbian手机浏览器,  Android默认浏览器.

#### Chromium/Bink (chrome)

在 Chromium 项目中研发 Bink  渲染引擎(浏览器核心) , 内置于 Chrome浏览器之中. 
Bink 其实是WebKit的分支,   大部分国产浏览器最新版都采用 Bink 内核.

#### Presto (Opera)
Presto是挪威产浏览器 opera(欧朋浏览器) 的 "前"内核,  目前的最新 opera浏览器已经不再使用该内核, 转而使用了 Bink 内核.

#### 移动端的浏览器内核主要说的是系统内置浏览器的内核.
目前移动设备浏览器上常用的内核有  WebKit, Bink,  Trident,  Gecko 等
其中 iPhone 和 iPad 等苹果 IOS 平台主要是 WebKit.
Android 4.4 之前 Android系统浏览器内核是  WebKit,   Android4.4 系统浏览器切换到了 Chromium, 内核是 WebKit的分支 Bink
Windows  phone 8  系统浏览器内核是 Trident.
