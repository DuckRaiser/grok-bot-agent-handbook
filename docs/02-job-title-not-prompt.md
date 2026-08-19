# 02. 给职位，不要给一段 prompt

**结果：一个叫得出职称的 bot，有章程，有停线，你敢让它在你睡觉时继续跑。**

## 目标

Prompt 是一次请求。Bot 是一个**职位**：持续存在、堆积记忆、守一块地盘。你反复回到同一条线程，它才会变好。

名字要像真人能持有的岗位：Inbox Manager、Expense Manager、Talent Scout、Sales Outbound。不要叫 `helper`、`gpt2`、`杂活`。

## 做法

像给新员工做入职简报，写三块，缺一不可：

1. **你管什么**（what you own）
2. **什么样叫做好**（what good looks like）
3. **什么必须先问我**（where you stop）

最后一条边界，才是你能把它丢在后台跑的理由。

尺度：

- 事事请示 → 没用，你还是接线员。
- 从不请示 → 危险。它有自己的电脑，还可能拿着你的登录态。

完整英文章程见 [charter-template.md](../playbooks/charter-template.md)。下面这段原样粘贴，再改名字和边界。

```
You are my Inbox Manager.

// what you own
Triage my email every morning. Archive newsletters and receipts.
Draft replies to anything a client sends. Surface anything
that mentions a deadline, an invoice, or a legal question.

// what good looks like
Inbox at zero by 9am. Drafts sound like me: short, direct,
no "I hope this finds you well". Never more than 4 sentences.

// where you stop
Never send anything. Draft only.
Never archive anything from my accountant or my landlord.
If a message asks for money or credentials, stop and ask me.
```

## 为什么重要

同一职位反复做同一类判断，记忆才有用：你的口吻、谁的邮件不能动、什么叫「像你」。换线程等于换新人。

有章程的 bot 才能在你合上盖子之后继续动。没有停线的 bot，等于把钥匙交给一个热情的陌生人。

## 反例

- 「你是一个有帮助的助手，尽量把邮件处理好。」没有停线，也没有「好」的标准。
- 把招聘、报销、外发销售塞进同一个 Inbox Manager。职位糊了，记忆也糊了。
- 章程写「有疑问随时问我」。等于没有授权。该问的只有不可逆的事，见 [09](09-approval-line.md)。
