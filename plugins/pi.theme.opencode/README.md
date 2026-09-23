# OpenCode 极客高清主题 (pi.theme.opencode)

1:1 严格对齐 OpenCode 官方源码（`anomalyco/opencode`）调色板与终端排版规范的 PI-Desktop 全局主题插件。专注消除单调的纯黑白字，带来极致清晰的结构分块、技术词汇穿透力与极客终端质感。

## 官方调色板对照（Pixel-Perfect 对齐）

| 语义角色 | OpenCode 官方色值 | 视觉用途 |
| :--- | :--- | :--- |
| **Heading** | `#9d7cd8` (紫罗兰) | 各级标题，紧凑纯净无下划线，结构一目了然 |
| **Code** | `#7fd88f` (薄荷绿) | 行内代码，无冗余底色边框，纯净代码语法穿透 |
| **Strong** | `#f5a742` (暖金琥珀) | 核心重点加粗，一眼抓取结论 |
| **Emph** | `#e5c07b` (小麦暖黄) | 斜体强调与引用块边框 |
| **List Item** | `#fab283` (蜜桃暖橙) | 无序列表项目符号与破折号 |
| **Enumeration**| `#56b6c2` (青蓝色) | 有序列表数字序号（1. 2. 3.） |
| **Background** | `#0a0a0a` (极深纯黑) | 深邃极客底色，彻底告别发灰浮层 |
| **Panels** | `#141414` | 输入框、侧边栏等面板底色 |

## 核心特性

- **全局现代等宽排版**：正文与代码全部统一为 `JetBrains Mono` / `Cascadia Code` / `Fira Code` 等宽栈，字符对齐整齐划一，重现终端 TUI 极客体验。
- **纯净语法高亮穿透**：行内代码遵循官方规范，剔除厚重药丸底色与边框，如同 IDE 语法高亮般自然穿插。
- **排他性安全隔离**：严格通过 `:not(pre) > code` 排他选择器，绝不破坏多行代码块内部的原生语法高亮。
- **双模全天候适配**：提供暗夜极客 `OpenCode Dark` 与清爽高对比 `OpenCode Light`。

## 包含主题

| 主题 ID | 名称 | 模式 | 路径 |
| :--- | :--- | :--- | :--- |
| `opencode-dark` | OpenCode Dark (官方原版) | dark | `themes/opencode-dark.css` |
| `opencode-light` | OpenCode Light (官方原版) | light | `themes/opencode-light.css` |

## 安装与使用

1. 在 PI-Desktop 中安装 `.piplug` 安装包或通过插件市场安装；
2. 进入 **【设置 -> 常规 / 外观 -> 主题】**，下拉选择 **`OpenCode Dark (官方原版)`**；
3. 即刻热生效，无需重启软件。

## 权限与安全

- 仅声明最低风险权限 `ui.theme`；
- 纯离线静态 CSS，无网络请求、无文件读写、无脚本执行；
- 100% 通过 PI-Desktop 官方自动化安全审计（`security_audit.py` 0 blockers）。
