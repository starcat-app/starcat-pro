<div align="center">
<a href="https://starcat.ink"><img src="./banner.webp" width="100%" alt="Starcat Pro" align="center"/></a>

<h2>Starcat Pro</h2>
<p>GitHub Stars management, local RAG knowledge base, My Projects, library and repository insights, macOS desktop widgets, AI summaries, semantic search, release tracking, browser plugins, Alfred / uTools / Raycast, and more.</p>

<a href="https://github.com/starcat-app/homebrew-starcat"><img src="https://img.shields.io/badge/Install%20with-Homebrew-FBBF24?style=for-the-badge&logo=homebrew&logoColor=white" width="220" alt="Install with Homebrew"/></a><br/>
<sub>
<b>macOS 15 Sequoia or newer</b>: Install with <a href="https://github.com/starcat-app/homebrew-starcat">Homebrew</a>, download the <a href="https://starcat.ink/downloads/Starcat-1.3.0-arm64.dmg">current Direct build (1.3.0)</a> for Apple Silicon Macs, or get <b>Starcat for GitHub</b> from the Mac App Store.<br>
Previous versions and release notes: <a href="./CHANGELOG.md">Changelog</a> · <a href="https://starcat.ink/changelog.html">Website changelog</a><br>
Public issue tracker: <a href="https://github.com/starcat-app/starcat-pro/issues">Report a bug or request a feature</a><br>
中文说明: <a href="./README-ZH.md">README-ZH.md</a>
</sub>
</div>

<br />

<div align="center">
<a href="https://starcat.ink"><img src="https://img.shields.io/badge/website-starcat.ink-38BDF8?style=flat&color=blue" alt="website"/></a>
<a href="https://starcat.ink/downloads/Starcat-1.3.0-arm64.dmg"><img src="https://img.shields.io/badge/platform-macOS%2015%2B-lightgrey.svg?style=flat&color=blue" alt="platform"/></a>
<a href="https://github.com/starcat-app/starcat-localization"><img src="https://img.shields.io/badge/localization-open%20for%20contributors-lightgrey.svg?style=flat&color=blue" alt="localization"/></a>
<a href="https://github.com/starcat-app/starcat-pro/issues"><img src="https://img.shields.io/github/issues/starcat-app/starcat-pro?style=flat&color=blue" alt="issues"/></a>
</div>

<br />

## About Starcat

**Starcat** is a native macOS app for people whose GitHub Stars have outgrown a bookmark list. It syncs starred repositories into a local-first desktop workspace, renders README content, adds tags, notes and reading status, tracks releases, evaluates repository health and turns saved projects into a searchable, askable knowledge base. Since 1.3.0 it also includes My Projects, library-wide and repository insights, macOS desktop widgets, and Alfred / uTools / Raycast search integrations. With AI enabled, Starcat can summarize README files, translate project docs, suggest tags, answer questions with repository and insight context, and prepare deeper code-intelligence workflows for Pro users.

<div align="center">
<img width="900" src="./main.webp" alt="Starcat main window"/>
</div>

## Key Features

- **Native GitHub Stars manager** - sign in with GitHub, sync starred repositories, and browse, pin and filter them in a focused macOS three-column interface.
- **Local-first data model** - tags, private notes and status live in local SQLite; repository cache can be rebuilt.
- **README rendering** - read GitHub README content with image handling, Mermaid diagrams, scroll tooling and a dedicated reading surface.
- **Knowledge-base RAG workspace** - turn ingested repositories into a local Q&A knowledge base with hybrid retrieval, streaming answers, citations and session management. *
- **AI-generated structured summaries** - generate summaries that explain what a repository does, what problem it solves and which stack it uses. *
- **README translation** - translate README content with bilingual segment view or full-document replacement while keeping original context available. *
- **Repo-level AI chat** - ask questions about the current repository, optionally reusing insight context. *
- **Tags, notes and status** - organize repositories with custom tags, private notes and reading or usage states; AI can help draft notes.
- **Batch organization** - select multiple repositories and apply tags or actions in bulk.
- **Full-text search** - search repository names, owners, descriptions, topics and notes with a local FTS5 index.
- **Semantic search** - find repositories by intent, not only exact keywords, when AI search is enabled. *
- **My Projects** - browse personal, organization and collaborator repositories via GitHub App scopes, including public, private and internal projects.
- **Library and repository insights** - review organization progress, tech distribution and follow-ups, then drill into stars, collaboration, commits, health and security signals.
- **Reusable insight context** - generated insights can feed AI summaries, repo chat and RAG answers as removable read-only context. *
- **macOS desktop widgets** - Starcat Focus, Today Reunion, Release Watch and collection trends, with deep links into the app.
- **Release subscriptions** - subscribe to important repositories, review new releases and keep updates visible.
- **Repo Health and OpenSSF signals** - evaluate maintenance, activity and security signals directly inside the app.
- **Explore and discovery views** - browse trending, discovery, GitHub search and ranked repository lists.
- **Browser Plugin workflow** - bring Starcat context, notes, tags, health and AI actions to GitHub pages.
- **Launcher search integrations** - search Starcat local repositories and GitHub from Alfred, uTools and Raycast.
- **Share cards and share links** - create visual cards and openable share links that jump back into Starcat.
- **Customizable shortcuts** - configure global shortcuts for search, refresh, knowledge-base RAG and current-repo AI.
- **CLI / MCP / Agent Skill** - let terminals and AI agents read the same local knowledge-base context.
- **CodeFlow and CodebaseMemory workflows** - prepare deeper code graph and repository intelligence workflows for Pro users. *
- **Dual distribution** - Mac App Store (**Starcat for GitHub**) and Direct (website DMG / Homebrew with Sparkle updates).
- **Localization** - 18 UI languages are available; community localization lives in a public repository.

