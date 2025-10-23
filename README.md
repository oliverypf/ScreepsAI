# ScreepsAI

这是一个 Screeps AI 项目骨架（TypeScript），包含构建与自动部署到 Screeps 官方服务器的 GitHub Actions 配置。

快速开始
1. 在 GitHub 仓库中创建以下 Secrets（Settings → Secrets and variables → Actions）:
   - SCREEPS_TOKEN （推荐）
   - SCREEPS_BRANCH （要上传到的 Screeps 分支，例如 "default"）
   - SCREEPS_HOST （可选，默认 screeps.com 或 ptr.screeps.com）

2. 在本地或通过 GitHub 推送本仓库文件到 main（或你偏好的分支）。
3. 每次 push 到受监控的分支（例如 main）时，Actions 会自动构建并上传代码到 Screeps。

说明
- 不要在仓库或聊天中明文保存 token；请使用 GitHub Secrets。
- 如果你希望自动把不同分支部署到正式服/测试服，请告诉我分支策略，我会调整 workflow.
