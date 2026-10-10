<h1 align="center">Hi, I'm Yuer</h1>

<p align="center">
  <em>个人开发者 · 软件工程 · 工具与 AI 相关</em>
</p>

<p align="center">
  <a href="https://anyuer678.github.io/yuer.dev/"><img alt="site" src="https://img.shields.io/badge/%E6%A1%88%E4%BE%8B%E7%AB%99-yuer.dev-8b5cf6"></a>
  <a href="https://github.com/anyuer678?tab=repositories"><img alt="repos" src="https://img.shields.io/badge/public_repos-28-blue"></a>
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

[evocode](https://github.com/anyuer678/evocode) · [developer-intelligence](https://github.com/anyuer678/developer-intelligence) · [desktoppet](https://github.com/anyuer678/desktoppet) · [picren](https://github.com/anyuer678/picren) · [spotlight-wallpaper](https://github.com/anyuer678/spotlight-wallpaper) · [huayinlaoqiang](https://github.com/anyuer678/huayinlaoqiang) · [eclipse-wasteland](https://github.com/anyuer678/eclipse-wasteland)

| 归档 | 状态 | 说明 |
|------|------|------|
| [todo-list](https://github.com/anyuer678/todo-list) / [key-tool](https://github.com/anyuer678/key-tool) 等 | `archived` | 学习仓 / 上游归档；key-tool 为已归档的 API Key 消费网关（替代见 keyvault）；upgrademate / stargrave / ai-toolbox 已于 2026-09 毕业归档（聚焦核心项目） |

### 近期工程重点（A+ 轨）

- 沙箱演进（2026-09）：polycodehub 判题沙箱从 136 行 seccomp 黑名单升级为 **trace 驱动白名单 + cgroup v2 按判题隔离 + NET/PID/MOUNT ns + chroot jail**（PR #18/#19/#20，adversarial CI 实测抓出并修复 12 个真 bug）；[演进长文](https://anyuer678.github.io/yuer.dev/notes/polycodehub-sandbox-notes/)
- 聚焦（2026-09）：作品集瘦身——upgrademate / stargrave / ai-toolbox **毕业归档**，维护精力集中于 polycodehub / kb-ui / lumen / evocode / desktoppet / codedrill；**冻结新仓，转向外部验证**
- 安全：lumen 权限硬化、voiceconsole 确认权拆分、keyvault step-up、polycodehub prod compose  
- 诚实：DI / evocode 声明与能力对齐  
- 治理：LICENSE 补齐、威胁模型、Issue 跟踪  
- 质量门禁：keyvault / voiceconsole / dsh-logtimeline / desktoppet 增加 **覆盖率下限**（pytest-cov / vitest coverage，阈值贴当前基线，不造红灯）  
- 素材：[design-assets](https://github.com/anyuer678/design-assets)（文档层引用，不改产品画风）
- 发布：kb-ui npm **四包**（组件库 / 工具库 / 参考后端 / scoped 脚手架 `@yuer678/create-kb`——无 scope `create-kb` 是同名无关项目）；design-assets **Release v1.0**（99 文件样例全集 2048×1152）  
- 门禁与保鲜（2026-09）：kb-ui E2E / 视觉回归 required、**npm audit 真门禁**（高危阻断合并）；案例站数据巡检刷新；27 仓 LICENSE 全覆盖、4 仓补 SECURITY / CONTRIBUTING  

**Portfolio quality pass（2026-09）**：安全加固完成。Dependabot 当前 **OPEN = 8**，全部为上游无补丁的构建工具链告警，如实披露如下——

- `extract-zip`（HIGH，GHSA-7pqw-9j4j-h8q3 / GHSA-jmr9-qjv8-65gv）× codedrill、desktoppet：npm 最新仍为 2.0.1（漏洞范围 `<= 2.0.1`），无可用补丁
- `vite` / `esbuild`（HIGH×1 + MODERATE×3）× kb-ui 文档站：来自 vitepress ^1.x 的传递依赖（vitepress 1.6.4 锁 `vite ^5.4.14`，2.x 仍在 alpha），组件库自身 vite 已是 ^8.3.0，文档站工具链在 vitepress 2.0 正式发布前结构性无法修复

以上均为 devDependencies / 构建期依赖，不进任何运行时产物。不伪造 override、不做营销式夸大；缓解说明见各仓 `docs/SECURITY-NOTES.md`。

---

<p align="center">
  <em>"软件不是一次写成的作品，而是在不断使用和修改中成长的系统。"</em>
</p>

