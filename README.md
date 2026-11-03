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

## 约定

- 分支：`agent/<ticket>`，由执行器自动创建
- 提交：执行器署名，评审后再合并
- 允许名单、规则与执行环境：见面板 `http://127.0.0.1:3082`

## 许可

私有仓库，未授权。
