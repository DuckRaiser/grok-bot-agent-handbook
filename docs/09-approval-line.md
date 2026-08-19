# 09. 画清审批线

**结果：可逆的事做完再汇报；不可逆的事排队等你。Sales Outbound 可以是 36 封草稿、0 封已发送。**

## 目标

Bot 把活做完，只在「需要批准」时回来。你必须定义什么叫需要批准。

这条线**不是任务大小**。是**可逆性**。

| 自己做完 | 停下来给你 |
| --- | --- |
| 起草、归档、打标签、摘要、研究、准备 | 外界看得到的动作 |
| 对账、整理、排队 | 动钱、锁价 |
| 一切能很快撤回的 | 不能收回的删除、公开、签约 |

## 做法

把下面这段放进每个会对外或会碰钱的 bot（完整版：[approval-policy.md](../playbooks/approval-policy.md)）：

```
// finish these alone, always
draft · file · tag · summarize · research · prepare · reconcile
 everything reversible. don't ask, just do it and log it.

// park these for me, always
send anything to a person outside the company
spend or move money, or commit to a price
publish anything public
delete anything that isn't obvious junk
sign up for, agree to, or accept any terms

// when unsure
If you can't undo it in under a minute, park it and ask.
```

不确定时用一分钟法则：一分钟内撤不掉，就停，问你。

产品里这条线常常长成 Auto-review：bot 准备好对外动作，系统拦住，它回来写一句 `needs your OK`。你点头才发出去。过夜盯发布可以自动发现链接，公开贴到 Slack 仍要你 OK。

Sales Outbound 的合格形态：研究、个性化、排队全做完，发送键在你手上。36 drafts queued, 0 sent——可逆的都做了，不可逆的一封都没动。

## 为什么重要

停线按大小画，你会在「小额付款」「短邮件外发」上不断被偷袭。停线按可逆性画，bot 才敢在你睡觉时把能做的做完，又不会替你签署世界。

## 反例

- 「金额小于 50 就直接付。」小，但不可逆。
- 「口吻听起来没问题就发送。」发送是对外事实，不是文风问题。
- 只写 park 列表，不写 finish 列表。它会为打标签来烦你，专家变成秘书。
