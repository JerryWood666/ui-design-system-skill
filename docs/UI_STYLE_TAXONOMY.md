# UI Style Taxonomy

这份风格谱系用于在写代码前建立明确审美方向。每种风格都应该落到 tokens、组件、页面模板和验收标准，而不只是形容词。

使用方式：先根据产品类型和用户场景选择 1 个主风格；如果需要混合，只允许加入 1 个辅助风格，并明确哪些部分继承辅助风格。

## 01 Modern SaaS / AI Tool

适合 AI 工具、开发者工具、轻量 B2B SaaS、自动化工作台。

- 关键词: 清晰、冷静、锋利、命令面板、细边框、低装饰。
- 布局: 左侧导航、顶部工具栏、工作区主面板、右侧属性栏。
- 色彩: 中性灰、墨黑、冷白，配一个高识别 accent。
- 字体: 干净无衬线，标题略紧凑，正文高可读。
- 组件: Command menu、Tabs、Table、Inspector、Toast、Popover。
- 禁忌: 大面积紫蓝渐变、营销页式英雄区、过度圆角卡片。

## 02 Apple-like Productivity

适合 macOS/iOS 气质的个人效率工具、创作者工具、日程与任务应用。

- 关键词: 空气感、半透明、精密、系统感、轻阴影。
- 布局: 大留白、浮动工具栏、分栏视图、内容优先。
- 色彩: 近白背景、浅灰层级、蓝色或绿色系统强调色。
- 字体: 系统字体或接近系统字体的高可读无衬线。
- 组件: Segmented control、Sidebar、Toolbar、Sheet、List、Calendar。
- 禁忌: 强烈阴影、过重边框、复杂纹理。

## 03 Enterprise Admin

适合 CRM、ERP、BI、运营后台、配置系统、权限管理。

- 关键词: 信息密度、可扫描、稳定、流程、权限。
- 布局: 顶栏 + 侧边栏 + 表格/筛选区 + 批量操作。
- 色彩: 白底、浅灰区隔、蓝色主操作、状态色清晰。
- 字体: 高可读无衬线，数字等宽或 tabular nums。
- 组件: Data table、Filter bar、Form、Drawer、Batch action、Status tag。
- 禁忌: 装饰性大图、过大标题、低信息密度。

## 04 Material / Google-like

适合通用移动应用、跨平台产品、教育工具、消费级应用。

- 关键词: 清楚层级、卡片、标准动效、友好、可预测。
- 布局: App bar、内容卡片、底部导航、清晰浮层。
- 色彩: 明亮底色、明确主色、状态色规范。
- 字体: 几何无衬线，层级清楚，正文舒适。
- 组件: FAB、Card、Bottom navigation、Snackbar、Date picker。
- 禁忌: 卡片过多导致页面碎片化，阴影层级混乱。

## 05 Microsoft Fluent / Office

适合桌面软件、协作文档、企业办公、知识工作台。

- 关键词: 深度、半透明、工具栏、办公感、精致状态。
- 布局: Ribbon/toolbar、侧边栏、文档区、右侧属性面板。
- 色彩: 中性灰、蓝色主色、柔和背景、轻玻璃感。
- 字体: 系统无衬线，文字层级清楚，控件紧凑。
- 组件: Toolbar、Context menu、Pane、Tree view、Command bar。
- 禁忌: 玻璃效果过强、装饰超过办公效率。

## 06 Notion / Document Workspace

适合知识库、笔记、文档协作、项目资料库、块编辑器。

- 关键词: 内容优先、低装饰、块结构、可编辑、轻量。
- 布局: 侧边文档树、正文编辑区、块级操作、评论侧栏。
- 色彩: 白底或浅灰底，低饱和强调色，弱边框。
- 字体: 高可读正文，标题克制，长文舒适。
- 组件: Block editor、Breadcrumb、Mention、Comment、Database view。
- 禁忌: 把文档界面做成卡片墙，过多颜色标签。

## 07 Linear / Developer Tool

适合 issue 管理、路线图、代码协作、开发者生产力软件。

- 关键词: 快捷键、暗色、细线、速度、列表优先。
- 布局: Sidebar、List、Detail pane、Command center、Keyboard flow。
- 色彩: 深灰/近黑、冷白文字、单一高亮色。
- 字体: 紧凑无衬线，数字和状态清晰。
- 组件: Issue list、Command menu、Status selector、Shortcut hint、Activity feed。
- 禁忌: 低效大卡片、营销化空话、过度插画。

## 08 Data / Finance

适合交易、财务、数据分析、指标监控、风控系统。

