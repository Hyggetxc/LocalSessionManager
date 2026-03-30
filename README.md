# LocalSessionManager

这是一个单文件本地工具，用来查看 `~/.codex` 里的会话内容，不依赖当前账号左侧历史是否展示。

在线预览：
`https://hyggetxc.github.io/LocalSessionManager/`

仓库地址：
`https://github.com/Hyggetxc/LocalSessionManager`

## 用法

1. 用 Chromium 浏览器打开 [`index.html`](/Users/lemon/Documents/project/Codex%20PJ/LocalSessionManager/index.html)
2. 点“选择 `.codex` 目录”
3. 选择你的本地 `~/.codex`
4. 左侧筛选会话，右侧直接查看完整对话

## 当前支持

- 扫描 `sessions` 和 `archived_sessions`
- 按项目、标题、内容、ID 搜索
- 按归档状态筛选
- 查看完整对话内容
- 查看会话元数据
- 查看原始 JSONL 事件
- 查看同项目下的其他会话
- 生成可复制或下载的交接包，方便切换账号后继续上下文

## 说明

- 数据只在浏览器本地处理
- 这个工具解决的是“本地会话还在，但 Codex 客户端左侧不展示”的问题
- 它不会把会话重新导入当前账号左侧历史列表
