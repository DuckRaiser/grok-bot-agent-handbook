# 06. 变成你不在也跑的 routine

**结果：日程或触发器扛着跑。你批准的是刚刚发生过的那一次，不是去搭工作流画布。**

## 目标

两个开火条件，用说话设定，没有工作流编辑器：

- **Schedule**：准时来找你（早 7 点简报、周五管线、月末报销）。
- **Trigger**：世界变了再动（新 Slack、匹配某种入站邮件、文档被改）。触发器让 bot 像在场，而不只是守时。

走查里，设一条基于触发器的 routine 大约两分钟、一句提示词。

## 做法

先把一次任务做满意。最后补一句：

```
Run this every week.
```

你不是在「搭建自动化」。你是在批准刚才那次，并要求再来。

四种现成配方（英文原样，完整版在 [routine-recipes.md](../playbooks/routine-recipes.md)）：

```
// schedule — the morning brief
Every weekday at 7am, check my calendar, my inbox, and the
#launches Slack channel. Give me one short brief: what's on
today, what needs a reply, what changed overnight.

// trigger — the inbound catcher
Whenever an email arrives from a domain not in my contacts and
it mentions pricing, draft a reply from the template and park it.

// schedule — the weekly close
Every Friday at 4pm, pull the week's receipts from my inbox,
file them, and tell me anything that has no matching invoice.

// the shortcut that creates most routines
Run this every week.
 ^ said right after a task you liked. That's the whole flow.
```

Schedule 适合你已经知道节奏的事。Trigger 适合「这件事出现时我必须在场」。两条都要带 [审批线](09-approval-line.md)：草稿可以自动，外发不能。

## 为什么重要

合上盖子之后还在跑的，不是聊天记录，是 routine。没有开火条件，专家只是一个你得记得去喊的收藏夹。

## 反例

- 还没做成功过一次，先写「每天早上自动处理所有邮件」。你批准的是幻觉。
- 触发条件写成「有需要时」。没有可观察的事件，就没有触发器。
- 一条 routine 同时盯日历、改生产配置、群发客户。开火可以很勤，权限必须很窄。
