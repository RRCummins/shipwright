# Changelog

All notable changes to Shipwright releases are documented here.

## 0.6.2 — 2026-10-11

- **New Background status.** When a Claude turn ends while its background shells, monitors or subagents are still running, the tab shows Background until they finish, instead of looking done.
- Tabs no longer bounce back into the Inbox after you click them, and agents that have exited no longer show as a fresh Result.
- **Less Warp left over.** Warp account, Drive, sharing and Warp AI commands are gone from the menus, command palette and keybinding settings. Settings, menus and notifications say Shipwright, Help links open the Shipwright repo, and the first-run theme picker no longer asks you to accept Warp's terms.
- `shipwright://` links now open in Shipwright. They were being dropped before.
- **Windows (alpha).** `Shipwright-0.6.2-windows-x64.zip` is an alpha build for Windows 10/11 x64: unzip it and run `shipwright.exe`. It isn't code-signed yet, so SmartScreen will warn the first time. Expect rough edges.

**Download:** `Shipwright-0.6.2.dmg` (macOS) or `Shipwright-0.6.2-windows-x64.zip` (Windows, alpha) from the release assets below.

## 0.6.1 — 2026-10-11

- **New Usage page.** Open it from the chart button in the sidebar footer. It shows tokens, cache reads, sessions and active days for Claude Code and Codex over 7 days to a year, a daily chart you can split by agent, a 12-month activity heatmap with your busiest hours, and a breakdown by agent, project or model. Everything is read from your local transcripts and stays on your Mac.
- **See what each open tab costs.** The Usage page lists every open tab with its memory (agent, MCP servers, shell and scrollback), how long it has been open and its session's tokens. Quick-select shells, tabs idle for over an hour, or tabs over 400 MB, and close them in one go. Restart an agent to free its memory; it picks up the same session.
- Freshly launched or resumed agents no longer show as Running before you've sent a prompt (for example, every resumed tab after relaunching Shipwright).
- Claude's "waiting for your input" reminders no longer push an idle tab back to Asking.

**Download:** `Shipwright-0.6.1.dmg` from the release assets below.

## 0.6.0 — 2026-10-10

- **New Linear Indigo colors.** Untinted neutral-grey window and cards, an indigo accent, and clearer agent status colors: yellow for Asking, indigo for Running, green for Done, red for errors, violet for Approve. Light mode gets matching tones.
- Refreshed project badge colors and an Indigo option in the project color picker.
- **No more beachballs during builds.** Shipwright no longer freezes while a build or an agent is writing lots of files. A leftover Warp file watcher was rescanning your whole project on every change; it and the other leftover Warp AI background scanners (skills, MCP configs, code indexing, rules) are now turned off.
- Faster file lookups in large projects, so the file explorer and diff views stay snappy.
- Claude Code sessions keep saving their transcripts even when Shipwright itself was opened from a Claude session, so `--resume` and session history work.

**Download:** `Shipwright-0.6.0.dmg` from the release assets below.

## 0.4.1 — 2026-10-09

- Linear-inspired UI refresh: the sidebar now owns the title bar, so the terminal card rises to the top of the window.
- Window controls (Settings, View options, Notifications, Code review, Sail, Appearance) moved to the sidebar footer, or the rail when collapsed.
- Single-line sidebar rows with status dots, Linear-style project headers, and a cleaner collapsed rail.
- Darker, deeper dark mode, thin-stroke icon set, and a soft fade at the top of the terminal card.
- Redesigned agent notifications, and the code review panel now floats as its own card.
- Diff view: Linear-style red/green, colored line numbers, slim file headers, and softer highlights.

**Download:** `Shipwright-0.4.1.dmg` from the release assets below.

## 0.3.3 — 2026-06-22

- Added an in-app App icon chooser (Settings → Appearance): Dark, Light, or Follow System, with pre-squircled dock art.
- Integrated status/time chip on project tabs showing agent state and last activity at a glance.
- Resume-clear affordances and a move-to-inbox action for tidying up project tabs.

**Download:** `Shipwright-0.3.3.dmg` from the release assets below.

## 0.3.2 — 2026-06-22

- Removed remaining Warp/Oz cloud surfaces: session sharing (Share menu + sign-up popup), Warp AI/Drive menus, and the Teams settings page.
- Resume now targets the exact Claude session (captures the session id), plus a "Resume all" action per project.
- Added a "Clear status" right-click action to reset a stuck tab.
- Project list alphabetical sort ignores leading symbols.

**Download:** `Shipwright-0.3.2.dmg` from the release assets below.

## 0.3.1 — 2026-06-20

First publicly distributed, signed and notarized macOS build.

- Signed with Apple Developer ID and notarized by Apple (launches without Gatekeeper warnings).
- Light/dark "Linear treatment" UI revision, with the shell chrome following the active theme.
- Floating conversation/card layout with uniform spacing between the sidebar and cards.
- Unified appearance setting (Light / Dark / System) with a first-run appearance choice.

**Download:** `Shipwright-0.3.1.dmg` from the release assets below.
