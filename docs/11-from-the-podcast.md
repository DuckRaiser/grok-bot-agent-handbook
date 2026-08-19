# 11. 播客里多出来的实操

**结果：10 步之外，能直接抄的现场例子。来源是推文挂的 ThursdAI（约 31 分钟），主讲 Shub Gaur（Cursor / SpaceXAI）和 Alex Volkov。**

教程写原则。这段写他们当场跑过的编制、开火条件和停法。模型评测、价格、Windows 排期不收——那是产品新闻，不是组队技巧。

## 怎么进得去

免费试用先跑。付费入口在演示里被点名的是 Cursor Ultra、Grok Super Heavy、Teams Premium。当时是桌面 + iOS，没有 Android。每人一台常驻云电脑（他们叫 Hermes），合上笔记本任务不会死；需要时也能切回本机。

企业电脑不准跑本地 agent 时，Cursor 若已被 IT 批准，Grok Bot 的 Slack 等连接可以跟着过。这是权限继承，不是绕过安全。

训练数据默认不交。要分享必须在设置里自己勾。

## 现场编制（按领域，不按任务大小）

| 职位 | 当场在干什么 | 停线 |
| --- | --- | --- |
| Chief of Staff | 扫收件箱、分诊、把活甩给对的专家 | 自己不外发、不公开贴 |
| House Hunter | 每 6 小时扫 Redfin / Zillow / StreetEasy，对照手绘地图 | 不付款、不提交看房申请除非你点头 |
| Yapper | 学你的口吻；被其他 bot @ 去对外说话 | 发送仍走审批 / Auto-review |
| DeepSeek Drop Watch | 过夜盯发布，许可一出就往指定 Slack 线程丢链接 | 公开帖被 Auto-review 拦住，等你 OK |
| Guest CRM EM | 从往期节目、嘉宾表、多邮箱邀请信拼出 CRM（Alex 说约 1.5 小时） | 不擅自给嘉宾发信 |
| ThursdAI Site Fixer | 在对话里拉起 Cursor cloud agent，开 PR | 合并仍是你的事 |
| Social Scheduler / Producer | 节目运营侧的常驻活 | 对外发布先停 |

搬家身份可以一句话带走（Alex 从旧 Hermes 迁 Chief）：

```
Hey, here's the most important things that I already know.
From you, do the same.
```

## 三个值得抄的开火条件

**找房（Shub，带数字，带地图图）**

每 6 小时扫新盘。租 <4.5k，买 <1.3M，HOA 不能超过 500，一室起、每间卧室尽量不超过 450k，卧室数 ≈ 卫生间数，要大窗、宠物友好。地图当图片丢给它，当「大致想住的范围」，不是精确定位。遇到 Zillow 验证码：它停、丢截图、你接管远端桌面、解开、交回去。完整英文见 [housing-sweep.md](../playbooks/housing-sweep.md)。

**过夜盯发布（Alex）**

```
I know DeepSeek is about to drop. I'm going to sleep.
In this Slack thread, tell people when the license drops.
```

链接随后被撤，有人骂它幻觉。它回：我看到的时候链接还在。过夜 bot 要能自证「我当时看见了什么」，不能只丢一个 URL。

**衣服挂售（Shub）**

把姐姐旧衣服的照片交给一个 bot：识别、上架、跟买家谈。端到端，人只在收款 / 成交这种不可逆点进场。

## 他们当场强调的三句

1. 这些不是 ChatGPT 对话。每个 bot 有你看不见的独立记忆。要喊谁，就 @ 谁（「tag the yapper」）。
2. 密钥走密文框，不进聊天。验证码 / 2FA / 付款：接管桌面，做完交还。
3. Auto-review 是审批线的产品形态。Alex 的 Drop Watch 写出过：`Slack post needs your OK -- Auto-review blocked sending as you.` 可逆的做完，对外的停。

Grok Bot 还能在对话里拉起 Cursor cloud agent（用你的 Cursor 额度，模型可以不是 Grok），卡片上有 View PR / Open in Cursor。这是「专家再雇专家」，编制仍然按领域拆：Site Fixer 管站点，不负责找房。
