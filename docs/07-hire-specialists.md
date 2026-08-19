# 07. 雇专家，别养一个万能工

**结果：并列几个 bot，各守一块。记忆分开，问责分开，其中一个变强不会把另外两块带糊。**

## 目标

并行多个 bot，按**领域**拆，不按任务大小拆。只想收据的 Expense Manager 会变强；同时兼顾报销、招聘和外发的万能工，三件事都会更差。

SpaceXAI 一侧的用法：销售外达、市场、办公室运营、修 bug，各是各的 bot。

## 做法

一个人起步的编制：

| 职位 | 管什么 | 默认停线 |
| --- | --- | --- |
| Chief | 分诊、缺人时协调 | 不亲自发信、不碰钱 |
| Inbox Manager | 早间分拣、草稿、截止日期 | 只起草，不发送 |
| Expense Manager | 收据、入账、缺口 | 不付款、不改额度 |
| Sales Outbound / Talent Scout（可选） | 名单、草稿、研究 | 队列停在「待你点发送」 |

真实编制里还会再拆出「对外说话」的专家。ThursdAI 里 Shub 的 **Yapper** 只学他的短信 / Slack / 邮件口吻；House Hunter 找到房源后 @ Yapper 去问照片，Yapper 起草、发送、回传。口吻和找房是两件事，所以是两个职位。

Alex 一侧能看见的名字：Chief of Staff、DeepSeek Drop Watch、ThursdAI Producer、Social Scheduler、Guest CRM EM、ThursdAI Site Fixer。Shub 一侧：House Hunter、Yapper、Sand Outreacher、Taskmaster、People Person、Here to Deescalate。名字都像岗位，不像 `helper-3`。

新领域出现再雇，不要给老 bot 加头衔。拆分信号：

- 你开始说「对了，你也顺便看一下招聘」
- 同一条线程里出现两套口吻、两套停线
- 复盘时说不清是谁写坏了那封草稿

## 为什么重要

记忆是资产，也是污染源。专家只吸收本领域的纠偏；万能工把报销口径和销售口径搅在一起。问责也需要名字：群里说「Inbox 去起草，Expense 去对收据」，比「你去处理一下」可执行。

## 反例

- 按「小任务 / 大任务」拆 bot。小任务没有领域，记忆攒不起来。
- 十个 bot 都叫 Assistant 1…10。没有职位就没有章程。
- 先雇 20 个，再想停线。编制可以长到 10–20，但每一个都要先有 [章程](../playbooks/charter-template.md) 和 [审批线](09-approval-line.md)。
