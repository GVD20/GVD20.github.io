# BK_Studio · Owlcarp

从宿舍角落的 BK_STATION，到建立在对话上的 BK_Studio。一个真实打印店的三年与下一步。

作者：Owlcarp

原文：https://gvd20.github.io/bk-station/

3D预览

# BK_STATION

一个真实的  
打印店运营项目

2023 年秋天，我购入了第一台二手打印机，型号是爱普生 L4168。还有一张小桌子、一台 J1900 主机作为服务器，设计了一套Logo，在宿舍角落开始运营这家名为 **BK_STATION 小黑店** 的打印铺。这还远算不上是一个项目，我最初只想在宿舍里做一点自己的小生意。

![2023 年 10 月，第一台打印机。](https://gvd20.github.io/images/responsive/articles/bk-studio/first-printer-480.webp)

![后来，iPad Kiosk 和逐渐丰富起来的打印区域](https://gvd20.github.io/images/responsive/articles/bk-studio/printing-area-480.webp)

![通过 April Tag 识别工具是否放置稳妥](https://gvd20.github.io/images/responsive/articles/bk-studio/april-tools-480.webp)

![“小黑店” 的品牌 Logo 和 Mockup 设计](https://gvd20.github.io/images/responsive/articles/bk-studio/brand-mockup-480.webp)

![Kiosk 上的交互 UX](https://gvd20.github.io/images/responsive/articles/bk-studio/kiosk-ux-480.webp)

**2023 年 10 月，第一台打印机。**

后来这个角落逐渐变得更丰富，塞进了能覆盖更多业务需求的设备，也塞进了我一些实验性的想法：

打印机从一台变成多台，喷墨机被分工，激光机承担大批量黑白任务，店内标识语言变得更成熟，服务器换代，承重货架被塞进床后的狭窄空间；门外多了海报、文件筐和自助说明，桌面上出现了固定位置的订书机、推夹器和固体胶，旁边又多了一台 iPad Kiosk。

再后来，我给打印店设计了一整套自动化后台程序。那台 iPad 知道哪台打印机正在工作、哪一份文件正在排队、哪台机器缺纸了，甚至有人把订书机拿走了会提醒他放回。空气净化器会跟随激光机打印负载改变工作模式；夜里暂停的打印任务可以由现场用户重新放行；屏幕上的 Live 2D 角色会随着通知和弹窗改变视线；打印完成以后，它还会主动询问用户有没有遇到问题。

![最初的打印角落](https://gvd20.github.io/images/responsive/articles/bk-studio/first-corner-480.webp)

2023秋季

![新增货架后的打印区域](https://gvd20.github.io/images/responsive/articles/bk-studio/shelf-480.webp)

2024夏季

![添置了打印机和 3D 打印机](https://gvd20.github.io/images/responsive/articles/bk-studio/expanded-480.webp)

2024年秋季

![逐渐完整的打印区域](https://gvd20.github.io/images/responsive/articles/bk-studio/complete-480.webp)

2025年秋季

**打印店三年以来的进化。**

以上这些都不只是一个 Demo 作品。

从 2023 年 10 月 30 日到 2026 年 9 月 15 日，**截止我写这篇博客的时间，BK_STATION 在接近三年、六个学期里累计产生了约 49,818 个订单、98,494.05 元营业额，消耗近 27 万张 A4 纸。**当然这谈不上什么正经的商业项目，但这个规模已经足够大到让许多抽象的问题变得具体：高峰排队，纸用完了，文件找不到，公共工具被拿走不放回来等等……因此一些设计可以真实地反馈在真实的运营上。

这个名叫 **BK_STATION** 的小店，算是我大学期间一个非常特别的试验场，我头一回将自己的想法付诸到真实的运营实践中，也第一次亲眼看见它们与真实商业行为之间的化学反应。

与此同时，我还在做另一个全新的尝试：让打印回到它最自然的交互方式——聊天。

![BK_Studio 的 UI 方案： 主页为单页设计，刻意只提供对话入口。](https://gvd20.github.io/images/responsive/articles/bk-studio/studio-home-375.webp)

![BK_Studio 的 UI 方案： 上滑展开的订单列表。](https://gvd20.github.io/images/responsive/articles/bk-studio/studio-orders-375.webp)

![BK_Studio 的 UI 方案： 文件上传和输入。](https://gvd20.github.io/images/responsive/articles/bk-studio/studio-upload-375.webp)

![BK_Studio 的 UI 方案： 文件修改、下单、格式控制都在对话中进行。](https://gvd20.github.io/images/responsive/articles/bk-studio/studio-dialogue-1-375.webp)

![BK_Studio 的 UI 方案： 文件修改、下单、格式控制都在对话中进行。](https://gvd20.github.io/images/responsive/articles/bk-studio/studio-dialogue-2-375.webp)

![BK_Studio 的 UI 方案： 订单详情页。](https://gvd20.github.io/images/responsive/articles/bk-studio/studio-detail-375.webp)

滑动翻页

**BK_Studio 的 UI 方案：** 主页为单页设计，刻意只提供对话入口。

**BK_Studio 是我正在开发的一套AI原生的打印平台**，它回答了这段经历接下来要面对的问题：如果我自己重新从头设计一套打印服务，我想让它变成什么样？而我的回答是，让“发文件、说需求、确认订单、完成打印”变得和找一个真人老板帮忙一样自然，同时保留自动化系统的效率、确定性和可扩展性。

目前 BK_Studio 已经完成了产品设计和前后端开发，能跑通整个“通过Agent打印的流程”，并准备开始上线运营。

这个项目很长，跨越了三年的各种细节。我希望能借这篇博客，记录下整个经营过程的思考、想法和实践。我写成了下面的三个部分，如果你有兴趣听我唠嗑，**可以选择感兴趣的部分阅读：**

[Part I

### 记一家宿舍角落 逐渐生长的打印店](https://gvd20.github.io/bk-station/part-i/)[Part II

### 一台老 iPad 上的 Kiosk 系统设计](https://gvd20.github.io/bk-station/part-ii/)[施工中

Part III

### BK_Studio，建立在 对话上的 AI 打印产品

施工中](https://gvd20.github.io/bk-station/part-iii/)

## 致谢

最后也想感谢一些在这三年里帮过小黑店的人。

- 感谢「派蒙云印」的豆豆学长。开店初期帮我宣传，也分享了不少运营经验和资源，让小黑店最开始积累客户顺利了很多。

- 感谢我的三位舍友。除了愿意让我在宿舍里放下这一整套打印设备，我不在的时候，他们也经常帮忙照看机器、处理一些日常事务。这个店能在宿舍里一直开下去，本身就离不开他们的配合。

- 也感谢校园打印店交流群里的同行们。三年里大家聊过设备、耗材、平台，也交流过不少实际经营中遇到的问题，很多经验都让我少走了弯路。

- 最后，感谢所有在 BK_STATION 小黑店下过单的同学。它能连续运行近三年，说到底还是因为一直有人愿意来这里打印、再回来打印，也愿意把它推荐给身边的人。
