# LocalSessionManager

[![GitHub Stars](https://img.shields.io/github/stars/Hyggetxc/LocalSessionManager?style=flat-square)](https://github.com/Hyggetxc/LocalSessionManager/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/Hyggetxc/LocalSessionManager?style=flat-square)](https://github.com/Hyggetxc/LocalSessionManager/network/members)
[![GitHub Issues](https://img.shields.io/github/issues/Hyggetxc/LocalSessionManager?style=flat-square)](https://github.com/Hyggetxc/LocalSessionManager/issues)
[![GitHub Pages](https://img.shields.io/badge/demo-online-2f81f7?style=flat-square)](https://hyggetxc.github.io/LocalSessionManager/)

LocalSessionManager 是一个轻量级的本地 Codex 会话查看器，用来直接读取 `~/.codex` 中的会话文件。

它尤其适合下面这些场景：

- 你在使用多个 Codex 账号
- 一些本地会话明明还在磁盘里，但当前账号下的 Codex 侧边栏没有完整展示出来
- 你想直接查看本地完整对话内容
- 你准备切换到另一个 Codex 账号继续工作，希望生成一份交接包，不用重新讲一遍上下文

## 语言

- [English](./README.md)
- [简体中文](./README.zh-CN.md)

## 在线地址

- 在线预览：[https://hyggetxc.github.io/LocalSessionManager/](https://hyggetxc.github.io/LocalSessionManager/)
- 仓库地址：[https://github.com/Hyggetxc/LocalSessionManager](https://github.com/Hyggetxc/LocalSessionManager)

## 这个工具解决什么问题

很多时候，Codex 的本地会话数据其实还在这些位置：

- `~/.codex/sessions`
- `~/.codex/archived_sessions`
- `~/.codex/session_index.jsonl`

但当前登录账号不一定会把这些历史完整展示在桌面端左侧列表里。

这个工具就是这个问题的补充解决方案：  
它不依赖当前账号侧边栏是否显示，而是直接在浏览器里读取本地会话文件，帮你把“本地还在但 UI 没显示”的会话找出来；如果你要切换到另一个账号继续协作，也可以直接生成交接包。

## 功能特性

- 扫描本地 `sessions` 和 `archived_sessions`
- 按标题、内容、会话 ID、项目目录搜索
- 按归档状态和项目筛选
- 以更干净的网页界面查看完整对话
- 查看元数据和原始 JSONL 事件
- 查看同项目下的其他会话
- 复制或下载交接包，方便切换到新的 Codex 账号继续工作
- 支持浅色 / 深色主题与中英文界面

## 使用方式

1. 用 Chromium 内核浏览器打开 [`index.html`](./index.html)
2. 点击 `选择 .codex 目录`
3. 选择本地 `~/.codex` 目录
4. 左侧筛选和选择会话，右侧查看完整对话
5. 如果你要切换账号继续，就使用 `复制交接包` 或 `下载交接包 .txt`

## 隐私说明

- 所有数据都只在浏览器本地处理
- 这个工具不会主动上传你的会话内容
- 它不会把会话重新导入到当前 Codex 账号的左侧历史列表

## 仓库后续扩展

这个仓库完全可以继续像一些成熟开源项目一样，逐步增加更多目录和组件。

后续很适合增加：

- `docs/`：放截图、FAQ、恢复说明
- `examples/`：放示例交接包或示例数据
- `scripts/`：放发布脚本或本地辅助工具
- `components/` 或 `packages/`：如果以后不想继续维持单文件结构，可以拆出可复用模块

## 支持一下

如果这个工具真的帮你找回了本地会话，或者帮你完成了多账号交接，欢迎给仓库点个 Star：

- [给这个仓库点个 Star](https://github.com/Hyggetxc/LocalSessionManager)
