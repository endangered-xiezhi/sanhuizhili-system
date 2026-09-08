# 三会智理路演 - Design Spec

## I. Project Information

| Item | Value |
| ---- | ----- |
| **Project Name** | roadshow_ppt |
| **Canvas Format** | PPT 16:9 (1280x720) |
| **Page Count** | 7 |
| **Design Style** | Top Consulting / 科技专业风 |
| **Target Audience** | 评委、投资人、潜在客户 |
| **Use Case** | 路演答辩 |
| **Created Date** | 2026-07-21 |

---

## II. Canvas Specification

| Property | Value |
| -------- | ----- |
| **Format** | PPT 16:9 |
| **Dimensions** | 1280x720 |
| **viewBox** | `0 0 1280 720` |
| **Margins** | 左/右 60px, 上/下 50px |
| **Content Area** | 1160x620 |

---

## III. Visual Theme

### Theme Style

- **Style**: Top Consulting / 科技专业风
- **Theme**: Dark theme (深色模式)
- **Tone**: 前沿、能量感、极客、权威

### Color Scheme

| Role | HEX | Purpose |
| ---- | --- | ------- |
| **Background** | `#1A1A24` | 深空背景 |
| **Secondary bg** | `#2A2A38` | 卡片背景 |
| **Primary** | `#1E3A5F` | 藏青主色，区块划分 |
| **Accent** | `#1565C0` | 科技蓝，高亮指标 |
| **Secondary accent** | `#D4AF37` | 金色点缀 |
| **Body text** | `#F8F9FA` | 正文文字 |
| **Secondary text** | `#B0B0C0` | 辅助文字 |
| **Tertiary text** | `#808090` | 注释 |
| **Border/divider** | `#3A3A4A` | 边框线 |
| **Success** | `#00796B` | 成功/合规 |
| **Warning** | `#C41E3A` | 警告/红线 |

### AI Image Strategy

- **Image Rendering**: 3d-isometric
- **Image Palette**: tech-neon

---

## IV. Typography System

### Font Plan

**Typography direction**: 中式权威与西方学术感融合 (楷体 + Times New Roman)

| Role | Chinese | English | Fallback tail |
| ---- | ------- | ------- | ------------- |
| **Title** | `KaiTi` | `"Times New Roman"` | `serif` |
| **Body** | `KaiTi` | `"Times New Roman"` | `serif` |
| **Emphasis** | `KaiTi` | `"Times New Roman"` | `serif` |
| **Code** | — | `Consolas, "Courier New"` | `monospace` |

**Per-role font stacks**:

- Title: `"Times New Roman", KaiTi, serif`
- Body: `"Times New Roman", KaiTi, serif`
- Emphasis: `"Times New Roman", KaiTi, serif`
- Code: `Consolas, "Courier New", monospace`

### Font Size Hierarchy

**Baseline**: Body font size = 18px

| Purpose | Ratio to body | Example @ body=18 (dense) | Weight |
| ------- | ------------- | ------------------------- | ------ |
| Cover title (hero headline) | 3-4x | 54-72px | Bold |
| Chapter / section opener | 2-2.5x | 36-45px | Bold |
| Page title | 1.5-2x | 27-36px | Bold |
| Hero number (consulting KPIs) | 1.5-2x | 27-36px | Bold |
| Subtitle | 1.2-1.5x | 22-27px | SemiBold |
| **Body content** | **1x** | **18px** | Regular |
| Annotation / caption | 0.85x | 15px | Regular |
| Page number / footnote | 0.65x | 12px | Regular |

---

## V. Layout Principles

### Page Structure

- **Header area**: 顶部 100px (Logo及页面标题)
- **Content area**: 中部 520px
- **Footer area**: 底部 50px (页码及免责声明)

### Spacing Specification

**Universal**:

| Element | Current Project |
| ------- | --------------- |
| Safe margin from canvas edge | 60px |
| Content block gap | 32px |
| Icon-text gap | 12px |

**Card-based layouts**:

