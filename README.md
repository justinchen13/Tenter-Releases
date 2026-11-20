<p align="center">
  <strong>English</strong> · <a href="README.zh-CN.md">简体中文</a>
</p>

<p align="center">
  <a href="https://tenter.build">
    <img src=".github/assets/tenter-mark.png" alt="Tenter logo" width="88" height="88">
  </a>
</p>

<h1 align="center">Tenter</h1>

<p align="center">
  <strong>Keep your product moving. Build. Maintain. Stay in control.</strong><br>
  Work on several cross-repo changes at once, each in its own workspace.
</p>

<p align="center">
  <a href="https://github.com/justinchen13/Tenter-Releases/releases/latest"><img alt="Latest release" src="https://img.shields.io/github/v/release/justinchen13/Tenter-Releases?sort=semver&label=release&color=FF5533"></a>
  <a href="https://discord.gg/SdVeMghYvH"><img alt="Discord" src="https://img.shields.io/badge/Discord-join-5865F2?logo=discord&logoColor=white"></a>
  <a href="https://x.com/tenterbuild"><img alt="X" src="https://img.shields.io/badge/@tenterbuild-follow-111111?logo=x&logoColor=white"></a>
</p>

<p align="center">
  <a href="https://tenter.build/en/download"><strong>Download for macOS</strong></a> ·
  <a href="https://tenter.build">Website</a> ·
  <a href="https://tenter.build/en/docs">Docs</a> ·
  <a href="https://github.com/justinchen13/Tenter-Releases/releases">Release notes</a>
</p>

<p align="center">
  <img src=".github/assets/workbench.webp" alt="Tenter workbench: project groups on the left, an agent session in the middle, and every repository's branch and PR status on the right" width="900">
</p>

## What is Tenter?

Tenter brings your product's repositories and shared materials together. You can work on several changes across the same repositories at once, then review and deliver each change separately.

### A workspace for each change

Open a workspace with the repositories and materials a change needs. Each repository has its own Git worktree and branch, and one agent session can work across them. Set access per repository to Writable, Reference (read-only), or Disabled. The system sandbox enforces those settings.

### Review and deliver each change

Review all repository diffs for a change in one workspace. Use `/pr` to open or update a PR for each changed repository on GitHub, GitLab, or Gitea. Merge with `/merge` or automation you enable.

<p align="center">
  <img src=".github/assets/delivery.webp" alt="Git panel showing a branch and pull request for each repository in the workspace" width="820">
</p>

### Follow progress across workspaces

The [Control Center](https://tenter.build/en/docs/guides/control-center) brings progress and blockers into one conversation. With takeover enabled, it can handle routine questions and approvals within the permissions you grant and bring back decisions that need your input.

<p align="center">
  <img src=".github/assets/coordination.webp" alt="Control Center following updates from conversations across several products" width="820">
</p>

### Keep project context for the next change

In [project management](https://tenter.build/en/docs/guides/project-management), tasks and bugs link to the workspaces where the work happens. Servers, domains, and devices keep their own [asset memory](https://tenter.build/en/docs/reference/assets), so agents can consult existing operating notes the next time they use them.

<p align="center">
  <img src=".github/assets/planning.webp" alt="Project management board with a task opened and linked to its workspace" width="820">
</p>

## Download

| Platform | Requirements | Download |
| --- | --- | --- |
| macOS | macOS 12 or later, Apple Silicon (M-series) | [Download the DMG](https://tenter.build/en/download) |
| Mobile | — | Coming soon |

You can also get the installer (`Tenter_<version>_aarch64.dmg`) directly from the [latest release](https://github.com/justinchen13/Tenter-Releases/releases/latest). Intel Macs are not supported.

## Getting started

1. Open the DMG and drag **Tenter** into **Applications**.
2. Launch Tenter and wait for it to prepare its managed Claude Code and Codex runtimes. You do not need to install those CLIs yourself.
3. Open **Settings → Providers**, choose Claude Code or Codex, and sign in with your subscription or add an API key.
4. [Connect your Git hosting platform](https://tenter.build/en/docs/git-setup), add a project repository, and [start your first task](https://tenter.build/en/docs/first-task).

Keep Git and your projects' own development tools installed locally. See the [installation guide](https://tenter.build/en/docs/installation) for details.

## Updates

Tenter updates itself. Open **Settings → About → Check for updates**, then restart right away or choose **Restart when idle** to let running agents finish first. Release notes for every version are on the [Releases page](https://github.com/justinchen13/Tenter-Releases/releases).

## Feedback

[Open an issue](https://github.com/justinchen13/Tenter-Releases/issues/new/choose) and choose **Bug report** or **Feature request**. You can also send feedback from inside the app.

- **Bug report**: describe what happened, the expected result, and any known reproduction steps or environment details (Tenter version, macOS version, model service).
- **Feature request**: describe your workflow, the difficulty you face, and the result you would like to achieve.

Before reporting, check the [troubleshooting guide](https://tenter.build/en/docs/troubleshooting/issues) and search [existing issues](https://github.com/justinchen13/Tenter-Releases/issues) to avoid duplicates.

> [!IMPORTANT]
> Issues and attachments are public. Review screenshots and diagnostic logs and remove sensitive information before sharing them.

## Community and contact

- **Discord**: join the [Tenter community](https://discord.gg/SdVeMghYvH) to exchange workflows and experiences.
- **X**: follow [@tenterbuild](https://x.com/tenterbuild) for product news.
- **Partnerships**: email [tenter.build@gmail.com](mailto:tenter.build@gmail.com).

## Maintaining feedback

The two web forms live in `.github/ISSUE_TEMPLATE/`. Keep the `bug` and `enhancement` repository labels available so GitHub can apply each form's configured label.

Titles use `[Bug]: ` and `[Feature]: ` prefixes. Application submissions use the same prefixes so their category remains identifiable even when the submitting account cannot apply labels. Maintainers can adjust the category and labels during triage.

These templates become available on GitHub after they are merged into the repository's default branch. This repository does not automatically publish issues, upload logs, or run classification workflows.
