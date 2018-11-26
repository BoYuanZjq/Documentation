
---
title: Dashboard 操作指南
description: 
platform: All Platforms
updatedAt: Mon Nov 26 2018 06:48:54 GMT+0000 (UTC)
---
# Dashboard 操作指南
欢迎使用 Agora Dashboard。在这里，你可以查看频道用量，追踪通话质量，管理项目和权限，以及获取 Agora 技术支持。

使用 Agora Dashboard 前，你需要创建 Agora 账号，详见 [注册与登录](../../cn/Interactive%20Broadcast/sign_in_and_sign_up.md)。如需找回账号密码，详见 [找回密码](../../cn/Interactive%20Broadcast/sign_in_and_sign_up.md)。

## 功能简介

<table>
<tr>
<th>功能</th>
<th>简介</th>
</tr>
<tr>
<td>查看用量</td>
<td>查看特定时间段内语音及视频通话时长，自助统计通话时长及费用。</td>
</tr>
<tr>
<td>追踪质量</td>
<td>通过图表全方位监控、分析并诊断各种实时网络产品的用户使用指标及设备性能，自助定位问题。</td>
</tr>
<tr>
<td>管理项目</td>
<td>创建并管理项目，获取项目 App ID 和 App Certificate。</td>
</tr>
<tr>
<td>管理成员</td>
<td>在项目中添加并管理成员角色，设置角色对应的项目管理权限。</td>
</tr>
<tr>
<td>提交与查看工单</td>
<td>在开发中遇到问题时，查询解决方案以及获取 Agora 技术支持。</td>
</tr>
<tr>
<td>使用 RESTful API</td>
<td>使用服务端操作的 API，实现从服务端踢人、用量查询、查询在线信息等功能。</td>
</tr>
<tr>
<td>其他功能</td>
<td>通过 Dashboard 顶栏按钮，进行账号相关设置，进入开发者社区。</td>
</tr>
</table>

## 查看用量

点击左侧导航栏**用量 > 用量统计**，进入用量统计页面，查看特定时间段内语音及视频通话时长，自助统计通话时长及费用。

![](https://web-cdn.agora.io/docs-files/1542965752366)

如上图所示，选择频道和周期后，可查看该频道在所选周期内的用量统计。该图展示频道中包括 [主播](../../cn/Agora%20Platform/terms.md) 和 [观众](../../cn/Agora%20Platform/terms.md) 在内的所有用户的通话用量，其中，

* **音频总量**：该频道在所选周期内音频通话的总分钟数。如图所示该频道在 2018 年 11 月 16 日至 22 日期间的音频通话的总分钟为 618958 分钟。
* **SD 视频总量**：该频道在所选周期内视频分辨率小于 360p 的标清视频通话的总分钟数，目前视频通话质量均按 HD 视频总量计费。
* **HD 视频总量**：该频道在所选周期内视频分辨率介于 360p 和 720p 之间的高清视频通话的总分钟数。如图所示该频道在 2018 年 11 月 16 日至 22 日期间的 HD 视频通话的总分钟为 145964 分钟。
* **HD+ 视频总量**：该频道在所选周期内视频分辨率大于 720p 的高清视频通话的总分钟数。如图所示该频道在 2018 年 11 月 19 日的 HD+ 视频通话的总分钟为 1328 分钟。

> 关于音视频对应的计费方式，详见 [计费](https://docs.agora.io/cn/Agora%20Platform/billing_faq)。

## 追踪质量

你可以通过 Agora Dashboard 中的水晶球对 SDK 的通话质量进行跟踪，从图表中获取每次通话全链路丰富的数据，包括设备状态、用户行为、音视频发送/接收码率、音视频卡顿情况和网络丢包率。

点击左侧导航栏**水晶球 > 通话调查**，进入通话调查页面。

使用 SDK 后，你可在本页面选择**项目**和**时间段**、输入**频道名称**或 **UID** 查看通话质量，详见 [水晶球教程](https://dashboard.agora.io/analytics/call/tutorial?_ga=2.197716463.1125435494.1542623251-764614247.1539586349)。

![](https://web-cdn.agora.io/docs-files/1542771871816)

## 管理项目

点击左侧导航栏**项目 > 项目列表**，进入项目列表页面，根据需求创建项目、管理项目、获取 App ID 及 App Certificate 等。

#### 创建项目并获取 App ID

详见校验用户权限中的 [获取 App ID](../../cn/Interactive%20Broadcast/token.md)。

> 对于已创建的项目，可根据创建时间、项目名和项目状态等对项目进行排序，也可通过输入项目名进行查找。
> 
> 若需要修改项目名称，可点击**编辑**进行修改或添加录制服务器 IP 或域名。

#### 获取 App Certificate

详见校验用户权限中的 [获取 App Certificate](../../cn/Interactive%20Broadcast/token.md)。

#### 踢人

如果想从 App 中踢出某个用户，可以选择使用 Dashboard RESTful 的 [服务端踢人 API](https://docs.agora.io/cn/Interactive%20Broadcast/dashboard_restful_live?platform=All_Platforms#5-api)，也可以联系 Agora 技术支持开通权限后，直接在**项目**中进行配置。


## 管理成员

点击左侧导航栏**成员管理**，进入成员管理页面。

![](https://web-cdn.agora.io/docs-files/1542624935837)

你可在本页面进行以下操作：

* 点击**添加成员**，设置不同的用户权限，进行协同管理。受邀者将收到邀请邮件。
* 点击**编辑**，根据需求重新设置该成员的角色和权限。
* 点击**重置成员密码**，该成员会收到密码重置邮件。
* 点击**删除**，将不需要继续参与该项目的成员移出。

#### 权限说明

不同角色对应的不同功能权限，其中，

* 管理员：拥有最大权限，能够查看用量、水晶球及项目详情，并负责项目管理和成员管理。
* 产品/运营：仅能查看用量，其他功能对其不开放。
* 技术支持/运维：仅能使用水晶球，其他功能对其不开放。
* 工程师：能够使用水晶球，有权查看项目和管理项目。

你也可以根据所需自定义团队成员的角色和权限。

## 提交与查看工单

你在产品使用过程中如有任何疑问，可通过工单获得解答。操作步骤如下：

1.点击页面上方**支持 > 提交工单**按钮，输入问题或关键字，查看关联内容。
2.如果现有内容无法解决你的问题，可选择类别，输入问题，提交工单。Agora 技术支持将与你联系。
3.点击**支持 > 查看工单**，查看工单处理进度。

![](https://web-cdn.agora.io/docs-files/1542963447515)


## 使用 RESTful API

Agora Dashboard 提供服务端操作的 API，实现从服务端踢人、用量查询、查询在线信息等功能。

点击页面右上角**用户名 > RESTful API**按钮，获取使用 Agora RESTful API 所需的 Customer ID 和 Customer Certificate。具体操作请见 [RESTful API 文档](../../cn/Interactive%20Broadcast/dashboard_restful_live.md)。

## 其他功能

### 修改账号设置

点击页面右上角**用户名**，可进行以下操作：
* 修改个人信息；
* 修改密码；
* 切换界面语言和 Agora 简讯语言。

### 进入开发者社区

点击页面上方**社区**按钮，进入 Github、在线论坛和微信公众号等开发者社区，与全球开发者进行交流互动。
