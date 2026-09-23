# OpenCode 极客高清主题 (pi.theme.opencode)

移植 OpenCode 编辑器标志性排版方案的 PI-Desktop 主题插件，专注提升技术长文、排错日志与代码讲解的阅读清晰度。

## 特性

- **专业等宽字体栈**：全局覆盖 `--font-mono`，按 `JetBrains Mono → Cascadia Code → Fira Code → Consolas → Menlo → Monaco` 顺序回退，行内代码与多行代码块均享受更清晰的字形区分（`0` / `O`、`1` / `l` / `I` 不再混淆）。
- **OpenCode 紫罗兰分级标题**：
  - Dark：H1 深天青 `#38bdf8`，H2 紫罗兰 `#c084fc`，H3 淡紫 `#a78bfa`，H4–H6 靛蓝 `#818cf8`，H1/H2 带同色系下边框。
  - Light：H1 深天青 `#0284c7`，H2 深紫罗兰 `#7e22ce`，H3 `#6d28d9`，H4–H6 `#4338ca`。
- **薄荷绿行内代码**：Dark 使用 `#4ade80` 文字配 `12%` 透明底色，Light 使用 `#15803d` 深绿，行内代码区块边界一目了然。
  - 选择器严格限定 `:not(pre) > code` / `p > code` / `li > code` / `td > code`，**不会覆盖多行代码块的语法高亮**。
- **强调色体系**：
  - Dark：加粗 `#fde047` 亮黄、斜体 `#f472b6` 粉、列表标记 `#fb923c` 橙、引用块紫色左边框 `#a855f7`、链接 `#60a5fa`。
  - Light：加粗 `#b45309` 琥珀金、列表标记 `#ea580c` 深橙、引用块 `#7e22ce` 深紫边框、链接 `#1d4ed8`。
- **表格与代码块增强**：表头带主色底纹、斑马纹与悬浮高亮；代码块容器深色 `#14141e` / 浅色 `#f6f7fb`，配紫罗兰描边与 8px 圆角。

## 包含主题

| 主题 ID | 名称 | 基础模式 | 样式文件 |
| --- | --- | --- | --- |
| `opencode-dark` | OpenCode Dark (清晰紫绿) | dark | `themes/opencode-dark.css` |
| `opencode-light` | OpenCode Light (清爽高彩) | light | `themes/opencode-light.css` |

## 安装与启用

1. 打开 PI-Desktop，进入 **设置 → 主题**。
2. 在主题列表中找到 **OpenCode Dark (清晰紫绿)** 或 **OpenCode Light (清爽高彩)**。
3. 点击即可立即生效；切换回内置主题也无需重启。
4. 若列表中未显示，可在 **设置 → 插件** 中确认 `pi.theme.opencode` 处于启用状态后重新打开主题页。

## 权限

- `ui.theme`：注册并应用主题样式表。主题仅注入 CSS 变量与排版规则，不含脚本、外部请求或网络资源。

## 安全说明

两个样式文件均为纯 CSS，满足以下约束：

- 无 `@import`
- 无外部 `url()`
- 无 `<style>` 标签或任何脚本
