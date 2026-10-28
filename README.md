<h1 align="center">Hi, I'm Yuer</h1>

<p align="center">
  <em>个人开发者 · 软件工程 · 工具与 AI 相关</em>
</p>

<p align="center">
  <a href="https://anyuer678.github.io/yuer.dev/"><img alt="site" src="https://img.shields.io/badge/%E6%A1%88%E4%BE%8B%E7%AB%99-yuer.dev-8b5cf6"></a>
  <a href="https://github.com/anyuer678?tab=repositories"><img alt="repos" src="https://img.shields.io/badge/public_repos-31-blue"></a>
  <img alt="status" src="https://img.shields.io/badge/portfolio-quality%20pass-lightgrey">
</p>

---

### 关于我

软件工程学生，把想法做成可运行的软件：从本机工具到多服务系统。当前作品集以 **可验证的安全边界** 与 **诚实的能力声明** 为准，而非空泛「平台」叙事。

**状态标签说明**（全仓库统一）

| 标签 | 含义 |
|------|------|
| `local-tool` | 本机单用户工具，默认勿公网 |
| `portfolio` | 作品集/课程旗舰，功能有但不承诺生产 |
| `engine` | 可复用引擎/库，API 可能变更 |
| `archived` | 学习存档，不再维护 |

---

### 核心项目

<table>
  <tr>
    <td width="50%">
      <h3><a href="https://github.com/anyuer678/polycodehub">PolycodeHub</a> <code>portfolio</code></h3>
      <p>全栈在线判题平台（OJ）</p>
      <p><code>Next.js</code> <code>Express</code> <code>Spring Boot</code> <code>FastAPI</code></p>
      <p>四层沙箱（2026-09）：seccomp 黑名单/白名单 + cgroup v2 + ns/jail · RabbitMQ 异步判题 · prod compose 不对宿主暴露中间件</p>
      <p>非生产就绪 · 非多租户容器（自评与未修复项见 THREAT_MODEL）· <a href="https://anyuer678.github.io/yuer.dev/notes/polycodehub-sandbox-notes/">沙箱演进长文</a></p>
      <p>▸ <a href="https://anyuer678.github.io/polycodehub/">在线演示</a></p>
    </td>
    <td width="50%">
      <h3><a href="https://github.com/anyuer678/lumen">Lumen · 流明</a> <code>portfolio</code></h3>
      <p>24/7 个人 AI Agent Runtime（本机）</p>
      <p><code>Go</code> <code>React</code> <code>AI</code></p>
      <p>权限分级 + 确认流 · 空 scopes fail-closed · 威胁模型见仓内 docs</p>
      <p>默认 127.0.0.1 · 勿公网部署 · 独立审计未做</p>
    </td>
  </tr>
</table>

---

### 作品体系（三主线）

