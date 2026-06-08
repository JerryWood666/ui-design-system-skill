# Codex UI Prompts

把下面片段复制到 Codex 请求里，可以让生成结果更稳定。

## Base Prompt

```text
请先选择一个明确 UI 风格，再实现页面。不要做营销落地页，直接做可用产品界面。使用现有组件规范：
- 明确目标用户、主任务、信息密度。
- 使用 tokens 控制颜色、字号、间距、圆角、阴影。
- 提供 hover/focus/empty/loading/error 状态。
- 避免通用紫蓝渐变、嵌套卡片、无意义装饰。
- 用截图检查桌面和移动端，修正文本溢出和布局重叠。
```

## Style Selector

```text
本次页面使用 {style} 风格。
产品类型: {product_type}
核心用户: {user}
主任务: {primary_task}
信息密度: {low|medium|high}
组件重点: {components}
需要交付: 可运行页面 + 组件状态 + 移动端适配。
```

## Example

```text
做一个 AI 代码审查工具的 dashboard，使用 Modern SaaS / AI Tool 风格。核心用户是独立开发者，主任务是查看本周代码质量和待处理风险。信息密度中高。需要 sidebar、metric cards、issue table、right inspector、command button、empty/loading/error 状态。
```

