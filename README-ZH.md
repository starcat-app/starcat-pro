<div align="center">
<a href="https://starcat.ink"><img src="./banner.webp" width="100%" alt="Starcat Pro" align="center"/></a>

<h2>Starcat Pro</h2>
<p>GitHub Stars 管理、本地知识库 RAG、GitHub 通知、我的项目、全局与仓库洞察、macOS 桌面小组件、AI 摘要与语义搜索、Release 追踪、Browser Plugin、Alfred / uTools / Raycast 等能力。</p>

<a href="https://github.com/starcat-app/homebrew-starcat"><img src="https://img.shields.io/badge/Install%20with-Homebrew-FBBF24?style=for-the-badge&logo=homebrew&logoColor=white" width="220" alt="Install with Homebrew"/></a><br/>
<sub>
<b>macOS 15 Sequoia 或更高版本</b>：优先使用 <a href="https://github.com/starcat-app/homebrew-starcat">Homebrew</a> 安装，也可以下载面向 Apple Silicon Mac 的 <a href="https://starcat.ink/downloads/Starcat-1.4.0-arm64.dmg">当前 Direct 版本（1.4.0）</a>，或在 Mac App Store 搜索 <b>Starcat for GitHub</b>。<br>
历史版本与发布说明：<a href="./CHANGELOG-ZH.md">更新日志</a> · <a href="https://starcat.ink/changelog.html">官网更新记录</a><br>
公开问题反馈：<a href="https://github.com/starcat-app/starcat-pro/issues">反馈 bug 或提出功能建议</a><br>
English: <a href="./README.md">README.md</a>
</sub>
</div>

<br />

<div align="center">
<a href="https://starcat.ink"><img src="https://img.shields.io/badge/website-starcat.ink-38BDF8?style=flat&color=blue" alt="website"/></a>
<a href="https://starcat.ink/downloads/Starcat-1.4.0-arm64.dmg"><img src="https://img.shields.io/badge/platform-macOS%2015%2B-lightgrey.svg?style=flat&color=blue" alt="platform"/></a>
<a href="https://github.com/starcat-app/starcat-localization"><img src="https://img.shields.io/badge/localization-open%20for%20contributors-lightgrey.svg?style=flat&color=blue" alt="localization"/></a>
<a href="https://github.com/starcat-app/starcat-pro/issues"><img src="https://img.shields.io/github/issues/starcat-app/starcat-pro?style=flat&color=blue" alt="issues"/></a>
</div>

<br />

## About Starcat

**Starcat** 是一款原生 macOS 应用，面向 GitHub Stars 已经超出普通收藏夹规模的用户。它把 starred repositories 同步到本地优先的桌面工作区，渲染 README，支持标签、私有笔记和阅读状态，追踪 Release，评估仓库健康度，并把收藏升级为可检索、可追问的本地知识库。从 1.3.0 起，你还可以集中管理「我的项目」、查看全局与单仓库洞察、使用 macOS 桌面小组件，并通过 Alfred / uTools / Raycast 快速找回仓库。1.4.0 在活动页加入了 GitHub 通知和 Issue / PR 会话。启用 AI 后，Starcat 可以生成 README 摘要、翻译项目文档、推荐标签、基于仓库与洞察上下文问答，并为 Pro 用户提供更深入的代码智能工作流。

<div align="center">
<img width="900" src="./main.webp" alt="Starcat 主窗口"/>
</div>

## Key Features

