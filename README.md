# UI 布局审美 Skill

[![version](https://img.shields.io/badge/version-0.3-blue?style=flat-square)](https://github.com/linyi-ui/ui-layout-skill/releases) [![license](https://img.shields.io/badge/license-MIT-green?style=flat-square)](https://github.com/linyi-ui/ui-layout-skill/blob/main/LICENSE) [![designs](https://img.shields.io/badge/设计点-12_个-orange?style=flat-square)](https://github.com/linyi-ui/ui-layout-skill/blob/main/skills/ui-layout/references/designs.md)

给 AI 编码助手（Claude Code、Codex、Cursor 等）用的网页布局审美技能包。

**装上之后，AI 做页面排版时会自动用上真实获奖网站拆出来的设计手法，而不是"一眼就是 AI 默认排版"。**

设计点库会跟着抖音视频每期更新。

---

## 快速开始

### 安装

**方式一：通用安装（Claude Code、Codex、Cursor 等都支持）**

```bash
npx skills add https://github.com/linyi-ui/ui-layout-skill
```

**方式二：Claude Code 插件**

在 Claude Code 里依次输入：

```
/plugin marketplace add linyi-ui/ui-layout-skill
/plugin install ui-layout@ui-layout
```

### 使用

装好后，在对话里直接说：

> 用 ui-layout 帮我排一个产品官网首屏
> 这个首屏看着很普通，用 ui-layout 的手法改一改
> 做一个相机品牌的落地页，用 ui-layout 里配色克制的那种风格

**AI 会按设计点库里的具体数值（色号、占比、字重）来排版，不用你再手动描述。**

---

## 不装 skill 也能用

每期视频拆的网站案例和提示词都整理在 `prompts/` 文件夹，直接复制给 AI 也行：

| 期 | 主题 | 提示词 |
|---|---|---|
| 第01期 | 35mm 胶片相机站首屏：配色极度克制、标题顶满边缘、线稿3D模型不填色 | [拆一个好看的首屏.md](prompts/拆一个好看的首屏.md) |
| 第02期 | 拆2个真实交互：按住触发物理反馈、悬停切视频、点击筛选重排 | [拆2个真实交互.md](prompts/拆2个真实交互.md) |
| 第03期 | 两种网站两种美学：标题当锚点、错落照片墙、框架无彩、大字当背景、整屏换色、小报营养版 | [两种网站两种美学.md](prompts/两种网站两种美学.md) |

---

## 设计点库（skill 内置）

装了 skill 的话，AI 会自动按这些设计点的完整参数实现，你只需要说想要什么风格：

| 编号 | 设计点 | 适用场景 |
|---|---|---|
| 01 | 配色极度克制 2 Colors Only | 想要"精密仪器感"、高级感的首屏；强调色只出现一次 |
| 02 | 标题顶满边缘 Edge-to-Edge Type | 想要标题成为画面主体，而不是规规矩矩缩在中间 |
| 03 | 线稿3D模型不填色 Wireframe 3D | 想要科技感/精密感的产品展示，比真实照片更有参与感 |
| 04 | 按住触发物理反馈 Press-and-Hold Physics（跨界：偏交互） | 技术型工作室想证明实力，不想堆文案自夸 |
| 05 | 同模型换材质 Material Swap on Same Model（跨界：偏交互） | 首屏3D主视觉想用一套模型讲两种调性 |
| 06 | 点击筛选重排 Filter-and-Reflow（跨界：偏交互） | 案例多且杂，想不跳页就能快速对比分类 |
| 07 | 标题当锚点 Anchor Title | 年度回顾/时间线长页面，滚着滚着会迷路 |
| 08 | 错落照片墙 Scatter Wall | 作品集/图集想要随手翻相册的松弛感 |
| 09 | 框架无彩 Mono Frame | 以照片为主角，想让照片色彩最大化跳出来 |
| 10 | 大字当背景 Type as Background | 产品造型普通，想靠排版制造冲击力 |
| 11 | 整屏换色 Full-screen Swatch | 多口味/多型号系列展示，滚动像翻色卡 |
| 12 | 小报营养版 Tabloid Nutrition | 枯燥的营养表/参数也想带上品牌个性 |

完整参数和使用场景见 [designs.md](skills/ui-layout/references/designs.md)。

## 核心能力

1. **场景自动匹配**：说出你想要的排版感觉，AI 从设计点库里挑最合适的手法 —— 见 [SKILL.md](skills/ui-layout/SKILL.md) 的场景判断表
2. **参数有真实依据**：色号、占比、字重都是从真实获奖网站量出来的具体数值，不是"好看一点"这种模糊描述 —— 见 [designs.md](skills/ui-layout/references/designs.md)
3. **反模板感自检**：交付前按清单检查，避免做出"一眼 AI 感"的排版 —— 见 [anti-template.md](skills/ui-layout/references/anti-template.md)

## 更新记录

- **v0.1**（第01期）：首次发布。新增 3 个设计点（配色极度克制、标题顶满边缘、线稿3D模型不填色），来源案例：35mm 胶片相机站首屏。
- **v0.2**（第02期）：新增 3 个设计点（按住触发物理反馈、同模型换材质、点击筛选重排），来源案例：Anubi（意大利CGI工作室站）+ Red Antler（纽约广告代理商站）。这3个设计点偏交互行为，和 ui-motion 栏目有交集，仍收在 ui-layout 里。
- **v0.3**（第03期）：新增 6 个设计点（标题当锚点、错落照片墙、框架无彩、大字当背景、整屏换色、小报营养版），来源案例：Better Off（年度回顾站，极致克制）+ Henrietta Said（辣味零食站，极致张扬）。一期拆两种相反的排版美学：前三个讲"克制"怎么让内容跳出来，后三个讲"张扬"怎么靠排版制造记忆点。

## 许可证

MIT
