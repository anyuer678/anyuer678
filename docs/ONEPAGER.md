# Yuer / anyuer678 · 项目一页纸（诚实版）

> 用途：面试 / 主页 / 自述材料  
> 数据基准：GitHub 公开仓 + CI 证据（2026-09）  
> 状态标签：`portfolio` 作品集 · `local-tool` 本机工具 · `engine` 引擎/库

---

## 我是谁

软件工程向个人开发者，5 个月内完成 **27** 个公开仓：从 OJ 判题沙箱、Agent Runtime、组件库到本机密钥工具。  
近期工作重点不是堆功能，而是：**可验证的安全边界、诚实的能力声明、可复跑的 CI**。

---

## 三个最硬的项目

### 1. PolycodeHub — 全栈 OJ（`portfolio`）
- **技术**：Next.js + Express 网关 + Spring Boot 认证 + FastAPI 判题 + RabbitMQ + PostgreSQL/Redis
- **亮点**：进程级沙箱（setuid + rlimit + seccomp 黑名单 + env 清洗）；**fail-closed**（无 netblock 拒判）
- **工程**：prod compose 不对宿主暴露 DB/MQ；FIX_LOG 源码回归 + 沙箱对抗 CI（**6 PASSED**）
- **边界**：黑名单隔离 ≠ gVisor/多租户；测试与生产镜像说明见 `docs/JUDGE_PRODUCTION_IMAGE.md`
- **链接**：https://github.com/anyuer678/polycodehub

### 2. Lumen — 个人 Agent Runtime（`portfolio`）
- **技术**：Go + React，Memory → Reasoning → Tools → Action
- **亮点**：Token 哈希、权限分级、确认流、审计；**空 scopes fail-closed**、confirm 需 `confirm:approve`
- **边界**：字符串 shell + 黑名单仍无法替代 OS 沙箱；默认仅本机
- **链接**：https://github.com/anyuer678/lumen

### 3. DSH LogTimeline — 日志时间查询插件（`engine`，★3）
- **亮点**：中文自然语言时间 → 日志过滤；VENDORED 纪律、框架无关核心、输出契约清晰
- **定位**：全账号工程纪律标杆（文档 + 测试 + 插件化）
- **链接**：https://github.com/anyuer678/dsh-logtimeline

---

## 本机工具链（`local-tool`）

| 项目 | 一句话 | 安全要点 |
|------|--------|----------|
| **keyvault** | API 密钥保险箱 | AES-256-GCM + scrypt；Web step-up；CLI 限速 |
| **voiceconsole** | 语音 MCP 控制台 | 确认权在本机 UI；路径沙箱；默认 TTS 不出网 |
| **picren / stargrave** | 图片整理 / star 清理 | 默认 dry-run / Token 走 env |

---

## 前端与素材

| 项目 | 说明 |
|------|------|
| **kb-ui** | Vue3 组件库，约 73 组件 / 46 主题；npm **kb-ui-vue**；发布策略 Path A |
| **design-assets** | 24 风格 AI 素材骨架 + 画风纪律 + 视觉圣经摘要（CC0） |
| **yuer.dev** | 作品集站点；各项目含深度复盘 |
| **chatez** | 暖色书房 AI 工作台（视觉圣经：禁赛博换皮） |

---

## 近期质量动作（可核验）

- 安全：lumen 权限硬化 PR、voiceconsole 确认权拆分、keyvault step-up、polycodehub prod compose
- 防假绿：CI 硬门禁（pattern-scan / sandbox passed≥4）；`VERIFY_TRUTH.md` 真伪审计
- 声明诚实：Profile 状态标签；DI collector 未交付已标明；evocode 定位 local-tool
- 依赖：polycodehub js-yaml Dependabot high → **fixed**
- 手册：`ACTIONS_HANDBOOK.md`（如何看历史红 vs 当前绿）

---

## 我怎么谈边界（面试可用）

1. **不吹生产**：作品集不等于上线产品；沙箱有明确非目标  
2. **CI 绿 ≠ 全绿产品**：区分本地可证伪测试 vs 历史 run  
3. **安全是过程**：scope/确认/路径沙箱/审计，而不是一句「加密了」  
4. **素材与产品画风分离**：文档可用素材库，产品 UI 遵循视觉圣经  

---

## 联系与仓库

- GitHub：https://github.com/anyuer678  
- 站点：https://anyuer678.github.io/yuer.dev/  
- 素材预览：https://anyuer678.github.io/design-assets/  

---

*本文与 `FINAL_ACCEPTANCE_REPORT.md` / `VERIFY_TRUTH.md` 一致；不声称未验证的生产指标。*