- 关键词: 数字优先、紧凑、风险感、实时状态。
- 布局: KPI 条、图表矩阵、筛选器、详情抽屉。
- 色彩: 深浅均可，红绿/蓝橙状态必须一致。
- 字体: 数字使用等宽或 tabular nums。
- 组件: Metric card、Sparkline、Heatmap、Ticker、Alert。
- 禁忌: 花哨图表、状态色混乱、数字没有单位。

## 09 Industrial Console

适合 DevOps、IoT、监控、工程控制台、设备管理。

- 关键词: 网格、状态灯、模块化、终端感、仪表。
- 布局: 密集 dashboard、可折叠面板、日志区域。
- 色彩: 深灰、荧光绿/青、警示橙。
- 字体: 无衬线 + 等宽数字/日志。
- 组件: Log stream、Gauge、Status chip、Node map、Control panel。
- 禁忌: 牺牲可读性的纯黑和过亮霓虹。

## 10 Cyberpunk / Hacker

适合安全工具、黑客主题、科幻产品、活动页、游戏周边。

- 关键词: 霓虹、终端、扫描线、故障感、未来城市。
- 布局: 强对比分区、命令行区域、地图/网络拓扑、警报条。
- 色彩: 黑底、青/紫/红霓虹、少量警示黄。
- 字体: 等宽或机械感字体，标题可更锋利。
- 组件: Terminal、Threat card、Network graph、Alert rail、Access panel。
- 禁忌: 低对比霓虹文字、动画过多影响阅读。

## 11 Chinese Classical

适合传统文化、茶、书法、文旅、古籍、内容型产品。

- 关键词: 宣纸、留白、水墨、印章红、宋体、纵横节奏。
- 布局: 屏风式分栏、卷轴式阅读、题跋/注释区。
- 色彩: 米白、墨黑、朱砂、石青、竹青。
- 字体: 中文标题可用宋体/楷体气质，正文要保持现代可读。
- 组件: Article card、Catalog、Seal button、Timeline、Annotation。
- 禁忌: 把传统纹样贴满屏幕、低对比浅棕、伪古董质感。

## 12 New Chinese / Guochao

适合国潮品牌、年轻消费品、文化电商、节庆活动。

- 关键词: 传统符号现代化、强色块、东方几何、年轻化。
- 布局: 大标题、符号化图形、产品展示、节奏强的分屏。
- 色彩: 朱红、靛蓝、金、玉绿、黑白强对比。
- 字体: 现代黑体搭配少量书法/宋体标题。
- 组件: Product card、Campaign banner、Badge、Story section、Coupon。
- 禁忌: 元素堆砌、廉价国潮贴纸感、色彩无主次。

## 13 Japanese Minimal / Wabi-sabi

适合生活方式、手作、摄影、空间、茶、民宿、慢内容。

- 关键词: 安静、自然材质、低饱和、非对称、留白。
- 布局: 单列或少列、稀疏内容、图片与文字保持呼吸。
- 色彩: 米白、灰褐、炭黑、苔绿、木色。
- 字体: 克制无衬线或细衬线，字号层级少。
- 组件: Gallery、Journal card、Reservation form、Product detail。
- 禁忌: 高饱和颜色、复杂动效、密集营销组件。

## 14 Korean Soft Commerce

适合美妆、服饰、生活方式电商、轻消费品牌。

- 关键词: 柔和、干净、亲和、轻时尚、精致卡片。
- 布局: 商品网格、浅色 banner、轻量筛选、社交证明。
- 色彩: 奶白、浅粉、雾蓝、鼠尾草绿、淡灰。
- 字体: 圆润无衬线，价格和标签清楚。
- 组件: Product tile、Swatch、Review card、Wishlist、Promo strip。
- 禁忌: 过度甜腻、低对比浅色文字、商品信息不清。

## 15 Editorial / Magazine

适合博客、作品集、内容产品、研究报告、媒体专题。

- 关键词: 强排版、图文节奏、大标题、非对称、栏目感。
- 布局: 多列网格、跨栏标题、图片与文字错位。
- 色彩: 黑白为主，局部高饱和点缀。
- 字体: 标题可用衬线或强性格字体，正文注重阅读。
- 组件: Feature story、Quote、Index、Author card、Reading progress。
- 禁忌: 所有内容都放卡片、标题层级无节奏。

## 16 Luxury / Premium Brand

适合高端服务、品牌官网、作品陈列、奢侈品、精品酒店。

- 关键词: 克制、材质感、衬线、低饱和、慢节奏。
- 布局: 大图、强留白、少量文本、精确对齐。
- 色彩: 黑、象牙白、香槟金、深绿、酒红。
- 字体: 高质量衬线 + 克制无衬线。
- 组件: Lookbook grid、Product detail、Reservation form、Gallery。
- 禁忌: 抢眼按钮过多、廉价渐变、拥挤布局。

