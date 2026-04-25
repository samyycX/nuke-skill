---
name: nuke
description: “原子弹爆炸”式的对项目进行介绍和宣传
compatibility: opencode
---

# 原子弹爆炸.SKILL

## 约束
全程使用中文。

## 触发条件

- `/nuke {BATCH_COUNT}` 使用这个指令触发一次生成流程。BATCH_COUNT是用户传入的可选参数（注意/nuke可能被软件吞掉，如果用户输入纯数字也算）。

---

## 引用

以当前 SKILL.md 所在文件夹为根目录，存在以下你可以引用的文件:
- `./references/summarize.agents.md`
- `./references/zhihu.agents.md`

## 工作内容
规定 BATCH_COUNT 为全局变量，你后续的流程要用到。如果用户没有指定BATCH_COUNT，则从1-10中随机挑选一个数字设置为值。

当用户触发生成流程时，你需要按照以下流程逐步进行。

1.  访问 `references/summarize.agents.md`，并启动Summarize Agent

    根据此文件的内容，启动Summarize的agent。

2.  访问 `./references/zhihu.agents.md` 

    访问 `./references/xiaohongshu.agents.md`
    
    访问 `./references/paper.agents.md`

    访问 `./references/qq.agents.md`

    访问 `./references/short-video.agents.md`

    同时启动以上 agent。