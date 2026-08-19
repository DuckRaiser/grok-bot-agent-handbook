# Grok Bot Agents 实战手册

大多数 AI 工具在等你开口。Grok Bot 反过来：每个 bot 有自己的云电脑，能登录你的工具，合上笔记本之后还在干活。这份手册把公开教程改写成可执行的中文 playbook——停下来写提示词，开始按职位委托工作。

> **来源（整理改写，非原文搬运）**
>
> - 推文：[Grok Bot Agents / 10–20 agents](https://x.com/0xCodez/status/2090043252669812886) · @0xCodez · 2026-08-19
> - 原文：[Grok Bot Agents: how to automate your life in 10 Steps (Full-tutorial)](https://x.com/i/article/2089655442657910784) · Codez (@0xCodez) · 2026-08-18
> - 作者站点：[movez.substack.com](https://movez.substack.com/)
>
> 模板保持英文原文，方便直接粘贴。讲解是中文改写。版权仍属原作者。详见 [SOURCES.md](SOURCES.md)。

## 核心原则

- **委托，不是提问。** 技能从「怎么措辞」变成「到底把什么交出去，权限到哪停」。
- **职位，不是 prompt。** Bot 会留下记忆、守一块地盘；同名线程越用越准。
- **先画停线，再放手。** 会事事请示的 bot 没用；从不请示的 bot 危险。停线按可逆性画，不按任务大小。
- **连一次，全员共用。** 账号连接挂在账户上，不是挂在单个 bot 上。爆炸半径等于你以后会建的每一个 bot。
- **交会话，不交密码。** 登录墙交给你点，bot 拿到的是 session，不是 secret。
- **演示一次，批准再跑。** 先做给你看，再「每周再来一次」。自动化是批准刚才那次，不是去搭工作流编辑器。

## 目录

1. [装好，先见 Chief](docs/01-install-meet-the-chief.md)
2. [给职位，不要给一段 prompt](docs/02-job-title-not-prompt.md)
3. [工具只连一次](docs/03-connect-tools-once.md)
4. [交登录，别把密码贴进对话](docs/04-handoff-login.md)
5. [演示一次，不要解释两遍](docs/05-show-once.md)
6. [变成你不在也跑的 routine](docs/06-routines.md)
7. [雇专家，别养一个万能工](docs/07-hire-specialists.md)
8. [把他们拉进群聊](docs/08-group-chat.md)
9. [画清审批线](docs/09-approval-line.md)
10. [每周复盘，狠删](docs/10-weekly-review.md)
11. [播客里多出来的实操](docs/11-from-the-podcast.md)

**可直接粘贴的 playbook**

- [职位章程 Charter](playbooks/charter-template.md)
- [审批策略 Approval](playbooks/approval-policy.md)
- [Routine 配方](playbooks/routine-recipes.md)
- [每周复盘提问](playbooks/weekly-review.md)
- [找房扫盘](playbooks/housing-sweep.md)

## 怎么用这份手册

1. 先读 [01](docs/01-install-meet-the-chief.md) 和 [02](docs/02-job-title-not-prompt.md)。装上桌面端，给第一个 bot 一个真实职位和停线。
2. 从 `playbooks/` 抄一份章程，改成你的 Inbox / Expense / Outbound。英文模板原样粘贴，中文只改你自己的边界。
3. 再读 [06](docs/06-routines.md)–[10](docs/10-weekly-review.md)。先跑通一个可检查的小任务，再上日程和触发器，最后才组群、画审批线、每周砍掉没用的自动化。

下一步九步的目标不是「测模型聪不聪明」，是学会把更大的活交给同一个职位。

## 许可

这里是个人使用的笔记和 playbook。原文版权属于 [@0xCodez](https://x.com/0xCodez)。不要把这份手册当成原文副本去再分发。