## 17 Neo Brutalism

适合年轻化产品、创意工具、活动页、实验性个人项目。

- 关键词: 粗边框、硬阴影、高饱和、直接、有态度。
- 布局: 大块撞色、明显网格、强烈按钮。
- 色彩: 黑白硬边界，高饱和黄/粉/蓝/绿。
- 字体: 粗体无衬线，标题直接有力。
- 组件: Loud button、Sticker card、Step blocks、Badge。
- 禁忌: 用在严肃金融/医疗场景，或可访问性对比不足。

## 18 Brutalist / Raw Web

适合开发者个人站、实验项目、反精致品牌、艺术页面。

- 关键词: 原始、直接、低修饰、默认控件、结构裸露。
- 布局: 文档式结构、明显链接、表格、朴素分隔线。
- 色彩: 黑白灰为主，可加入单一强烈强调色。
- 字体: 系统字体、等宽字体、少量粗体。
- 组件: Plain table、Text link、Directory list、Raw form、Index page。
- 禁忌: 误把未完成当风格，缺少信息层级。

## 19 Retro / Y2K / Pixel

适合小游戏、个人站、怀旧产品、创意活动、音乐/潮流页面。

- 关键词: 像素、复古窗口、贴纸、低保真、怀旧科技。
- 布局: 桌面窗口、像素面板、弹窗、收藏夹/播放器结构。
- 色彩: 高饱和蓝粉绿、银灰、CRT 深色。
- 字体: 像素字体或复古无衬线，正文要可读。
- 组件: Window、Pixel button、Player、Badge、Inventory grid。
- 禁忌: 像素字体用于长正文，动效闪烁过强。

## 20 Playful / Toy-like

适合儿童教育、轻量工具、学习产品、娱乐化应用。

- 关键词: 友好、圆润、弹性、明亮、鼓励感。
- 布局: 大按钮、清晰步骤、可视反馈、角色/插画辅助。
- 色彩: 明亮但分层，避免整页彩虹。
- 字体: 圆润无衬线，字号偏大，行距舒适。
- 组件: Progress path、Reward card、Big CTA、Quiz card、Mascot panel。
- 禁忌: 幼稚化严肃任务，动画过多拖慢操作。

## 21 Calm Health

适合健康、心理、冥想、睡眠、生活方式工具。

- 关键词: 温和、低刺激、安心、清楚引导。
- 布局: 分步引导、低密度、单一主任务。
- 色彩: 柔和绿、蓝、米白、淡紫灰。
- 字体: 温和无衬线，正文宽松，错误信息不刺眼。
- 组件: Stepper、Check-in card、Progress、Reminder、Journal input。
- 禁忌: 高压促销、错误状态过于刺眼。

## 22 Education / Learning

适合在线课程、知识训练、题库、学习社区、训练营。

- 关键词: 清晰、进度、鼓励、结构化、可持续学习。
- 布局: 课程目录、学习主区、练习区、进度侧栏。
- 色彩: 可信蓝/绿为主，奖励色适度。
- 字体: 高可读正文，代码/公式使用专门样式。
- 组件: Lesson card、Quiz、Progress bar、Note panel、Achievement。
- 禁忌: 游戏化过度、学习路径不清、反馈延迟。

## 23 Government / Public Service

适合政务、公共服务、公益、教育公共系统、办事平台。

- 关键词: 可信、清楚、无障碍、稳重、流程明确。
- 布局: 信息公告、办事入口、步骤流程、搜索与分类。
- 色彩: 白底、深蓝/红/绿主色，状态色克制。
- 字体: 极高可读性，字号和对比要充足。
- 组件: Service card、Process step、Notice、Search、Form wizard。
- 禁忌: 花哨视觉、低对比、隐藏关键流程。

## 24 Gaming / Immersive

适合游戏门户、游戏内工具、互动活动、虚拟世界产品。

- 关键词: 沉浸、场景感、状态、奖励、强反馈。
- 布局: 全屏主场景、HUD、任务栏、背包/卡牌/排行榜。
- 色彩: 根据题材定调，必须有明确主色和危险/奖励色。
- 字体: 标题可风格化，正文和数值必须易读。
- 组件: HUD、Quest card、Inventory、Leaderboard、Reward modal。
- 禁忌: 装饰遮挡信息、特效影响操作、移动端按钮过小。

## Mixing Rules

- 一个页面最多 1 个主风格 + 1 个辅助风格。
- 后台/工具类产品优先保证效率，再考虑表达性。
- 内容/品牌类产品优先建立记忆点，但不能牺牲阅读和转化。
- 行业类产品优先尊重用户预期，例如金融要稳、医疗要安心、政务要清楚。
- 不确定时先输出 2-3 个风格方向，让用户选择后再实现。
