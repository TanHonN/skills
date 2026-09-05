# Shop Skill

`shop-skill` 是一组兼容 Agent Skills 格式的购物辅助技能集合，用于沉淀国内电商购物中的通用概念口径和购物推荐能力。

## 组成 Skill

- `shop-concept`：解释和统一国内电商购物通用概念，例如店铺类型、商品规格、价格优惠、服务保障和可信信号。
- `shop-recommend`：根据用户描述的问题、场景或需求推荐可解决问题的物品类型和品牌方向。

## 安装

从远程仓库安装：

```bash
npx skills add https://github.com/TanHonN/shop-skill.git -g -a universal --skill '*' -y
npx skills add git@github.com:TanHonN/shop-skill.git -g -a universal --skill '*' -y
```

更新本仓库或全局更新：

```bash
npx skills update shop-concept shop-recommend -g -y
npx skills update -g -y
```

卸载本项目 skill：

```bash
npx skills remove shop-concept shop-recommend -g -a universal -y
```
