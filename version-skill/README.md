# Version Skill

`version-skill` 是一组用于形成、组织和维护仓库版本的 skill 集合。

## 组成 Skill

- `version-commit`：用于检查 Git 仓库改动、确认提交方案并完成本地提交和远程同步。

## 安装

从远程仓库安装：

```bash
npx skills add https://github.com/hsen-uiro/version-skill.git -g -a universal --skill '*' -y
npx skills add git@github.com:hsen-uiro/version-skill.git -g -a universal --skill '*' -y
```

更新本仓库或全局更新：

```bash
npx skills update version-commit -g -y
npx skills update -g -y
```

卸载本项目 skill：

```bash
npx skills remove version-commit -g -a universal -y
```
