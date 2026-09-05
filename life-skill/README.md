# Life Skill

`life-skill` 是一组兼容 Agent Skills 格式的生活辅助技能集合，用于把购物比价、浏览器循环任务、幕布编辑和 JetBrains 库 API 学习等任务拆成可复用、可触发的 agent skill。

## 组成 Skill

- `life-shop`：在京东、拼多多、淘宝/天猫、抖音商城等主流电商平台中搜索可信同款商品，并输出跨平台比价结果。
- `life-browser-automation`：为用户授权页面中需要循环等待、低频重试或持续监控的任务编写并执行 Playwright 自动化脚本。
- `life-mubu-edit`：在用户指定的可操作浏览器环境中安全编辑已打开的幕布大纲文档，逐节点更新、整理和校验内容。
- `note-jetbrains-code`：通过 JetBrains IDE 或 JetBrains MCP 学习当前工程中的公开 API。

## 安装

从远程仓库安装：

```bash
npx skills add https://github.com/hsen-uiro/life-skill.git -g -a universal --skill '*' -y
npx skills add git@github.com:hsen-uiro/life-skill.git -g -a universal --skill '*' -y
```

更新本仓库或全局更新：

```bash
npx skills update life-shop life-browser-automation life-mubu-edit note-jetbrains-code -g -y
npx skills update -g -y
```

卸载本项目 skill：

```bash
npx skills remove life-shop life-browser-automation life-mubu-edit note-jetbrains-code -g -a universal -y
```
