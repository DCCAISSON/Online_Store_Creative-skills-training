# Creative Skills Training Design System

## 1. Atmosphere & Identity

这是一个安静、具体、以作品为导向的职业技能培训目录。页面的签名是“课程内容先于营销口号”：每个课程都说明学习主题、练习项目和交付方式，让跨境客户能够快速判断课程是否适合自己。

## 2. Color

### Palette

| Role | Token | Light | Dark | Usage |
|------|-------|-------|------|-------|
| Surface/primary | --surface-primary | #F7F4ED | #1F211F | 页面背景 |
| Surface/elevated | --surface-elevated | #FFFFFF | #2A2C29 | 课程与联系面板 |
| Surface/soft | --surface-soft | #E6EEE9 | #303832 | 强调区背景 |
| Surface/header | --surface-header | rgba(247,244,237,.94) | rgba(31,33,31,.94) | 固定导航背景 |
| Surface/contact | --surface-contact | rgba(255,255,255,.72) | rgba(42,44,41,.72) | 联系面板背景 |
| Text/primary | --text-primary | #151515 | #F7F4ED | 标题和正文 |
| Text/lead | --text-lead | #3E3D39 | #D8DDD8 | 首屏和深色区说明 |
| Text/secondary | --text-secondary | #66625A | #B9B8B0 | 辅助说明 |
| Text/inverse | --text-inverse | #FFFFFF | #151515 | 深色区文字 |
| Text/footer | --text-footer | #DDDDDD | #999999 | 页脚文字 |
| Border/default | --border-default | #D8D2C8 | #4A4D48 | 卡片和分隔线 |
| Border/dark | --border-dark | #3D403C | #3D403C | 深色区分隔线 |
| Border/contact | --border-contact | rgba(31,79,70,.25) | rgba(159,194,184,.25) | 联系面板边框 |
| Accent/primary | --accent-primary | #1F4F46 | #9FC2B8 | 标签、链接和重点数字 |
| Accent/hover | --accent-hover | #173B35 | #B5D4CA | 交互悬停 |
| Accent/soft-border | --accent-soft-border | #B7C8C1 | #B7C8C1 | 重点课程边框 |

### Rules

- 页面不使用渐变、阴影或装饰性彩色光斑。
- 深色区使用整段背景，不用阴影制造层级。
- 强调色只用于可交互元素、标签和课程编号。

## 3. Typography

| Level | Size | Weight | Line Height | Usage |
|-------|------|--------|-------------|-------|
| Display | clamp(48px, 7vw, 88px) | 700 | 1.02 | 首屏标题 |
| H1 | clamp(36px, 5vw, 64px) | 700 | 1.08 | 区块标题 |
| H2 | 28px | 600 | 1.25 | 课程标题 |
| Body/lg | 18px | 400 | 1.6 | 首屏说明 |
| Body | 16px | 400 | 1.6 | 正文 |
| Body/sm | 14px | 400 | 1.5 | 课程元信息 |
| Caption | 12px | 600 | 1.4 | 标签和编号 |

字体使用 `DM Sans` 作为界面字体，`Playfair Display` 作为英文展示标题，中文由系统无衬线字体回退。项目只使用两组字体。

## 4. Spacing & Layout

间距以 4px 为基础单位，主要使用 8、16、24、32、40、48、64、80 和 96px。内容最大宽度为 1120px，桌面端使用双栏或三栏布局，768px 以下改为单栏，640px 以下导航改为可换行布局。

## 5. Components

### Course Card

- **Structure**: 编号、课程名称、中文说明、课程范围、交付形式。
- **Variants**: 基础课程、应用课程、定制培训。
- **Spacing**: 24px 内边距，32px 卡片间距。
- **States**: 默认、悬停、键盘聚焦。
- **Accessibility**: 使用 article、标题层级和可见焦点环。

### Price Card

- **Structure**: 课程档位、学费、适用对象、交付内容。
- **Variants**: 基础、应用、定制。
- **Spacing**: 24px 内边距，16px 信息间距。
- **States**: 默认、重点课程悬停、键盘聚焦。

### Process Row

- **Structure**: 步骤编号、步骤名称、交付说明。
- **Spacing**: 16px 垂直内边距，顶部边框分隔。
- **Accessibility**: 使用有序列表表达流程。

## 6. Motion & Interaction

按钮和卡片只使用 200ms 的颜色与 transform 变化；不改变布局尺寸。所有链接和按钮有 hover、active、focus-visible 状态。`prefers-reduced-motion` 开启时关闭平滑滚动和非必要过渡。

## 7. Depth & Surface

采用 **borders-only** 策略。卡片用 1px 边框分隔，页面区块用背景色区分，不使用 box-shadow。
