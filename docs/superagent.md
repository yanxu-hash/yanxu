# super agent 约定

本仓库是 dsh-superagent 的工作对象，以下是它需要知道的约定。

## 收到请求后

1. 编排器读取 Issue / PR 评论，按 Policy 判断是否建 Ticket
2. 执行器为每个 Ticket 创建独立 worktree：`agent/<ticket>`
3. 执行完成后在原始会话回贴结果（PR 或说明）

## 人工介入点

- Policy 允许名单：只有名单内的人能触发工作
- Execution：目录根与 prepare 命令
- Prompts：团队语气、署名、合并条件
