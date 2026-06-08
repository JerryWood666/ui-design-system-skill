# UI Design System Skill

一个面向独立开发者和 Codex 工作流的 UI 规范库。它把审美判断、组件规则、页面范式和 Codex 可执行提示沉淀成可复用 skill，帮助你在大型软件开发中先约定风格，再稳定生成高质量 UI。

## 适合什么时候用

- 你正在用 Codex 开发 Web/App/桌面软件，需要更稳定的 UI 审美。
- 你已经约定了风格，例如 Apple-like、Modern SaaS、中式古典、企业后台。
- 你希望 Codex 在实现页面前先加载风格规范、组件规则和验收标准。
- 你想把 shadcn/ui、Radix、Headless UI 这类能力变成自己的可复用设计系统。

## 安装到 Codex

将 skill 目录复制到 Codex skills 目录：

```bash
mkdir -p ~/.codex/skills
cp -R skills/ui-design-system ~/.codex/skills/
```

之后在 Codex 中这样调用：

```text
使用 $ui-design-system。我要做一个 AI 代码审查工具，风格选择 Modern SaaS / AI Tool。请先加载对应风格规则，再实现 dashboard、issue table、right inspector 和 empty/loading/error 状态。
```

或者：

```text
使用 $ui-design-system。我要做一个中式古典风格的文旅内容产品，不要堆纹样，重点是宣纸、宋体、朱砂、注释栏和阅读节奏。请实现首页和文章页。
```

## 仓库结构

```text
.
├── skills/ui-design-system/       # Codex skill，可复制安装
│   ├── SKILL.md                   # 运行时工作流
│   ├── agents/openai.yaml         # Codex UI 元数据
│   ├── references/                # 风格、组件、prompt 规范
│   └── assets/                    # tokens 和 HTML 样例
├── docs/                          # 面向人的规范文档
├── tokens/                        # 根目录 demo 使用的共享 CSS tokens
├── examples/                      # 可直接打开的 HTML 样例
└── screenshots/                   # 桌面和移动端截图
```

## GitHub / 开源生态参考

- [shadcn/ui](https://github.com/shadcn-ui/ui): 可复制源码的组件分发方式，适合构建自己的组件库。
- [Radix Primitives](https://github.com/radix-ui/primitives): 低层、可访问、无样式交互基座。
- [Headless UI](https://github.com/tailwindlabs/headlessui): 无样式、可访问组件，适合 Tailwind 生态。
- [Mantine](https://github.com/mantinedev/mantine): 完整 React 组件与 hooks 库，适合快速开发。
- [Ant Design](https://github.com/ant-design/ant-design): 企业级中后台和数据密集型产品参考。
- [MUI](https://github.com/mui/material-ui): 成熟 Material Design 组件体系。
- [HeroUI](https://github.com/heroui-inc/heroui): 现代 React/Tailwind 组件库，适合 SaaS 与 AI 产品。

## 核心规范

- [风格谱系](./docs/UI_STYLE_TAXONOMY.md)
- [组件规范](./docs/UI_COMPONENT_SPEC.md)
- [Codex 使用提示](./docs/CODEX_UI_PROMPTS.md)
- [共享 CSS tokens](./tokens/ui-tokens.css)
- [HTML 样例入口](./examples/index.html)

## HTML 样例

这些页面是静态 HTML，可以直接打开 [examples/index.html](./examples/index.html)。

### Modern SaaS / AI Tool

适合 AI 工具、开发者工具、代码审查、自动化工作台。

![Modern SaaS desktop](./screenshots/modern-saas-desktop.png)

### Apple-like Productivity

适合个人效率、日程、创作者工具和 macOS 气质应用。

![Apple-like mobile](./screenshots/apple-productivity-mobile.png)

### Chinese Classical

适合文旅、茶、书法、古籍、内容产品。重点是宣纸、宋体、朱砂、注释栏和留白，不是堆纹样。

![Chinese Classical desktop](./screenshots/chinese-classical-desktop.png)

### Admin Console

适合企业后台、订单、CRM、运营系统、数据密集型产品。

![Admin Console mobile](./screenshots/admin-console-mobile.png)

## 推荐工作流

1. 先让 Codex 使用 `$ui-design-system` 选择或确认风格。
2. 再让 Codex 读取风格谱系和组件规范。
3. 实现页面时要求包含组件状态和响应式。
4. 最后用截图验收桌面和移动端。

## 验证记录

已用 Playwright 对 5 个页面进行 1366px 桌面和 390px 移动端截图检查，未发现页面级横向溢出。截图保存在 [screenshots](./screenshots)。
