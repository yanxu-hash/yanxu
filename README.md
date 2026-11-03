# yanxu

这个仓库由 **dsh-superagent**（DeepSeek Harness 的 super agent 架构）托管：
在 Issue 或 PR 评论里 `@yanxu-hash` 提出需求，编排器会评估、建 Ticket，
再由独立 Session 在自己的 worktree 里执行并回贴结果。

## 结构

```
.
├── README.md
└── docs/
    └── superagent.md   # 本仓库与 super agent 的约定
```

`docs/` 目录用于存放本仓库的说明文档，目前只有 `superagent.md` 一个文件，记录本仓库与 super agent 的协作约定。后续新增的细节说明也统一放在这里，让 README 保持精简。

## 约定

- 分支：`agent/<ticket>`，由执行器自动创建
- 提交：执行器署名，评审后再合并
- 允许名单、规则与执行环境：见面板 `http://127.0.0.1:3082`

## 许可

私有仓库，未授权。

## 用途

本仓库用于演示 **dsh-superagent** 的完整工作流程：从 Issue 或 PR 评论提出需求，到编排器评估并创建 Ticket，再到独立 Session 执行并回贴结果。它同时用来验证规则匹配、任务路由与评审合并等环节，因此仓库内容保持精简，只保留演示所需的部分。