- **原生 GitHub Stars 管理器** - 使用 GitHub 登录，同步 starred repositories，并在 macOS 三栏界面中浏览、置顶与筛选。
- **本地优先数据模型** - 标签、私有笔记和状态保存在本地 SQLite；仓库缓存可重建。
- **README 渲染** - 阅读 GitHub README，支持图片处理、Mermaid 图表、滚动工具和专注阅读界面。
- **知识库 RAG 工作台** - 把入库仓库变成可问答的本地知识库，支持混合检索、流式回答、引用证据与会话管理。*
- **AI 结构化摘要** - 生成仓库摘要，解释项目做什么、解决什么问题、使用什么技术栈。*
- **README 翻译** - 支持分段中英对照与全文翻译，同时保留原始项目上下文。*
- **仓库级 AI 对话** - 围绕当前仓库上下文提问，并可复用洞察上下文。*
- **标签、笔记和状态** - 用自定义标签、私有笔记、阅读状态或使用状态组织仓库；支持 AI 辅助生成笔记。
- **批量整理** - 多选仓库后批量打标或执行操作。
- **全文搜索** - 使用本地 FTS5 索引搜索仓库名、作者、描述、topics 和笔记。
- **语义搜索** - 启用 AI 搜索后，可以按意图找仓库，而不只依赖精确关键词。*
- **我的项目** - 集中查看个人、组织及外部协作仓库；通过 GitHub App 按授权范围浏览公开、私有和 Internal 项目。
- **我的洞察 / 仓库洞察** - 从收藏或知识库查看整理进度、技术分布与待办，并下钻到 Star 增长、协作、提交、健康度与安全信号。
- **洞察上下文复用** - 生成后的洞察可进入 AI 摘要、仓库对话与 RAG 回答，并以可移除的只读上下文展示。*
- **macOS 桌面小组件** - 提供 Starcat Focus、今日重逢、Release Watch 和收藏趋势，点击直达对应内容。
- **Release 订阅** - 订阅重要仓库，查看新版本，并让关键更新保持可见。
- **Repo Health 和 OpenSSF 信号** - 在应用内查看维护活跃度、安全和健康度信号。
- **GitHub 通知** - 在活动页处理被 @、评审请求和 Issue / PR 会话，支持 AI 起草回复与评论翻译。
- **Explore 和发现视图** - 浏览 Trending、Discovery、GitHub 搜索和仓库榜单。
- **Browser Plugin 工作流** - 在 GitHub 页面中使用 Starcat 上下文、笔记、标签、健康度和 AI 操作。
- **外部启动器搜索** - 通过 Alfred、uTools、Raycast 搜索 Starcat 本地仓库与 GitHub。
- **分享卡片与分享链接** - 为仓库和个人资料生成视觉卡片，并支持可定位回应用的分享链接。
- **可自定义快捷键** - 为搜索、刷新、知识库 RAG 与当前仓库 AI 配置全局快捷键。
- **CLI / MCP / Agent Skill** - 让终端与 AI Agent 读取同一份本地知识库上下文。
- **CodeFlow 和 CodebaseMemory 工作流** - 为 Pro 用户准备更深入的代码图谱和仓库智能分析。*
- **双渠道分发** - Mac App Store（Starcat for GitHub）与 Direct（官网 DMG / Homebrew + Sparkle 更新）。
- **本地化** - 已支持 18 种界面语言，公开本地化资源仓库接受社区贡献。

更多能力会随着版本迭代继续加入。当前公开版本为 **Starcat 1.4.0**。

_注：带星号 (*) 的能力是 Pro 方向工作流，或依赖当前应用版本中启用的 AI/provider。_

## Getting Starcat

Starcat 同时提供 Mac App Store 与 Direct 两个渠道。核心整理能力可免费使用；Pro 工作流、更高 AI 配额和高级代码智能能力可通过 App Store 内购，或 Direct 授权开通。

- 官网与下载：https://starcat.ink
- Mac App Store：搜索 **Starcat for GitHub**
- Homebrew tap：https://github.com/starcat-app/homebrew-starcat
- 当前 Direct 版本：https://starcat.ink/downloads/Starcat-1.4.0-arm64.dmg
- 发布说明：https://starcat.ink/changelog.html

欢迎 star GitHub 页面、试用应用并反馈问题，这会帮助公开版本更快变好。

## Installation

首选使用 Homebrew 安装：

```bash
brew tap starcat-app/starcat
brew trust starcat-app/starcat
brew install --cask starcat
```

也可以手动安装：

1. 从 https://starcat.ink 下载最新 Direct `.dmg`。
2. 打开 `.dmg` 文件。
3. 把 Starcat 拖到 `/Applications`。
4. 从 `/Applications`、Launchpad 或 Spotlight 启动 Starcat。
5. 使用 GitHub 登录，或使用支持的 token 登录流程。

## Using the App

先同步你的 GitHub Stars。之后可以按标签、语言、智能集合、状态、活动和搜索浏览仓库。打开任意仓库详情页后，可以阅读 README、添加笔记、管理标签、订阅 Release、生成 AI 摘要，或启动更深入的仓库工作流。

