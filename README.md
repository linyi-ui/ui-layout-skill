# UI 布局审美 Skill

[![version](https://img.shields.io/badge/version-0.2-blue?style=flat-square)](https://github.com/linyi-ui/ui-layout-skill/releases) [![license](https://img.shields.io/badge/license-MIT-green?style=flat-square)](https://github.com/linyi-ui/ui-layout-skill/blob/main/LICENSE) [![designs](https://img.shields.io/badge/设计点-7_个-orange?style=flat-square)](https://github.com/linyi-ui/ui-layout-skill/blob/main/skills/ui-layout/references/designs.md)

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
| 第02期 | 2个网站首屏颜色反差：衬线大字压天空、九成淡色+一处高饱和点缀、树枝镂空露材质、照片当背景色、超粗圆体无衬线标题、品牌名弧形排布 | [2个网站首屏颜色反差.md](prompts/2个网站首屏颜色反差.md) |

---

## 设计点库（skill 内置）

装了 skill 的话，AI 会自动按这些设计点的完整参数实现，你只需要说想要什么风格：

| 编号 | 设计点 | 适用场景 |
|---|---|---|
| 01 | 配色极度克制 2 Colors Only | 想要"精密仪器感"、高级感的首屏；强调色只出现一次 |
| 02 | 标题顶满边缘 Edge-to-Edge Type | 想要标题成为画面主体，而不是规规矩矩缩在中间 |
| 03 | 线稿3D模型不填色 Wireframe 3D | 想要科技感/精密感的产品展示，比真实照片更有参与感 |
| 04 | 衬线大字压天空 Serif Title Over Sky | 建筑/地产/人文类标题想要和实景图融为一体 |
| 05 | 九成淡色+一处高饱和点缀 90% Muted + One Accent | 想要克制高级但留一点彩色呼吸感 |
| 06 | 照片当背景色 Photo As Background Color | 某个色块区域想要比纯色更有质感 |
| 07 | 品牌名弧形排布 Arc Text Layout | 品牌名/标题想要比直排多一点俏皮感、亲和力 |

完整参数和使用场景见 [designs.md](skills/ui-layout/references/designs.md)。

## 核心能力

1. **场景自动匹配**：说出你想要的排版感觉，AI 从设计点库里挑最合适的手法 —— 见 [SKILL.md](skills/ui-layout/SKILL.md) 的场景判断表
2. **参数有真实依据**：色号、占比、字重都是从真实获奖网站量出来的具体数值，不是"好看一点"这种模糊描述 —— 见 [designs.md](skills/ui-layout/references/designs.md)
3. **反模板感自检**：交付前按清单检查，避免做出"一眼 AI 感"的排版 —— 见 [anti-template.md](skills/ui-layout/references/anti-template.md)

## 更新记录

- **v0.1**（第01期）：首次发布。新增 3 个设计点（配色极度克制、标题顶满边缘、线稿3D模型不填色），来源案例：35mm 胶片相机站首屏。
- **v0.2**（第02期）：新增 4 个设计点（衬线大字压天空、九成淡色+一处高饱和点缀、照片当背景色、品牌名弧形排布），来源案例：建筑3D展示站 + 番茄品牌页脚站。

## 许可证

MIT
