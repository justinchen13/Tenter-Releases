<p align="center">
  <a href="README.md">English</a> · <strong>简体中文</strong>
</p>

<p align="center">
  <a href="https://tenter.build/zh-CN">
    <img src=".github/assets/tenter-mark.png" alt="Tenter 标志" width="88" height="88">
  </a>
</p>

<h1 align="center">Tenter</h1>

<p align="center">
  <strong>让产品持续向前。开发与维护，尽在掌握。</strong><br>
  为全栈工程师和超级个体设计的 AI 工作台，一台 Mac 同时推进多个产品。
</p>

<p align="center">
  <a href="https://github.com/justinchen13/Tenter-Releases/releases/latest"><img alt="最新版本" src="https://img.shields.io/github/v/release/justinchen13/Tenter-Releases?sort=semver&label=release&color=FF5533"></a>
  <img alt="macOS 12+，Apple Silicon" src="https://img.shields.io/badge/macOS%2012%2B-Apple%20Silicon-111111?logo=apple&logoColor=white">
  <a href="https://discord.gg/SdVeMghYvH"><img alt="Discord" src="https://img.shields.io/badge/Discord-join-5865F2?logo=discord&logoColor=white"></a>
  <a href="https://x.com/tenterbuild"><img alt="X" src="https://img.shields.io/badge/@tenterbuild-follow-111111?logo=x&logoColor=white"></a>
</p>

<p align="center">
  <a href="https://tenter.build/zh-CN/download"><strong>下载 macOS 版</strong></a> ·
  <a href="https://tenter.build/zh-CN">官网</a> ·
  <a href="https://tenter.build/zh-CN/docs">使用文档</a> ·
  <a href="https://github.com/justinchen13/Tenter-Releases/releases">更新日志</a>
</p>

<p align="center">
  <img src=".github/assets/workbench-zh-CN.webp" alt="Tenter 工作台：左侧是项目组，中间是 Agent 会话，右侧是每个仓库的分支与 PR 状态" width="900">
</p>

本仓库发布 Tenter 官方 macOS 安装包，并收集公开的问题反馈与功能建议。Tenter 的源代码不在这里公开。

## Tenter 是什么？

Tenter 是一个 macOS 应用，在一个地方组织产品的仓库、资料和 AI 工作，让一个人也能像整个团队一样，同时推进多个产品。使用你自己的 Claude 或 Codex 账号，Tenter 让它们并行工作。

### 并行工作，工作区互相隔离

每个任务都有独立的 worktree 和会话，Claude 与 Codex 可以同时工作、互不干扰。一个工作区可以覆盖一项改动涉及的所有仓库。

### 中控

目标只需描述一次。中控会拆分和派发工作、跟进每个会话，只把需要你拍板的事情带回来。

<p align="center">
  <img src=".github/assets/coordination-zh-CN.webp" alt="中控汇总来自多个产品会话的进展" width="820">
</p>

### 上下文持续积累

内置的项目管理、记忆、Skills 和资产在工作区之间共享。任务和缺陷关联到正在处理它们的工作区，每个新任务都能接着上一次继续。

<p align="center">
  <img src=".github/assets/planning-zh-CN.webp" alt="项目管理看板，打开的任务关联着对应的工作区" width="820">
</p>

### 从计划到 PR

执行前先审阅计划，完成后在同一流程里审阅改动、提交并创建 Pull Request，每个仓库一个分支、一个 PR。

<p align="center">
  <img src=".github/assets/delivery-zh-CN.webp" alt="Git 面板显示工作区内每个仓库的分支与 Pull Request" width="820">
</p>

## 下载

| 平台 | 系统要求 | 下载 |
| --- | --- | --- |
| macOS | macOS 12 或更高版本，Apple Silicon（M 系列芯片） | [下载 DMG](https://tenter.build/zh-CN/download) |
| 移动端 | — | 即将推出 |

也可以从 [最新版本](https://github.com/justinchen13/Tenter-Releases/releases/latest) 直接下载安装包（`Tenter_<版本号>_aarch64.dmg`）。暂不支持 Intel 芯片的 Mac。

## 快速开始

1. 打开 DMG，把 **Tenter** 拖入「应用程序」（Applications）。
2. 启动 Tenter，等待它准备好受管的 Claude Code 和 Codex 运行时，无需自行安装这些 CLI。
3. 打开 **设置 → 服务商**（Settings → Providers），选择 Claude Code 或 Codex，用已有订阅登录，或添加 API key。
4. [连接 Git 托管平台](https://tenter.build/zh-CN/docs/git-setup)，添加项目仓库，然后 [完成第一个任务](https://tenter.build/zh-CN/docs/first-task)。

本机需要准备 Git 以及项目本身要求的开发工具。详见 [安装与连接模型](https://tenter.build/zh-CN/docs/installation)。

## 更新

Tenter 会自动更新。打开 **设置 → 关于 → 检查更新**，更新准备好后可以立即重启；如果 Agent 还在工作，选择 **空闲时重启并更新**（Restart when idle）。每个版本的更新说明见 [Releases 页面](https://github.com/justinchen13/Tenter-Releases/releases)。

## 反馈

[新建 Issue](https://github.com/justinchen13/Tenter-Releases/issues/new/choose)，选择 **Bug report**（问题反馈）或 **Feature request**（功能建议）。也可以在应用内直接提交反馈。表单为英文，可以用中文填写。

- **问题反馈**：说明发生了什么、你预期的结果，以及已知的复现步骤和环境信息（Tenter 版本、macOS 版本、模型服务）。
- **功能建议**：说明你的工作流程、遇到的困难，以及希望达到的效果。

提交前，建议先查看 [常见问题与排错](https://tenter.build/zh-CN/docs/troubleshooting/issues)，并搜索 [已有 Issue](https://github.com/justinchen13/Tenter-Releases/issues)，避免重复。

> [!IMPORTANT]
> Issue 及其附件会公开可见。分享截图和诊断日志前，请先检查并删除敏感信息。

收到功能建议不代表已排入开发计划。

## 社区与联系

- **Discord**：加入 [Tenter 社区](https://discord.gg/SdVeMghYvH)，交流工作流和使用经验。
- **X**：关注 [@tenterbuild](https://x.com/tenterbuild) 获取产品动态。
- **商务合作**：发送邮件至 [tenter.build@gmail.com](mailto:tenter.build@gmail.com)。

问题反馈和功能建议统一在本仓库跟踪。

## 维护反馈模板

两个网页表单位于 `.github/ISSUE_TEMPLATE/`。请保留仓库的 `bug` 和 `enhancement` 标签，GitHub 才能为每个表单自动加上配置的标签。

标题使用 `[Bug]: ` 和 `[Feature]: ` 前缀。应用内提交也使用相同前缀，即使提交账号无权添加标签，也能识别类别。维护者可以在分类时调整类别和标签。

模板合并到仓库默认分支后才会在 GitHub 上生效。本仓库不会自动发布 Issue、上传日志或运行分类工作流。