遇到问题时，请先搜索已有 issue；如果没有对应问题，请创建新 issue，并附上 Starcat 版本、macOS 版本、复现步骤和可用截图。

## Compatibility

- Starcat 当前支持 **macOS 15 Sequoia 或更高版本**。
- 公开 Direct 下载面向 **Apple Silicon Mac**。
- 目前没有 iOS、iPadOS、watchOS、Windows 或 Android 版本。
- AI 能力取决于当前应用版本中配置的 provider 或 API key。
- 仓库缓存可重建；用户创建的标签、笔记和状态属于本地用户数据，需要时应自行备份或导出。

## Browser Extension & Integrations

Starcat 提供 GitHub 页面 companion 工作流。Browser Plugin 可以在 GitHub 页面上下文中展示 Starcat 操作：笔记、标签、健康度、README AI 摘要，以及跳回 macOS 应用的仓库入口。

项目也在扩展本地自动化和仓库智能工作流的集成点，例如 CodeFlow、CodebaseMemory，以及桌面启动器搜索。

### CLI、MCP 与 AI Agent 项目

- [starcat-cli](https://github.com/starcat-app/starcat-cli) - 用于读取和整理 Starcat 数据的跨平台 CLI 与 MCP bridge。
- [homebrew-starcat-cli](https://github.com/starcat-app/homebrew-starcat-cli) - 用于安装和更新 CLI 的官方 Homebrew tap。
- [starcat-skill](https://github.com/starcat-app/starcat-skill) - 面向 Codex、Claude Code 等 AI Agent 的官方工作流与安全约束。

### Browser Plugin Projects

- [starcat-chrome-plugin](https://github.com/starcat-app/starcat-chrome-plugin) - 用于 GitHub 页面的 Chrome/Chromium companion extension。
- [starcat-safari-plugin](https://github.com/starcat-app/starcat-safari-plugin) - 面向 macOS 的 Safari WebExtension companion package。

### Launcher Integrations

- [starcat-alfred-workflow](https://github.com/starcat-app/starcat-alfred-workflow) - 在 Alfred 中搜索 Starcat 本地仓库与 GitHub。
- [starcat-utools-plugin](https://github.com/starcat-app/starcat-utools-plugin) - 在 uTools 中搜索 Starcat 本地仓库与 GitHub。
- [starcat-raycast-extension](https://github.com/starcat-app/starcat-raycast-extension) - 在 Raycast 中搜索 Starcat 本地仓库与 GitHub。

### Self-Hostable API Projects

Starcat 使用多个小型支撑 API 来提供可选的发现、分享和仓库智能工作流。这些服务已开源，进阶用户可以审查实现、本地运行，或在需要完全控制服务端时自行部署。

- [starcat-sharing-api](https://github.com/starcat-app/starcat-sharing-api) - 分享页面生成与渲染支撑服务。
- [starcat-trending-api](https://github.com/starcat-app/starcat-trending-api) - GitHub Trending 抓取与 API。
- [starcat-weekly-api](https://github.com/starcat-app/starcat-weekly-api) - 周刊项目源聚合与 API。
- [starcat-wiki-api](https://github.com/starcat-app/starcat-wiki-api) - GitHub Wiki 与文档可用性探测。
- [starcat-recommend-api](https://github.com/starcat-app/starcat-recommend-api) - 相似仓库推荐代理。
- [starcat-discovery-api](https://github.com/starcat-app/starcat-discovery-api) - 探索发现、热门和新发布仓库 feed。

每个 API 项目都有自己的 README 和部署说明。Starcat 默认托管服务面向开箱即用；如果你希望使用自己的基础设施、API key 和数据保留策略，也可以自行部署这些 API。

## Localization

Starcat 已支持 18 种界面语言。公开本地化资源仓库在这里：

https://github.com/starcat-app/starcat-localization

贡献者可以通过 PR 改进翻译，也可以在 localization 仓库的 issue 中附上修改后的 `.xcstrings` 文件。

## Contact & Feedback

请先查看官方主页：https://starcat.ink

这个仓库是 Starcat Pro 的公开支持和发布说明入口。请使用 GitHub Issues 反馈 bug、体验问题和功能建议：

https://github.com/starcat-app/starcat-pro/issues

这个仓库**不包含**应用源码、后端源码、构建脚本或私有配置。
