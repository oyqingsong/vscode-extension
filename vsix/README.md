# VS Code 离线扩展包

本目录收集了常用 VS Code 扩展的 `.vsix` 文件，适用于**离线环境**或**网络受限**情况下安装。

## 如何使用

在 VS Code 中按 `Ctrl+Shift+P` 打开命令面板，选择 **"Extensions: Install from VSIX..."**，然后选择对应的 `.vsix` 文件即可安装。

## 扩展列表

| 扩展 | 版本 | 大小 | 说明 |
|------|------|------|------|
| [CodeSnap](https://marketplace.visualstudio.com/items?itemName=adpyke.codesnap) | 1.3.4 | 2.6 MB | 快速生成美观的代码截图，用于分享或文档 |
| [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) | 3.0.24 | 257 KB | 集成 ESLint，提供 JS/TS 代码静态检查与自动修复 |
| [ES7+ React/Redux/React-Native snippets](https://marketplace.visualstudio.com/items?itemName=dsznajder.es7-react-js-snippets) | 4.4.3 | 4.6 MB | React/Redux 代码片段，提升开发效率 |
| [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) | 12.4.0 | 3.5 MB | 代码格式化工具，支持多种语言 |
| [Auto Close Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-close-tag) | 0.5.15 | 773 KB | 自动闭合 HTML/JSX 标签 |
| [Auto Rename Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag) | 0.1.10 | 662 KB | 自动同步修改 HTML/JSX 配对标签 |
| [Git Graph](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph) | 1.30.0 | 346 KB | 可视化的 Git 分支图谱与操作界面 |
| [CSS Peek](https://marketplace.visualstudio.com/items?itemName=pranaygp.vscode-css-peek) | 4.4.3 | 6.6 MB | 在 HTML 中跳转到 CSS 定义位置，支持 Peek/Go to Definition |
| [vscode-icons](https://marketplace.visualstudio.com/items?itemName=vscode-icons-team.vscode-icons) | 12.18.0 | 2.3 MB | 为不同文件类型提供图标标识，提升文件浏览体验 |
| [Todo Highlight](https://marketplace.visualstudio.com/items?itemName=wayou.vscode-todo-highlight) | 1.0.5 | 1.3 MB | 高亮代码中的 TODO/FIXME 等注释标记 |
| [One Dark Pro](https://marketplace.visualstudio.com/items?itemName=zhuangtongfa.material-theme) | 3.19.0 | 310 KB | 经典的 Atom One Dark 主题 |

## 分类

### 代码质量
- **ESLint** — 静态代码检查
- **Prettier** — 代码格式化

### 前端开发
- **Auto Close Tag** / **Auto Rename Tag** — HTML/JSX 标签操作
- **ES7+ React snippets** — React 相关代码片段
- **CSS Peek** — 样式定义跳转

### 可视化与主题
- **vscode-icons** — 文件图标主题
- **One Dark Pro** — 颜色主题
- **CodeSnap** — 代码截图

### 效率工具
- **Git Graph** — Git 历史可视化
- **Todo Highlight** — 待办注释高亮

## 批量安装

可通过命令行批量安装所有扩展：

```bash
# Windows (PowerShell)
Get-ChildItem -Path . -Filter *.vsix | ForEach-Object { code --install-extension $_.FullName }

# macOS / Linux
for f in *.vsix; do code --install-extension "$f"; done
```
