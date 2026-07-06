<div align="center">
<a href="https://starcat.ink"><img src="./banner.webp" width="100%" alt="Starcat Pro" align="center"/></a>

<h2>Starcat Pro</h2>
<p>GitHub Stars Management, README Rendering, AI Summaries, Semantic Search, Release Tracking, Repo Health, Browser Plugin, CodeFlow, CodebaseMemory and More!</p>

<a href="https://starcat.ink/downloads/Starcat-1.1.0-arm64.dmg"><img src="https://img.shields.io/badge/Download%20for-macOS-22C55E?style=for-the-badge&logo=apple&logoColor=white" width="220" alt="Download for macOS"/></a><br/>
<sub>
<b>macOS 15 Sequoia or newer</b>: Download the <a href="https://starcat.ink/downloads/Starcat-1.1.0-arm64.dmg">current Direct build</a> for Apple Silicon Macs.<br>
Previous versions and release notes: <a href="./CHANGELOG.md">Changelog</a> · <a href="https://starcat.ink/changelog.html">Website changelog</a><br>
Public issue tracker: <a href="https://github.com/dong4j/starcat-pro/issues">Report a bug or request a feature</a><br>
中文说明: <a href="./README-ZH.md">README-ZH.md</a>
</sub>
</div>

<br />

<div align="center">
<a href="https://starcat.ink"><img src="https://img.shields.io/badge/website-starcat.ink-38BDF8?style=flat&color=blue" alt="website"/></a>
<a href="https://starcat.ink/downloads/Starcat-1.1.0-arm64.dmg"><img src="https://img.shields.io/badge/platform-macOS%2015%2B-lightgrey.svg?style=flat&color=blue" alt="platform"/></a>
<a href="https://github.com/dong4j/starcat-localization"><img src="https://img.shields.io/badge/localization-open%20for%20contributors-lightgrey.svg?style=flat&color=blue" alt="localization"/></a>
<a href="https://github.com/dong4j/starcat-pro/issues"><img src="https://img.shields.io/github/issues/dong4j/starcat-pro?style=flat&color=blue" alt="issues"/></a>
</div>

<br />

## About Starcat

**Starcat** is a native macOS app for people whose GitHub Stars have outgrown a bookmark list. It syncs starred repositories into a local-first desktop workspace, renders README content, adds tags, notes and reading status, tracks releases, evaluates repository health and helps you turn saved projects into a reusable knowledge base. With AI enabled, Starcat can summarize README files, translate project docs, suggest tags, answer questions with repository context and prepare deeper code-intelligence workflows for Pro users.

<div align="center">
<img width="900" src="./main.webp" alt="Starcat main window"/>
</div>

## Key Features

- **Native GitHub Stars manager** - sign in with GitHub, sync your starred repositories and browse them in a focused macOS three-column interface.
- **Local-first data model** - tags, private notes and status live in local SQLite; repository cache can be rebuilt.
- **README rendering** - read GitHub README content with image handling, scroll tooling and a dedicated reading surface.
- **AI-generated structured summaries** - generate summaries that explain what a repository does, what problem it solves and which stack it uses. *
- **README translation** - translate repository README content while keeping the original project context available. *
- **Repo-level AI chat** - ask questions about the current repository with preserved context. *
- **Tags, notes and status** - organize repositories with custom tags, private notes and reading or usage states.
- **Batch organization** - select multiple repositories and apply tags or actions in bulk.
- **Full-text search** - search repository names, owners, descriptions, topics and notes with a local FTS5 index.
- **Semantic search** - find repositories by intent, not only exact keywords, when AI search is enabled. *
- **Release subscriptions** - subscribe to important repositories, review new releases and keep updates visible.
- **Repo Health and OpenSSF signals** - evaluate maintenance, activity and security signals directly inside the app.
- **Explore and discovery views** - browse trending, discovery, GitHub search and ranked repository lists.
- **Browser Plugin workflow** - bring Starcat context, notes, tags, health and AI actions to GitHub pages.
- **Share cards** - create visual cards for repositories and profiles.
- **CodeFlow and CodebaseMemory workflows** - prepare deeper code graph and repository intelligence workflows for Pro users. *
- **Direct distribution** - current macOS Direct build supports in-app updates through Sparkle.
- **Localization** - English and Simplified Chinese are available; community localization lives in a public repository.

...and more is coming as Starcat Pro stabilizes.

_Note: features marked with an asterisk (*) are Pro-oriented workflows or depend on AI/provider availability. Pro purchasing is not open yet._

## Getting Starcat Pro

Starcat currently ships as a macOS Direct build. Core organization features are free while Pro workflows, higher AI quotas and advanced code-intelligence features are being prepared.

- Download Starcat from the official website: https://starcat.ink
- Current Direct build: https://starcat.ink/downloads/Starcat-1.1.0-arm64.dmg
- Release notes: https://starcat.ink/changelog.html

Pro purchasing is not available yet. Final pricing, entitlement rules and payment flow will be announced when Starcat Pro opens.

Please star the GitHub page, try the app and report issues so the public release can improve faster.

## Installation

Install the app manually:

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

The project also prepares integration points for local automation and repository intelligence workflows such as CodeFlow and CodebaseMemory.

## Localization

Starcat supports localization. Public localization resources are available here:

https://github.com/dong4j/starcat-localization

Contributors can improve translations through pull requests or by attaching edited `.xcstrings` files to issues in the localization repository.

## Contact & Feedback

Please check the official homepage first: https://starcat.ink

This repository is the public support and release-notes home for Starcat Pro. Use GitHub Issues for bugs, usability problems and feature requests:

https://github.com/dong4j/starcat-pro/issues

This repository does **not** contain application source code, backend source code, build scripts or private configuration.