> 每条主线与联动关系均可在各仓 README「生态」区块与代码中验证。体系地图见 [yuer.dev/map](https://anyuer678.github.io/yuer.dev/map)。

**① AI Agent 生态**（核心 [lumen](https://github.com/anyuer678/lumen)——24/7 Agent Runtime，内置 MCP 注册与分级权限）

| 项目 | 生态角色 | 描述 |
|------|---------|------|
| [voiceconsole](https://github.com/anyuer678/voiceconsole) | MCP 插件 · 语音入口 | 语音指令 MCP（本机确认权 + 路径沙箱），可注册进 lumen |
| [dsh-logtimeline](https://github.com/anyuer678/dsh-logtimeline) | MCP 插件 · 日志查询 | 中文自然语言日志时间查询（DSH 插件） |
| [keyvault](https://github.com/anyuer678/keyvault) | 密钥设施 | API 密钥保险箱（AES-256-GCM + step-up Web），生态公共前置 |
| [chatez](https://github.com/anyuer678/chatez) | 平级工作台 | Prompt + Skill 的 AI 客户端工作台（纯前端，[在线](https://anyuer678.github.io/chatez/)） |

**② UI / 工程基建**（自建组件库，被生态项目真实消费）

| 项目 | 生态角色 | 描述 |
|------|---------|------|
| [kb-ui](https://github.com/anyuer678/kb-ui) | 组件库 · npm 四件套 | Vue 3 **73** 组件 · 46 主题：[kb-ui-vue](https://www.npmjs.com/package/kb-ui-vue) · [@yuer678/kb-utils](https://www.npmjs.com/package/@yuer678/kb-utils) · [@yuer678/kb-api](https://www.npmjs.com/package/@yuer678/kb-api) · [@yuer678/create-kb](https://www.npmjs.com/package/@yuer678/create-kb)（[在线](https://anyuer678.github.io/kb-ui/)）；**yuer.dev 的作品地图页由其驱动** |
| [yuer.dev](https://github.com/anyuer678/yuer.dev) | 门面 + 作品地图 | 个人作品集 / 数字花园（[在线](https://anyuer678.github.io/yuer.dev/) · [地图](https://anyuer678.github.io/yuer.dev/map)） |
| [design-assets](https://github.com/anyuer678/design-assets) | 设计资产 | AI 设计素材库（24 风格 meta + 画风纪律 + 视觉圣经；[预览站](https://anyuer678.github.io/design-assets/) · [Release v1.0](https://github.com/anyuer678/design-assets/releases/tag/v1.0) 99 文件全集） |

**③ 训练 / 评测平台**（核心 [polycodehub](https://github.com/anyuer678/polycodehub)——四层沙箱在线判题）

| 项目 | 生态角色 | 描述 |
|------|---------|------|
| [codedrill](https://github.com/anyuer678/codedrill) | 离线训练 | SRS 编程训练 · 635 题（多端完成度不一，[在线](https://anyuer678.github.io/codedrill/)） |

**独立作品**（与主线无耦合，诚实单列）

[evocode](https://github.com/anyuer678/evocode) · [developer-intelligence](https://github.com/anyuer678/developer-intelligence) · [desktoppet](https://github.com/anyuer678/desktoppet) · [picren](https://github.com/anyuer678/picren) · [spotlight-wallpaper](https://github.com/anyuer678/spotlight-wallpaper) · [huayinlaoqiang](https://github.com/anyuer678/huayinlaoqiang)（内容封存） · [eclipse-wasteland](https://github.com/anyuer678/eclipse-wasteland)

| 归档 | 状态 | 说明 |
|------|------|------|
| [todo-list](https://github.com/anyuer678/todo-list) / [key-tool](https://github.com/anyuer678/key-tool) 等 | `archived` | 学习仓 / 上游归档；key-tool 为已归档的 API Key 消费网关（替代见 keyvault）；upgrademate / stargrave / ai-toolbox 已于 2026-09 毕业归档（聚焦核心项目） |

### 近期工程重点（A+ 轨）

- 沙箱演进（2026-09）：polycodehub 判题沙箱从 136 行 seccomp 黑名单升级为 **trace 驱动白名单 + cgroup v2 按判题隔离 + NET/PID/MOUNT ns + chroot jail**（PR #18/#19/#20，adversarial CI 实测抓出并修复 12 个真 bug）；[演进长文](https://anyuer678.github.io/yuer.dev/notes/polycodehub-sandbox-notes/)
- 聚焦（2026-09）：作品集瘦身——upgrademate / stargrave / ai-toolbox **毕业归档**，维护精力集中于 polycodehub / kb-ui / lumen / evocode / desktoppet / codedrill；**新仓只作实验登记，不纳入维护承诺**（time-archaeologist / world 为实验仓）；重心转向外部验证
- 安全：lumen 权限硬化、voiceconsole 确认权拆分、keyvault step-up、polycodehub prod compose  
- 诚实：DI / evocode 声明与能力对齐  
- 治理：LICENSE 补齐、威胁模型、Issue 跟踪  
- 质量门禁：keyvault / voiceconsole / dsh-logtimeline / desktoppet 增加 **覆盖率下限**（pytest-cov / vitest coverage，阈值贴当前基线，不造红灯）  
- 素材：[design-assets](https://github.com/anyuer678/design-assets)（文档层引用，不改产品画风）
- 发布：kb-ui npm **四包**（组件库 / 工具库 / 参考后端 / scoped 脚手架 `@yuer678/create-kb`——无 scope `create-kb` 是同名无关项目）；design-assets **Release v1.0**（99 文件样例全集 2048×1152）  
- 门禁与保鲜（2026-09，2026-10 复核）：kb-ui 的四项 required check 实测为 `pattern-scan` / `Lint · Typecheck · Test · Build` / `claims` / `E2E (playground + docs)` / `Visual regression`，其中 `Dependency audit`（`pnpm audit --prod --audit-level=high`）是构建 job 内的步骤，所以「高危阻断合并」成立；案例站（chatez）当前**没有**定时数据刷新 workflow（仓内唯一 cron 是 secret-scan），数据更新走手动流程；27 仓 LICENSE 全覆盖、11 仓已有 SECURITY 与 CONTRIBUTING（扩仓后的许可证现状见下方「合规」条）

**Portfolio quality pass（2026-10）**：安全加固收口。Dependabot 当前 **OPEN = 2**（2026-10-28 逐仓复核：26 个仓开启告警、5 个无依赖清单的仓保持关闭），处置口径如下——

- `extract-zip`（HIGH，GHSA-7pqw-9j4j-h8q3 / GHSA-jmr9-qjv8-65gv）× codedrill、desktoppet：随 **Electron 42** 升级被 `@electron-internal/extract-zip` 取代，告警已消失（npm 上 `extract-zip@2.0.1` 本身仍是漏洞版本、无补丁，所以不是"修好了"，而是换掉了实现）
- `vite` ×8 / `esbuild` ×1 × kb-ui 文档站：9 条已全部消除或缓解，逐条现状写在 [kb-ui 的 SECURITY-NOTES](https://github.com/anyuer678/kb-ui/blob/master/docs/SECURITY-NOTES.md)——vite 四条的影响区间是 `8.3.0–8.3.2` / `8.0.x`，而仓内是 8.3.5；四条 `launch-editor` 由 override 拉到 2.14.2；`esbuild` 由 0.21.5 提到 0.25.12（`docs:build` 13.68s 通过）。唯一保留的钉死是 `vite@^5.4.14 → 5.4.21`：vitepress 1.6.4 的 peer 只到 5.x，解除要等 vitepress 2 GA
- 本轮新开启告警的 8 个仓（LastTap / world / shijing / ziyou-shi / course-design-2026 / wolai-paikebiao / quote-rectifier / cs-notes-public）首次扫描共 **82 条**，已清零 **80**：shijing 24 条（`next` 16.3.1 → 16.4.3，5 条 critical 全消）、quote-rectifier 51 条（`electron` 44.10.0 起 + undici / fast-uri / brace-expansion 分线 override）、ziyou-shi 5 条（`@capacitor/*` 8.5.3 + `uuid` 11.1.1）
- 保留且**明确不 dismiss** 的 2 条：`pdfjs-dist`（high，cs-notes-public）——线上真正跑的是 `docs/public/pdfjs/pdf.min.js`（3.11.174），改它要做 ESM 迁移 + 构建验证，仓库无 CI 所以没盲改；`glib`（medium，wolai-paikebiao）——Tauri 的 `gtk 0.18` 锁死 `glib 0.18`，只影响 Linux target。两条的修法与复审条件都写在各自仓的 `SECURITY-NOTES.md`
- 合规：31 个非归档仓中 **29 个**已声明许可证（MIT）；cs-notes-reference（开源笔记/教材代码）与 cs-notes-public（408 + 考研数学笔记整理）**刻意不声明**——整理他人内容的仓库不套用 MIT

`cs-notes-public` 的 pdfjs 那条**确实进浏览器产物**，不属于构建期依赖，所以它保留 OPEN，而不是被当作开发工具链问题略过。不伪造 override、不做营销式夸大；说明见 codedrill / desktoppet / kb-ui / wolai-paikebiao / cs-notes-public 的 ``SECURITY-NOTES.md``。

---

<p align="center">
  <em>"软件不是一次写成的作品，而是在不断使用和修改中成长的系统。"</em>
</p>

