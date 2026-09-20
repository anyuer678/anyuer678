<h1 align="center">Hi, I'm Yuer</h1>

<p align="center">
  <em>个人开发者 · 软件工程 · 工具与 AI 相关</em>
</p>

<p align="center">
  <a href="https://github.com/anyuer678?tab=repositories"><img alt="repos" src="https://img.shields.io/badge/public_repos-27-blue"></a>
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
      <p>seccomp/rlimit 进程级沙箱 · RabbitMQ 异步判题 · prod compose 不对宿主暴露中间件</p>
      <p>非生产就绪 · 沙箱为黑名单进程级隔离，非多租户容器</p>
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

### 项目一览

| 项目 | 状态 | 描述 | 技术 |
|------|------|------|------|
| [dsh-logtimeline](https://github.com/anyuer678/dsh-logtimeline) | `engine` | 中文自然语言日志时间查询（DSH 插件） | Python |
| [keyvault](https://github.com/anyuer678/keyvault) | `local-tool` | API 密钥保险箱（AES-256-GCM + step-up Web） | Python |
| [voiceconsole](https://github.com/anyuer678/voiceconsole) | `local-tool` | 语音指令 MCP（本机确认权 + 路径沙箱） | Python |
| [evocode](https://github.com/anyuer678/evocode) | `local-tool` | 软件体检：规则扫描为主，LLM 可选 | Java + Vue + Python |
| [developer-intelligence](https://github.com/anyuer678/developer-intelligence) | `engine` | 仓库静态解析引擎（零 LLM）；GH collector **P0 未交付** | Python |
| [chatez](https://github.com/anyuer678/chatez) | `portfolio` | Prompt + Skill 的 AI 客户端工作台（纯前端） | TypeScript |
| [kb-ui](https://github.com/anyuer678/kb-ui) | `portfolio` | Vue 3 组件库 **73** 组件 · 46 主题 · npm [kb-ui-vue](https://www.npmjs.com/package/kb-ui-vue) | Vue 3 |
| [desktoppet](https://github.com/anyuer678/desktoppet) | `portfolio` | Electron 桌宠平台（角色包解耦；单测约 450 例） | Electron |
| [codedrill](https://github.com/anyuer678/codedrill) | `portfolio` | 离线编程训练（SRS）；多端完成度不一 | Vue + Electron |
| [upgrademate](https://github.com/anyuer678/upgrademate) | `local-tool` | 行级正则升级**检查清单**（非 AST 迁移） | Python |
| [picren](https://github.com/anyuer678/picren) | `local-tool` | 图片批量 AI 重命名（默认 dry-run） | Python |
| [stargrave](https://github.com/anyuer678/stargrave) | `local-tool` | GitHub star 清理建议器 | Python |
| [yuer.dev](https://github.com/anyuer678/yuer.dev) | `portfolio` | 个人作品集 / 数字花园 | Vue 3 |
| [spotlight-wallpaper](https://github.com/anyuer678/spotlight-wallpaper) | `local-tool` | Windows 聚光壁纸（MIT） | Python |
| [huayinlaoqiang](https://github.com/anyuer678/huayinlaoqiang) | `portfolio` | 非遗展示站（代码 MIT；媒体见 CREDITS） | HTML |
| [eclipse-wasteland](https://github.com/anyuer678/eclipse-wasteland) | `portfolio` | Three.js 浏览器射击游戏 | TypeScript |
| [ai-toolbox](https://github.com/anyuer678/ai-toolbox) | `local-tool` | 本地 AI 工具用量监控 | Python |
| [todo-list](https://github.com/anyuer678/todo-list) 等 | `archived` | 学习仓 / 上游工具归档 | — |

---

### 近期工程重点（A+ 轨）

- 安全：lumen 权限硬化、voiceconsole 确认权拆分、keyvault step-up、polycodehub prod compose  
- 诚实：DI / evocode / upgrademate 声明与能力对齐  
- 治理：LICENSE 补齐、威胁模型、Issue 跟踪  

---

<p align="center">
  <em>"软件不是一次写成的作品，而是在不断使用和修改中成长的系统。"</em>
</p>
