# drift-race Constitution

> 漂移赛车 Web 游戏。main = 开发分支；gh-pages = 发布产物同步分支（勿在 gh-pages 直接开发）。

## Core Principles

### I. 静态可玩 (No-Build Playable)
- 发布形态为纯静态站点：打开即玩，无构建步骤、无服务端依赖（工具脚本除外）
- gh-pages 分支只承载可上线产物；一切开发在 main 进行

### II. 性能预算 (Performance Budget)
- 目标 60fps（桌面）；新效果/资源须实测帧率，明显超标先优化再合入
- 资源体积保持轻量：大文件按需加载，不进首屏关键路径

### III. 第三方资产许可登记 (Vendor Licensing)
- vendor/ 下每个第三方库/素材须可追溯（名称+版本+许可证）
- 引入新库须记录理由；能复用既有依赖就不新增

### IV. 小步可回退 (Small Reversible Steps)
- 每次提交单一主题、可独立回滚；玩法/操控类改动须附一次实机自测记录

## Governance
- 修订随 commit 说明理由，版本与日期更新

**Version**: 1.0.0 | **Ratified**: 2026-10-02 | **Initial draft**: 基于仓库现状证据起草（AI-assisted, 鲸）
