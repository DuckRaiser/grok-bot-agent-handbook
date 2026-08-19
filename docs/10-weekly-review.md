# 10. 每周复盘，狠删

**结果：日历上有 15 分钟。每条 routine 过三问。活着的自动化都是你仍会想念的。**

## 目标

自动化会悄悄腐烂：布局改了，routine 开始产垃圾，三周没人发现。防止的方法不是再加监控产品，是每周问三次：

1. 它跑了吗？
2. 产出真的对吗？
3. **杀掉我会不会想念它？**

第三问最要紧。默认趋势是堆一堆半有用、没人删的自动化。

## 做法

1. 日历固定 15 分钟，不要「有空再看」。
2. 先让 bot 自己交卷——线程在它们那边。提问原文：

```
List every routine you ran this week. For each one:

 - how many times it fired
 - what it produced
 - anything it skipped, failed, or had to guess at
 - anything you parked for me that I never answered

Then tell me which one you think is least useful, and why.
```

3. 你再**亲手抽查每条 routine 的一份产出**。只看它们的自评，等于没有复盘。
4. 对「杀掉也不会想念」的：停掉，不要改参数续命。章程过时就改章程。

完整提问在 [weekly-review.md](../playbooks/weekly-review.md)。积压未答的 park 项，优先于新雇 bot。

## 为什么重要

技能已经从「怎么措辞」变成「我究竟在委托什么，权限到哪结束」。这是管理问题。不管，编制会从 3 涨到 20，同时正确率往下掉。

推文里的方向（转述）：有人跑 10–20 个 GrokBot，覆盖约 90% 例行，并用 Chief of Staff 盯住其余 bot。那是复盘之后的编制，不是第一周的目标。

## 反例

- 只看「跑了多少次」。次数不是质量。
- 出错就加一条补丁 prompt，从不删。腐烂被补丁盖住。
- 抽查时只看成功案例。先看它承认猜过、跳过、失败过的那些。
