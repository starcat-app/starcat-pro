# Starcat Changelog

All notable changes to Starcat are summarized here for release notes.

## 1.2.0-待发布

### New

- Added repository pinning in Manage, with Pin and Unpin actions, most-recently-pinned ordering within each category, and a card-corner indicator.
- Added repository share links that open Starcat and locate the shared repository.
- Added customizable app shortcuts for search, refreshing the current content, opening the Knowledge RAG workspace, and opening AI for the current repository, with global and per-shortcut enable controls.
- Added local Mermaid diagram rendering to repository README pages, with responsive sizing in narrow detail panes and readable source fallback when rendering fails.
- Added segmented and full README translation modes: segmented translation is the default for paragraph-by-paragraph bilingual reading, while full translation replaces visible text without rewriting the README structure.

### Improvements

- Improved the add-tag popover with clearer colored-icon rows and selection, plus a solid window-matched background.
- Improved the Pro sidebar username gradient for light and dark themes, with smoother first-letter color and better light-mode contrast.
- Improved navigation across Starred and Explore with clearer three-level hierarchy and filter context.
- Improved README translation speed with a smaller first batch, incremental results, up to four concurrent AI requests, per-segment caching, and resume support for untranslated segments.
- Improved personal notes with README-based AI generation and refinement, visible progress, Markdown editing and preview, draft copying, and clearer save status.
- Improved AI sharing by reusing existing AI summaries, with support for cancelling creation and generating a new AI share link.
- Improved knowledge-base chunk management: shard counts match language/stars sizing on repo cards; edit and detail views show last-updated time and approximate token counts.

### Fixes

- Fixed the Knowledge Base entry occasionally not responding, failing to restore a minimized window, or opening the empty-library setup before index status finished loading.

## 1.1.0

Starcat 1.1.0 turns saved repositories into a local-first, explainable RAG knowledge base, with broad performance, reliability, and macOS interface improvements.

### New

- Added a full knowledge-base RAG workspace with multi-repository context, streaming answers, citations, conversation groups, pinning, history, and draft recovery.
- Added hybrid retrieval across vector and bilingual keyword search, repository metadata, Wiki, RepoContext, optional reranking, live GitHub context, and external search.
- Added knowledge-base browsing and index management with batch Star imports, README completion, chunk editing and exclusion, targeted rebuilds, and index health checks.
- Added explainable RAG controls for query plans, execution timelines, retrieval funnels, context budgets, historical replay, retrieval settings, and debug export.
- Added a local AI usage dashboard for requests, tokens, latency, and failures without storing prompts or response content.
- Added global Star-status filters and AI-summary indicators for faster repository triage.

### Improvements

- Improved large-library and long-conversation performance with bounded indexing, batched vector work, incremental persistence, limited prefetching, and caching.
- Improved the RAG workspace with resizable columns, loading skeletons, richer citation panels, code and table copying, stable scrolling, and responsive typography.
- Improved AI settings and background jobs with clearer model capabilities, safer tag suggestions, actionable diagnostics, progress reporting, and cancel or skip controls.
- Improved Explore, Trending, and Weekly with shared snapshots, session caches, cancellation-safe switching, source filters, timelines, and stable loading states.
- Improved native macOS consistency across settings, pickers, segmented controls, sidebar icons, semantic colors, and compact window layouts.
- Improved browser Companion workflows with configurable local ports, recommendation pagination, Star-state synchronization, and clearer availability feedback.
- Improved Direct Pro Pass activation, device management, seat-limit feedback, subscription cancellation, and channel-specific update controls.

### Fixes

- Fixed RAG scope isolation across repository or account switches, concurrent tasks, cancellations, and stale callbacks.
- Fixed retrieval and citation correctness for explicit repository scopes, private notes, bilingual keywords, Wiki content, excluded chunks, false citation markers, and no-evidence refusal.
- Fixed conversation stability for title generation, pin ordering, draft and history restoration, long-session compression, streaming timers, and scroll-to-bottom behavior.
- Fixed knowledge-base refresh and indexing issues, including unnecessary reloads, stale vectors overwriting new chunks, inaccurate source updates, and background Wiki refresh failures.
- Fixed browser-based GitHub sign-in, localized AI and RAG error feedback, and several settings, layout, and accessibility issues.

## 1.0.0

Initial Starcat public release.

### Highlights

- Manage GitHub stars in a native macOS three-column app.
- Sign in with GitHub and sync starred repositories with progress, refresh, and rate-limit handling.
- Browse repositories by all stars, tags, languages, smart collections, status, archived state, forks, and search.
- Read repository details with metadata, README rendering, GitHub shortcuts, clone links, and unstar actions.
- Organize repositories with tags, batch tagging, private notes, and reading or usage status.
- Search locally across repository names, owners, descriptions, notes, and related metadata.
- Explore GitHub Trending, weekly sources, recommendations, and repository activity.
- Track releases, subscribe to repositories, review assets, and mark updates as read.
- Use AI features with your own provider settings, including repository summaries, tag suggestions, chat, semantic search, README translation, and sharing support.
- Review repository health signals, OpenSSF Scorecard information, Wiki context, and related insights.
- Create and export share cards and repository collections for external sharing.
- Manage app settings, storage, diagnostics, open-source credits, themes, language, and interface preferences.
- Use English and Simplified Chinese throughout the app.
- Run as a native macOS app with sandboxing, hardened runtime, window management, and App Store readiness work in place.