| Element | Current Project |
| ------- | --------------- |
| Card gap | 24px |
| Card padding | 24px |
| Card border radius | 12px |

---

## VI. Icon Usage Specification

### Source

- **Built-in icon library**: `templates/icons/`

### Recommended Icon List

| Purpose | Icon Path | Page |
| ------- | --------- | ---- |
| 架构/体系 | `tabler-outline/box-model` | P02 |
| 合规 | `tabler-outline/shield-check` | P03 |
| 规则引擎 | `tabler-outline/engine` | P04 |
| 飞书集成 | `tabler-outline/brand-feishu` | P05 |

---

## VII. Visualization Reference List

(None matched, custom SVG charts if needed)

---

## VIII. Image Resource List

| Filename | Dimensions | Ratio | Purpose | Type | Layout pattern | Acquire Via | Status | Reference | text_policy | page_role |
| -------- | --------- | ----- | ------- | ---- | -------------- | ----------- | ------ | --------- | ----------- | --------- |
| cover_bg.png | 1280x720 | 1.78 | 封面背景 | Background | #1 full-bleed background with floating title + #29 two-stop scrim | ai | Pending | abstract technology network nodes connected by glowing lines | none | hero_page |
| architecture.png | 600x600 | 1.0 | 架构图配图 | Diagram | #44 background image + native network/architecture diagram | ai | Pending | 3D isometric representation of a data processing engine routing information | none | local |

---

## IX. Content Outline

### P01 - 封面页
- **Layout**: Full-screen background image + centered title
- **Title**: 三会智理
- **Subtitle**: 将繁琐留给系统，将合规交予规则
- **Info**: 2026年7月

### P02 - 痛点分析
- **Layout**: 左右分栏对比
- **Title**: 传统公司治理的困境
- **Core message**: 传统合规依靠人工排查，效率低下且容易出错。
- **Content**:
  - 人工审查耗时长，历史决议难追溯。
  - 飞书等多端协同信息零散，缺乏统筹。
  - 合规红线易被忽略，存在极高法律风险。

### P03 - 解决方案：双通道审批
- **Layout**: 上下分栏 / 流程图
- **Title**: 大模型+规则引擎的双通道审查
- **Core message**: 结合确定的规则引擎和兜底的大模型能力，实现精准合规。
- **Content**:
  - 规则引擎：处理明确的、法定的刚性合规要求。
  - 大模型辅助：处理语义模糊的意图识别与风险提示。

### P04 - 技术壁垒：数据不出域
- **Layout**: 中心发散
- **Title**: 飞书原生集成与数据安全
- **Core message**: 深度绑定飞书生态，实现多维表格的自动流转。
- **Content**:
  - 本地化处理，核心数据不出域。
  - 多维表格直接作为数据底座与操作前端。

### P05 - 产品演示 / 核心场景
- **Layout**: 三卡片并列
- **Title**: 典型使用场景
- **Core message**: 满足议题申报、会议表决、会后归档全流程。
- **Content**:
  - 议题智能审查。
  - 决议自动生成。
  - 历史风险关联。

### P06 - 商业模式与展望
- **Layout**: 对称分栏
- **Title**: 商业模式与未来演进
- **Core message**: 采用 SaaS 订阅制，并向多领域拓展。
- **Content**:
  - 面向企业客户的订阅收费。
  - 后续向投融资合规、劳动合规等领域延展。

### P07 - 尾页
- **Layout**: 居中，留白
- **Title**: 谢谢聆听
- **Subtitle**: 期待与您共建智能合规新纪元

---

## X. Speaker Notes Requirements

(To be generated per slide)

## XI. Technical Constraints Reminder
1. viewBox: `0 0 1280 720`
2. Background uses `<rect>` elements
3. Text wrapping uses `<tspan>` (`<foreignObject>` FORBIDDEN)
4. Transparency uses `fill-opacity` / `stroke-opacity`; `rgba()` FORBIDDEN
5. FORBIDDEN: `mask`, `<style>`, `class`, `foreignObject`
