# MacAppUpdater community feedback

This is the place to report bugs, suggest features, or ask questions about MacAppUpdater. We read everything that comes in.

---

## What is MacAppUpdater?

MacAppUpdater is a native macOS app (SwiftUI) that helps you see which of your installed apps are up to date. It scans your Mac, talks to our update server and the Mac App Store, and shows you what is current and what is not. Support for Sparkle-based updates and more is in the pipeline.

We track planned work and the roadmap on our [Trello board](https://trello.com/b/N8iNVYHh/my-trello-board). If you are curious what is coming next or want to see how your feature request fits in, that is the place to look.

**This repository is for feedback only.** The app’s source code is not published here.

---

## How to contribute

**Report a bug**  
Open an issue with: what you did, what you expected, what actually happened, your macOS version and MacAppUpdater version, and any screenshots or logs that help.

**Suggest a feature**  
Open an issue describing what you want and why it would help. Mockups or examples are optional but welcome.

**Ask a question**  
Search existing issues and discussions first. If nothing fits, open a new issue or discussion.

**Vote**  
Use reactions (e.g. 👍) on issues you care about. It helps us prioritise.

---

## Before you post

1. **Check the in-app Help** — MacAppUpdater includes built-in Help (Help menu or from within the app) with detailed info on usage, permissions, troubleshooting, Sparkle/MAS behaviour, privacy, and more. It is worth a look before posting.
2. **Search** — Your bug or question might already be reported or answered in issues or discussions.
3. **Check the FAQ** below for common answers.
4. **Use the right labels** when opening issues so we can triage faster.

---

## FAQ

**Where can I get MacAppUpdater?**  
From our website: [cycleruncode.club](https://cycleruncode.club).

**Where is the full documentation?**  
Inside the app: use **Help → MacAppUpdater Help** (or the help entry point in the app). The in-app Help has a lot of detail—getting started, scanning, server sync, Sparkle and Mac App Store behaviour, keyboard shortcuts, settings, troubleshooting, and privacy—so check there first for deep dives.

**Is it free?**  
Right now the app is free while we are in active development. We plan to introduce a subscription once we are out of beta; we will announce that on the website and in the app.

**What versions of macOS are supported?**  
macOS 14 (Sonoma) or later. We support both Intel and Apple Silicon.

**Why is my app not showing up after a scan?**  
We only scan `/Applications` (and optionally `/System/Applications` in settings). Apps installed elsewhere (e.g. in your home folder) will not appear. If an app is in `/Applications` and still missing, try a full rescan (⌘R) and check that Full Disk Access is granted in System Settings → Privacy & Security.

**I see a warning about MacAppUpdater “modifying apps”. Does it change my other apps?**  
No. MacAppUpdater only *reads* app metadata (names, versions, bundle IDs, etc.). It never writes to or modifies other applications. The warning is macOS’s generic notice for any app that has Full Disk Access.

**What data does MacAppUpdater send or store?**  
When checking for updates we send app metadata only (names, versions, bundle IDs, macOS version, architecture). We do not send account IDs, emails, or anything that identifies you. The server stores aggregate app/version data for update checks and does not store per-user or per-device data.

**Does it work offline?**  
Yes. You can scan and browse your app list offline. Update checks are queued and run when you are back online.

---

## Support

- **Website:** [cycleruncode.club](https://cycleruncode.club)
- **Email:** [support@cycleruncode.club](mailto:support@cycleruncode.club)
- **Bugs and feature requests:** Open an issue in this repository

---

## Labels we use

We use [GitHub’s default labels](https://docs.github.com/en/issues/using-labels-and-milestones-to-track-work/managing-labels) plus a few conventions so issues are easy to filter and triage.

| Label | When to use | Example |
|-------|--------------|--------|
| `bug` | Unexpected problem or unintended behaviour in the app | “Rescan crashes with 500+ apps”, “Outdated tab empty after updating an app” |
| `enhancement` | New feature or improvement you would like to see | “Bulk select and update multiple apps”, “Menu bar icon with update count” |
| `documentation` | Improvements or additions to docs or in-app Help | “Help says X but app does Y”, “Add a section on Sparkle update formats” |
| `question` | General question or you need more information | “Does this work with Homebrew?”, “Where is the database stored?” |
| `good first issue` | Small, well-scoped issue we think is ideal for first-time contributors (we add this) | “Fix typo in README”, “Clarify a FAQ answer” |
| `help wanted` | We would welcome community help (e.g. wording, suggestions, FAQ ideas) (we add this) | “Suggest clearer wording for this section”, “Propose a new FAQ entry” |
| `duplicate` | Same topic as an existing issue (we add this when closing) | Same as #42 |
| `wontfix` | We have decided not to implement or change this (we add this when closing) | Out of scope or not something we will do |
| `invalid` | Issue or discussion no longer relevant (we add this when closing) | Report was for wrong app, or issue is resolved and thread is noise |

### Templates for common labels

When you open a new issue, you can copy and paste one of these templates into the description and fill it in. This keeps reports consistent and makes it easier for us to help.

#### `bug` report template

```markdown
**Summary**
A short, clear description of the bug.

**Steps to reproduce**
1. …
2. …
3. …

**Expected behaviour**
What you thought would happen.

**Actual behaviour**
What actually happened, including any error messages.

**Environment**
- macOS version:
- MacAppUpdater version:
- How you installed MacAppUpdater (website / other):
- Anything else that might be relevant (number of apps, network set-up, screenshots, logs, etc.):
```

#### `enhancement` / feature request template

```markdown
**Problem**
What you are trying to achieve, or what feels painful or missing.

**Proposed solution**
What you would like MacAppUpdater to do.

**Alternatives you have considered**
Any other approaches or workarounds you have tried or thought about.

**Additional context**
Screenshots, rough mock-ups, or anything else that helps explain the idea.
```

#### `documentation` template

```markdown
**Page or section**
Where in the documentation or in-app Help the problem is (if you know).

**Current wording or behaviour**
What it says or does now.

**Suggested wording or change**
What you think it should say or do instead.

**Why this matters**
How the change would make things clearer or more accurate.
```

#### `question` template

```markdown
**Question**
What you would like to know.

**Context**
Anything about your set-up or goal that might affect the answer (macOS version, how you use MacAppUpdater, etc.).

**What you have already tried**
Search terms you used, FAQ entries or docs you read, or experiments you have already done.
```

We may add **priority** or **resolution** labels later; for now we keep to this set so it stays simple and consistent with what people expect on GitHub.

---

## Code of conduct

Please keep things respectful and constructive. We are a small team and we use this repository to make the app better for everyone.

---

MacAppUpdater is made by [CycleRunCode](https://cycleruncode.club). If you find it useful, you can [buy us a coffee](https://buymeacoffee.com/vksvicky).
