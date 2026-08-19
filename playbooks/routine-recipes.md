# Playbook：Routine 配方

先做成功一次，再设开火条件。两种：Schedule（守时）、Trigger（在场）。

配套说明：[06 变成你不在也跑的 routine](../docs/06-routines.md)

绝大多数 routine 的创建方式就这一句，说在你刚满意的那次任务后面：

```
Run this every week.
```

## 现成配方（原样粘贴再改频道名 / 时钟）

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

// schedule — overnight watch (swap the event)
I know [THING] is about to drop. I'm going to sleep.
In this Slack thread, tell people when it drops.
Do not invent a link. If the URL later 404s, say what you saw and when.
```

带硬数字的扫盘（每 N 小时、价格上限、不可伪造）见 [housing-sweep.md](housing-sweep.md)。

## 改之前先问自己

- 这一次已经做对过吗？没有就先别调度。
- 触发器的事件外人能不能看见？（新邮件、新消息、文档变更。不是「有需要时」。）
- 自动段是否停在草稿 / 归档 / 通知，而不是发送和付款？
