---
name: product-design-system
description: 使用 Product 的七色角色、Inter 字体、8px 网格和可访问组件规则构建响应式 Web 产品界面。
user-invocable: true
---

# Product Design System Skill

## What is inside

- `README.md`：包结构、预览清单与复用流程。
- `DESIGN.md`：颜色、字体、版式、组件、交互、语气与反模式。
- `BRAND.md`：品牌与资产边界。
- `colors_and_type.css`：可直接导入的基础令牌。
- `preview/`：颜色、字体、间距、圆角、资产、按钮和表单的聚焦预览。
- `system/`：引擎派生的 light、dark、compact 主题和组件套件。
- `ui_kits/app/`：响应式应用示例。
- `assets/`：来源明确的原始参考图。

## Source context

系统来源为 `context/input-DESIGN.md` 与四张本地演示页参考图。没有网站、Figma、仓库、字体文件或 logo。不要把参考图中的演示品牌语言误写成真实 Product 业务事实。

Source evidence is local only; no repository, GitHub project or production app was provided.

## When to use this skill

- 创建或改造响应式 Web 产品、控制台、工作台、表单和数据界面。
- 需要 Product 的白色画布、冷灰分组、蓝色交互与克制编辑式层级。
- 需要统一 Button、Card、Form、Navigation 与反馈状态。
- Designed for building interfaces, prototypes and production-oriented artifacts.

## How to use

1. 读取 `README.md` 与 `DESIGN.md`，确认任务与组件范围。
2. 引入 `colors_and_type.css`，从语义角色而不是散落色值开始。
3. 使用 `system/variables.css` 或 `system/theme.json` 接入完整派生令牌。
4. 对照 `preview/` 与 `system/kit.html` 检查浅色状态，对照 `system/kit.dark.html` 检查深色状态。
5. 参考 `ui_kits/app/index.html` 的 44px 控件、焦点环、响应式导航和单主动作。
6. 需要新增资产时保留真实文件与来源；没有证据时使用明确占位，不生成看似真实的替代物。

## Design system highlights

- 七个角色：background、surface、foreground、muted、border、accent、accent-secondary。
- 亮蓝负责链接、焦点和选择；深钴蓝负责承载白字的实心动作。
- Inter 同时服务 display 与 body，中文由系统无衬线回退。
- 8px 基线、8px 圆角、1px 边框、44px 默认控件。
- 白色画布优先，冷灰用于分组，阴影只用于浮层。
- 每个视口一个实心主 CTA；移动端重排而不是缩小。
- Highlights: colors, typography, spacing, radius, layout and interaction states are all source-bound or explicitly marked as inferred.

## Package Boundaries

- `assets/` 是原始图像证据，不能改画成 logo。
- 当前没有 `fonts/`、`build/` 或 `source_examples/`，因为来源未提供相应证据。
- `ui_kits/app/` 是实现样例，不是产品事实或业务承诺。
