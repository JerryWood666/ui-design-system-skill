# UI Component Spec

组件规范采用“行为优先、视觉可换皮”的方式。复杂交互优先参考 Radix Primitives / Headless UI 的可访问模式，视觉层通过 tokens 控制。

## Token Layers

1. Global tokens: 颜色、字号、间距、圆角、阴影、动效。
2. Semantic tokens: background、surface、text、border、accent、danger、success。
3. Component tokens: button height、input radius、table row height、card padding。
4. Style presets: modern-saas、apple、chinese-classical、admin-console。

## Core Components

### Button

- Variants: primary、secondary、ghost、danger、seal。
- Sizes: sm 32px、md 40px、lg 48px。
- 必须有 hover、active、focus-visible、disabled。
- 图标按钮必须有 `aria-label`。
- 主操作每个区域最多一个。

### Input

- 高度: 40px 默认，复杂后台可用 36px。
- 状态: default、hover、focus、error、disabled。
- 错误文案放在输入框下方，不能只用红色表达。
- 搜索框要支持清空按钮和快捷键提示。

### Card / Panel

- 用于重复实体、工具面板、弹窗内容。
- 不要把页面 section 都做成浮动卡片。
- 半径根据风格变化: admin 6px、modern 12px、apple 18px、classical 2px。
- 卡片内标题不使用 hero 级字体。

### Tabs

- 用于同级视图切换，不用于流程步骤。
- 当前项必须有明确视觉状态。
- 内容区切换不能导致主要布局跳动。

### Table

- 后台表格行高 44-52px。
- 数字右对齐，名称左对齐，状态居中或左对齐。
- 必备状态: loading skeleton、empty、error、selected、hover。
- 批量操作只在选择后出现。

### Modal / Dialog

- 用于确认、短表单、阻塞操作。
- 复杂详情优先 Drawer 或独立页面。
- 必须支持 Esc 关闭、焦点圈定、返回触发点。

### Navigation

- SaaS: sidebar + command menu。
- Apple-like: translucent sidebar + toolbar。
- Classical: catalog + chapter rail。
- Admin: dense sidebar + breadcrumb + tab views。

## Page Acceptance Checklist

- 首屏是否直接呈现真实产品功能，而不是空泛介绍。
- 是否有清晰主任务和一个主要 CTA。
- 文本是否在移动端和桌面端都不溢出。
- hover、focus、disabled、empty、loading、error 是否可见。
- 颜色对比是否满足常规阅读需求。
- 组件尺寸是否稳定，动态内容不会挤压布局。
- 是否避免了模板化紫色渐变和无意义装饰。