More capabilities continue to ship with each release. The current public version is **Starcat 1.3.0**.

_Note: features marked with an asterisk (*) are Pro-oriented workflows or depend on AI/provider availability._

## Getting Starcat

Starcat ships through both the Mac App Store and Direct channels. Core organization features are free; Pro workflows, higher AI quotas and advanced code-intelligence features are available via App Store in-app purchase or Direct licensing.

- Website and downloads: https://starcat.ink
- Mac App Store: search for **Starcat for GitHub**
- Homebrew tap: https://github.com/starcat-app/homebrew-starcat
- Current Direct build: https://starcat.ink/downloads/Starcat-1.3.0-arm64.dmg
- Release notes: https://starcat.ink/changelog.html

Please star the GitHub page, try the app and report issues so the public release can improve faster.

## Installation

Homebrew is the preferred installation method:

```bash
brew tap starcat-app/starcat
brew trust starcat-app/starcat
brew install --cask starcat
```

You can also install the app manually:

1. Download the latest Direct `.dmg` from https://starcat.ink
2. Open the `.dmg` file.
3. Move Starcat to `/Applications`.
4. Launch Starcat from `/Applications`, Launchpad or Spotlight.
5. Sign in with GitHub or use a supported token-based flow.

## Using the App

Start by syncing your GitHub Stars. Then browse repositories by tags, languages, smart collections, status, activity and search. Open any repository detail page to read its README, add notes, manage tags, subscribe to releases, generate AI summaries or launch deeper repository workflows.

If you run into a problem, search existing issues first and then open a new issue with your Starcat version, macOS version, reproduction steps and screenshots when available.

## Compatibility

- Starcat currently supports **macOS 15 Sequoia or newer**.
- The public Direct download is intended for **Apple Silicon Macs**.
- There are no iOS, iPadOS, watchOS, Windows or Android builds today.
- AI features depend on the provider or API key configured in the current app build.
- Repo cache can be rebuilt; user-created tags, notes and status are local user data and should be backed up or exported when needed.

## Browser Extension & Integrations

Starcat includes companion workflows for GitHub pages. The browser plugin can surface Starcat actions in context: notes, tags, health information, README AI summaries and repository handoff back to the macOS app.

The project also expands local automation and repository intelligence integrations such as CodeFlow, CodebaseMemory and desktop launcher search.

### CLI, MCP & AI Agent Projects

- [starcat-cli](https://github.com/starcat-app/starcat-cli) - cross-platform CLI and MCP bridge for reading and organizing Starcat data.
- [homebrew-starcat-cli](https://github.com/starcat-app/homebrew-starcat-cli) - official Homebrew tap for installing and updating the CLI.
- [starcat-skill](https://github.com/starcat-app/starcat-skill) - official workflow and safety contract for AI agents such as Codex and Claude Code.

### Browser Plugin Projects

- [starcat-chrome-plugin](https://github.com/starcat-app/starcat-chrome-plugin) - Chrome/Chromium companion extension for GitHub pages.
- [starcat-safari-plugin](https://github.com/starcat-app/starcat-safari-plugin) - Safari WebExtension companion package for macOS.

### Launcher Integrations

- [starcat-alfred-workflow](https://github.com/starcat-app/starcat-alfred-workflow) - search Starcat local repositories and GitHub from Alfred.
- [starcat-utools-plugin](https://github.com/starcat-app/starcat-utools-plugin) - search Starcat local repositories and GitHub from uTools.
- [starcat-raycast-extension](https://github.com/starcat-app/starcat-raycast-extension) - search Starcat local repositories and GitHub from Raycast.

### Self-Hostable API Projects

Starcat uses small support APIs for optional discovery, sharing and repository intelligence workflows. These services are open so advanced users can inspect them, run them locally or deploy their own instances when they want full control of the server side.

- [starcat-sharing-api](https://github.com/starcat-app/starcat-sharing-api) - share page generation and rendering support.
- [starcat-trending-api](https://github.com/starcat-app/starcat-trending-api) - GitHub Trending collection and API.
- [starcat-weekly-api](https://github.com/starcat-app/starcat-weekly-api) - weekly project source aggregation and API.
- [starcat-wiki-api](https://github.com/starcat-app/starcat-wiki-api) - GitHub Wiki and documentation availability checks.
- [starcat-recommend-api](https://github.com/starcat-app/starcat-recommend-api) - similar repository recommendation proxy.
- [starcat-discovery-api](https://github.com/starcat-app/starcat-discovery-api) - discovery, hot and newly released repository feeds.

Each API project contains its own README and deployment notes. Starcat's hosted defaults are meant to work out of the box, but self-hosting is available for users who prefer their own infrastructure, API keys and data-retention policy.

## Localization

Starcat currently ships with 18 UI languages. Public localization resources are available here:

https://github.com/starcat-app/starcat-localization

Contributors can improve translations through pull requests or by attaching edited `.xcstrings` files to issues in the localization repository.

## Contact & Feedback

Please check the official homepage first: https://starcat.ink

This repository is the public support and release-notes home for Starcat Pro. Use GitHub Issues for bugs, usability problems and feature requests:

https://github.com/starcat-app/starcat-pro/issues

This repository does **not** contain application source code, backend source code, build scripts or private configuration.
