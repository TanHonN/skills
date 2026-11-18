# Experimental Skills

`experimental-skills` 是正在开发、验证或尚未完成稳定发布准备的个人 skill 聚合仓库。

## Skill 集合

仓库按 `<集合名>/<skill-name>/` 组织具体 skill；集合目录保留自己的 README，必要时可直接包含集合级辅助入口；集合说明和 skill 清单由对应集合 README 承载。

- [life-skill](life-skill/)：生活购物比价和浏览器自动化。

## 获取仓库

```bash
git clone https://github.com/TanHonN/skills.git
```

## 安装

当前使用 `npx skills` 从聚合仓库安装全部实验 skill：

```bash
npx skills add https://github.com/TanHonN/skills.git --full-depth -g -a universal --skill '*' -y
```

更新已安装的 skill：

```bash
npx skills update -g -y
```

源仓库删除或改名后，更新不会自动清理本地旧 skill；需要按旧名称显式执行 `npx skills remove <skill-name> -g -a universal -y`。

本仓库承载开发和验证中的 skill 集合；skill 稳定后，可以将对应集合迁入 `official-skills`，再按成熟仓库的维护规则处理。