### New

- Added Getting Started onboarding system covering sync, RAG/Agent trials, project homepage, and knowledge base setup, with back navigation and debug-mode toggle.
- Added overlay state protection to prevent onboarding lockout after unexpected exits, unified manual replay guard, and share guidance bubble positioning.
- Added Agent and RAG workbenches as independent system windows with floating pin control, collapsible sidebars, and inherited interface scale.
- Added Agent plan and tool output display, expanded event model, and completed runtime event feedback loop.
- Added landing page hero loading animation with multi-stage transitions, macOS-native download modal with refreshed pricing grid, and a download version section.
- Added similar repository recommendations, with saved results, clearer recommendation cards, starred-repo indicators, and the option to open recommended repositories in a separate Starcat window.
- Added more GitHub sign-in choices, including browser-based sign-in, token sign-in, a clearer login chooser, and a visible authorization countdown.
- Added repository code intelligence as a Pro feature, giving each repository its own analysis workspace, cached results, and a dedicated settings entry.
- Added an in-detail AI assistant entry, README AI summaries, summary caching, and smoother summary generation from both Starcat and browser-based entry points.
- Added a Browser Plugin workflow for GitHub pages, including local pairing, repository context, notes, tags, health data, Wiki context, recommendations, and Safari WebExtension support.
- Added a getting started checklist to guide first-time setup and key actions.
- Added Explore and discovery surfaces for trending, discovery, GitHub search, and ranked repository lists.
- Added README background fetching and health score prefetching so repository details can feel ready sooner.
- Added health score sorting, health color states, and OpenSSF Scorecard warmup for easier repository evaluation.
- Added menu bar and macOS menu controls for quicker access to common actions.
- Added Direct distribution support alongside the App Store channel, including a separate Direct build target, channel-aware configuration, and Direct-only Sparkle update integration.
- Added Sparkle update support for Direct builds, including an appcast feed, EdDSA key configuration, update menu integration, and documentation for key backup and multi-Mac signing workflows.
- Added Direct license infrastructure with a License API service, local license storage, and a channel-neutral entitlement layer for App Store and Direct builds.
- Added a provider-neutral direct payment abstraction so future payment gateways such as Creem can be integrated without binding the app to one vendor.
- Added service status badges, service health checks, and local operations tools for easier setup and troubleshooting.
- Added interface size controls, release timeline paging, and release subscription counts in the sidebar.

- Includes an Agent workbench with audit trail visibility, refined reply styling, recognizable toolbar entry points, and title bar controls.
- Includes a polished DMG background, clear app-drop-link placement, and readable Direct distribution file names.
- Includes a refined landing page presentation, macOS-native download flow, pricing layout, and product texture.
- Includes first-sync and weekly page loading states with shared loading indicators.
- Includes recommendation cards, recommendation caching, clear placement, starred-repository indicators, and Pro gating.
- Includes README rendering with GitHub image handling, system-style scrollbars, and clear loading states.
- Includes global search with keyboard shortcut, history, reliable focus behavior, and GitHub result pagination.
- Includes GitHub Stars list handling, sidebar counts, language icons, and empty states.
- Includes Activity and Weekly browsing with filters, fast counts, and detail loading states.
- Includes sharing cards with multiple layouts, color options, profile details, and Pro-aware availability.
- Includes Settings copy, storage actions, service configuration, and diagnostic log feedback.
- Includes dark mode support across AI, health, search, sharing, and plugin-related screens.
- Includes release readiness materials, open-source credits, distribution planning, and in-app release notes loading.
- Includes Direct release tooling with separate App Store and Direct packaging scripts, Direct run targets, Sparkle appcast generation, and release orchestration for appcast and DMG upload.
- Includes Starcat website nginx rules for Sparkle appcast freshness and Direct download paths.
- Includes shared action icon patterns across toolbars, dangerous actions, common actions, tags, sidebars, and batch operations.
- Includes internal diagnostics, telemetry safety, and developer-only controls without exposing unfinished features as product features.
- Includes stable Agent default artifact selection on load.
- Includes stable RAG and workbench input handling for first-keystroke text entry.
- Includes RAG middle column message alignment and workbench title bar icon visibility.
- Includes correct landing page macOS version labeling.
- Includes Dock and menu bar reopening behavior after the main window is closed.
- Includes correct cursor behavior when overlays sit above README content or other interactive views.
- Includes AI summary generation for repositories whose GitHub names differ only by letter case.
- Includes browser plugin handling for unavailable or Pro-only actions.
- Includes automatic visible-content refresh after notes or tags are changed from external entry points.
- Includes stable recommended repository windows and README loading behavior.
- Includes CodebaseMemory launch, storage, cache, and repository-switching support.
- Includes README image support for subdirectories and GitHub raw image paths.
- Includes global search focus timing and refined search result interactions.
- Includes storage reset completion states, unsigned-in storage scrolling, and settings layout edge cases.
- Includes language aggregation sorting for repositories with missing language data.
- Includes release-build-safe debug-only menu controls.
- Includes Direct build signing and entitlement checks so non-App Store builds run without the App Sandbox entitlement while App Store builds keep their sandbox configuration.
- Includes Direct update test packaging with temporary marketing/build version overrides and appcast generation that only uses the intended DMG files.
