## 合集展示

注：Github 限制 gif 大小，超过 10 mb 无法上传。

### 1. 一秒语音包变声器 App

[瑞宇](https://github.com/zhangruiyu) 独立开发的 **一秒语音包变声器**，市场累计下载量 100w+，获得过华为耀星 App 奖

![59E6C54EBCCF56E6B7744292BB3AB70D.jpg](https://p9-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/81a515ad92a1447e9bd014f5d80bfc42~tplv-k3u1fbpfcp-watermark.image)

下面是使用 keframe 前后统计 300 帧的对比：

>**卡顿帧从平均 60 帧出现一次优化为 300 帧中出现一次，轻微卡顿由平均 7 帧一次优化为未出现，流畅占比从 36.3% 提高到 74.7%**。

#### **数据展示**

测试机型：Mate30 pro
| 优化前                                                       | 优化后                                                       |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![Screenshot_20210712-152724.jpg](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/51fd23f6358040ebbc5f5a14a33416b0~tplv-k3u1fbpfcp-watermark.image) | ![Screenshot_20210712-152659.jpg](https://p6-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/79cbdbdb48a1437181bee07be62d12cd~tplv-k3u1fbpfcp-watermark.image) |

|                            | 优化前  | 优化后                 |
| -------------------------- | ------- | ---------------------- |
| 平均多少帧出现一帧卡顿     | 60      | 300                    |
| 平均多少帧出现一帧轻微卡顿 | 7.0     | 未出现轻微卡顿         |
| 最大耗时                   | 146.0ms | 76.0ms（图中展示有误） |
| 平均耗时                   | 25.2ms  | 18.3ms                 |
| 流畅帧占比                 | 36.3%   | 74.7%                  |

这个 Case 中，卡顿大多发生在 TAB 切换的场景。因为系统会在瞬间完成页面渲染，如果页面结构复杂，在 mate30 pro 这样的高端设备上也容易引起卡顿。通过 keframe 对页面中每一个模块进行分帧加载，能有效优化切换时的卡顿。并且从体感而言，整个过渡任然非常自然。

***

### 2. 匿名 A 岛

「麋鹿君」，一个还在战斗的独立开发，上架了多款精美的应用，[AppStore](https://apps.apple.com/cn/developer/嘉楠-孙/id1480541469) & [GooglePlay](https://play.google.com/store/apps/dev?id=5706067037523299093)

<img src="https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/841c7af0d3e0419f9c015cc59ffef193~tplv-k3u1fbpfcp-watermark.image" alt="image.png" align='left' style="zoom:30%;" />

> 开发者反馈：这是一款刚刚开始的 A 岛第三方客户端项目，搭配 Keframe 框架后在测试用机（乐视1s）上有惊人表现，效果对比「惨烈」。

#### 数据展示

下面是使用 keframe 前后统计 100 帧的对比，测试机型：乐视 1S。

| 优化前                                                       | 优化后                                                       |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| <img src="https://p1-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/fbb7d774e2964d51a22b57b39089090e~tplv-k3u1fbpfcp-watermark.image" alt="20210712_173854_rmscr.jpg" style="zoom:50%;" /> | <img src="https://p1-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/c6a0deedeae44e0caf731ef8879ddcc7~tplv-k3u1fbpfcp-watermark.image" alt="20210712_173313_rmscr.jpg" style="zoom:50%;" /> |

这个优化效果我觉得不需要任何多余的说明，**整个 App 从几乎不可用状态到 100 帧中 0 卡顿**。这也是 keframe 优化的最大价值，让**一些复杂页面在中低端设备上从不可用到流畅运行的状态**。

同时还有 iPhone11 上的演示数据

| 优化前 | 优化后 |
| --- | --- |
| ![image.png](https://p1-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/45431165cbfe4b0a821dbb02f537aaf3~tplv-k3u1fbpfcp-watermark.image) |  ![image.png](https://p6-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/15cd40b851b64feba7bc468dc78629a2~tplv-k3u1fbpfcp-watermark.image)|

性能较好的设备本身卡顿也几乎不存在卡顿，而 keframe 则更进一步保证了每一帧的流畅。


### 3、百灵创作
这是一款还在开发阶段的 App ，希望做一款简约而不简单，自由又安全的专业码字软件。
#### 数据展示

下面是使用 keframe 前后统计 300 帧的对比，测试机型：小米 9。

| 优化前                                                       | 优化后                                                       |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ![image.png](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/49d6c70bf34d4bea9c0a08378b630087~tplv-k3u1fbpfcp-watermark.image)|  ![image.png](https://p1-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/a02d3c680c7b412e83c2fb8662281ffc~tplv-k3u1fbpfcp-watermark.image) |

**卡顿峰值从 244.0ms 降低到了 126.0ms ，从平均 50 帧出现一次卡顿优化为平均 150 帧出现一次卡顿，300帧平均帧率从 22.4ms 优化至 18.5 ms**。


有关 keframe 的更多用法请查看：

github 地址：[https://github.com/LianjiaTech/keframe](https://github.com/LianjiaTech/keframe)

pub 查看：[https://pub.dev/packages/keframe](https://pub.dev/packages/keframe)

> **Dont forget star !**

## 

我日常的使用经验来看，对于一些分页的列表，我会将 ListView 的 `cacheExtent` 设置为 700，同时加上渐变动画，在中低端设备上能得到明显的体验优化，而高端设备上用户几乎无感知加载。

而对于详情这一类列表项内容有限的页面，我会将 `cacheExtent` 直接调到 `double.infinity`，打开页面即进行分帧加载，这样在滑动过程中也能带来最好的体验。

再次感谢提供案例的三位开发者，能感受到每个开发者对自己的 app 倾注了大量的心血，做得都非常精美。

最后，非常欢迎分享你的优化演示或者优化技巧（不局限于 keframe），这个项目会持续跟进，欢迎你的关注。

