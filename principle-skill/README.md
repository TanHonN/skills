# Principle Skill

`principle-skill` 是一组跨领域通用原则 skill，聚焦事物分析、问题分析、信息组织和迭代推进。

## 组成 Skill

- `principle-object-analysis`：用于从对象结构以及时间和空间维度分析事物。
- `principle-problem-solution`：用于从业务领域、问题或需求出发，逐步推进问题分析、方案形成、实现和反馈。
- `principle-information-organization`：用于根据信息关注点确定分类、层级、顺序、用途和归位方式。
- `principle-iterative-process`：用于以已有结果和执行中获得的新信息为下一轮输入，组织少量核心任务逐轮推进并收敛。

## 安装

从远程仓库安装：

```bash
npx skills add https://github.com/hsen-uiro/principle-skill.git -g -a universal --skill '*' -y
npx skills add git@github.com:hsen-uiro/principle-skill.git -g -a universal --skill '*' -y
```

更新本仓库或全局更新：

```bash
npx skills update principle-object-analysis principle-problem-solution principle-information-organization principle-iterative-process -g -y
npx skills update -g -y
```

卸载本项目 skill：

```bash
npx skills remove principle-object-analysis principle-problem-solution principle-information-organization principle-iterative-process -g -a universal -y
```
