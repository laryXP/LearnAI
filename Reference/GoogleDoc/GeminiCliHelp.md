# 📘Gemini CLI 基础操作

## 基础功能（Basics）

- **添加上下文**：使用 `@` 指定文件作为上下文，例如`@src/myFile.ts`（可以作用于单个文件或整个文件夹）
- **Shell 模式**：执行 Shell 命令用 `!` 开头，例如`!npm run start`， 也可以用自然语言，例如直接发送 “start server”（模型会自动理解为执行 server 命令）

---

## 命令（Commands）

- **`/about`** ：显示版本信息

- **`/auth`** ：更改认证方式

- **`/bug`** ：提交 bug 报告

---

### `/chat` 对话管理

- `list` — 列出保存的对话检查点
- `save <tag>` — 保存当前对话为一个检查点
- `resume <tag>` — 从某个检查点恢复对话
- `delete <tag>` — 删除一个检查点
- `share <file>` — 将当前对话导出为 markdown 或 json 文件

---

### `/clear` 清屏并清除对话历史

### `/compress` 压缩当前上下文，将其替换为总结摘要

### `/copy` 将上一次生成的结果或代码复制到剪贴板

### `/docs` 在浏览器打开完整 Gemini CLI 文档

---

### `/directory` 工作区目录管理

- `add` — 添加目录到工作区（多个路径用逗号分隔）
- `show` — 显示工作区中的所有目录

---

### `/editor` 设置外部编辑器偏好

---

### `/extensions` 扩展管理

- `list` — 列出所有启用的扩展
- `update <name>|--all` — 更新指定扩展或全部扩展
- `explore` — 在浏览器中打开扩展页面
- `restart` — 重启所有扩展

---

### `/help`

显示 Gemini CLI 帮助

---

### `/ide`

管理 IDE 集成

---

### `/init`

分析项目并生成一个定制的 `GEMINI.md`

---

### `/mcp`（Model Context Protocol）管理 MCP 服务器

- `list` — 列出已配置的 MCP 服务器和工具
- `desc` — 列出所有 MCP 服务器与工具的说明
- `schema` — 列出所有 MCP 服务器与工具的说明和 schema
- `auth` — 为启用 OAuth 的 MCP 服务器执行认证
- `refresh` — 重启 MCP 服务器

---

### `/memory` 记忆系统管理

- `show` — 查看当前记忆内容
- `add` — 添加内容到记忆
- `refresh` — 从存储源刷新记忆
- `list` — 列出当前使用的 GEMINI.md 文件路径

---

### `/model`

打开对话框以配置当前使用的模型

---

### `/privacy`

显示隐私声明

---

### `/quit`

退出 CLI

---

### `/stats`

查看会话统计信息
用法：`/stats [model|tools]`

- `model` — 显示模型使用统计
- `tools` — 显示工具调用统计

---

### `/theme`

更改 CLI 主题风格

---

### `/tools`

列出可用的 Gemini CLI 工具
用法：`/tools [desc]`

---

### `/settings`

查看和编辑 Gemini CLI 设置

---

### `/vim`

开启或关闭 Vim 模式

---

### `/setup-github`

设置 GitHub Actions

---

### `/terminal-setup`

为多行输入配置终端按键绑定（VS Code、Cursor、Windsurf）

---

### `!`

执行 Shell 命令

---

### `[MCP]`

外部 MCP 服务器提供的命令

---

# ⌨️ **键盘快捷键（Keyboard Shortcuts）**

- **Alt + 左/右** — 输入框中按词移动
- **Ctrl + C** — 退出应用
- **Ctrl + Enter** — 输入新行
- **Ctrl + L** — 清屏
- **Ctrl + S** — 进入选择模式以复制文本
- **Ctrl + X** — 在外部编辑器中打开输入
- **Ctrl + Y** — 切换 YOLO 模式（自动执行可能危险的操作）
- **Enter** — 发送消息
- **Esc** — 取消操作 / 双击清空输入
- **Page Up / Page Down** — 上下翻页
- **Shift + Tab** — 切换自动接受编辑
- **Up/Down** — 在历史提示中切换
