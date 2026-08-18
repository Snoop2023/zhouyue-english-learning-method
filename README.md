# 周越英语学习方法 / Zhouyue English Learning Method

一套自己试出来的英语学习方法。核心只有一句话：

> **大脑不能同时跑多个进程。拆开跑，各自自动化，自然合并。**
>
> The brain can't run multiple processes at once. Split them, automate each, and fluency emerges on its own.

---

## 两篇文档 / The Two Documents

| 文档 | 内容 | Document | About |
|---|---|---|---|
| [周越英语学习法_口语.md](周越英语学习法_口语.md) | 输出倒逼输入的口播循环系统：0 启动、IG 口播素材、learn in public | Speaking | Output-driven speaking loop: zero-threshold start, Instagram clip materials, learn in public |
| [周越英语学习法_阅读.md](周越英语学习法_阅读.md) | 五级骨架递进法：骨架留英文、生词换中文，S1→S2→S3→原文 | Reading | Five-level skeleton-first reading: keep sentence skeletons in English, swap hard words for Chinese, then progressively restore English |

## 口语的 Core Insight / Speaking Core Insight

**学习就是输出：讲不出来，就是没学会。** 所以口语方法从输出端倒推——用输出倒逼输入。素材从一句话开始，启动门槛拉到无限低；自己录口播发到自媒体上（learn in public），真实环境的压力和点赞评论的正反馈，同时到账。

Learning = output: if you can't say it, you haven't learned it. So the method works backwards from output — output drives input. Start with one-sentence clips (near-zero threshold), record yourself and post publicly (learn in public): real pressure and real feedback arrive together.

## 阅读的 Core Insight / Reading Core Insight

读英文又慢又累，因为大脑里有三个进程在同时跑：

1. **结构焦虑**（最大头）——不知道句子多长、什么时候结束，全程绷着神经
2. **被迫串行**——只能一个词一个词读，因为你不知道结构
3. **生词翻译**（最小头）——真的不认识，停下来想意思

Reading English feels slow and exhausting because three cognitive processes run at once: structural anxiety (the biggest load), forced serial reading, and word translation (the smallest load, most overestimated).

**解法：先灭掉最大的那个。** 把生词全部换成中文，只留英文骨架，让大脑一次只干一件事。

**The fix: kill the biggest process first.** Swap all hard words for Chinese, keep only the English skeleton, let the brain do one thing at a time.

最近我又发现：一段纯英文稿，它的英文骨架、英文连接词本身很通顺、很简单，还隐含很多意思；但知识点、难点和关键信息，就用中文翻译。这样中英夹杂读起来速度非常快——**感觉兼顾了中英各自的优点。**

## 配套 Agent Skills / Companion Agent Skills

`skills/` 目录里有两个 skill，装到你的 AI agent 上，直接丢英文材料给它，它按这套方法带你练：

Two skills in `skills/` — install them into your AI agent, then just throw English material at it:

| Skill | 用途 | Purpose |
|---|---|---|
| [skills/skeleton-first-reading](skills/skeleton-first-reading/SKILL.md) | 丢一段英文 → 自动生成 S1/S2/S3 骨架递进版 + 提取骨架做 7-12 场景复现 | Feed it a passage → get S1/S2/S3 progressive versions + skeleton extraction with 7-12 scene variations |
| [skills/sound-loop-speaking](skills/sound-loop-speaking/SKILL.md) | 口语训练：听写→复述引导 + 用你练过的句式生成「你的口吻」的英文材料 | Speaking: dictation→retell guidance + AI-generated material in your own voice patterns |

安装方式（Codex / 兼容 agents）：

```bash
git clone https://github.com/Snoop2023/zhouyue-english-learning-method.git
mkdir -p ~/.agents/skills
cp -R zhouyue-english-learning-method/skills/skeleton-first-reading ~/.agents/skills/
cp -R zhouyue-english-learning-method/skills/sound-loop-speaking ~/.agents/skills/
```

或者直接把 `SKILL.md` 的内容贴给你的 agent 用。

Or simply paste the SKILL.md content to your agent as standing instructions.

## 方法来源 / Origin

这套方法是 2026 年 7-8 月和 AI 对话时一段一段试出来的：先试「原文→中文→中英夹杂」，发现「骨架英文+生词中文」读起来明显更快，追问为什么，方法就是这么长出来的。

This method was discovered through trial and error in conversations with AI (July–August 2026).

## License

MIT — 方法随便用，注明出处即可。
