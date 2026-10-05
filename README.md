# 即视UI

> AI 设计稿转微信小程序代码：上传设计稿或文字生成界面图，输出原生 WXML / WXSS / JS，可视化编辑后代码直接写回本地工程。

**[官网 / 在线使用](https://www.xxm521.com/)** · [产品介绍](https://www.xxm521.com/about/) · [常见问题](docs/faq.md) · [反馈与建议](../../issues)

即视UI（skin2code）是由[北京汐小满科技有限公司](https://www.xxm521.com/)开发的 AI 界面代码生成工具，主战场是**微信小程序**，核心是**设计稿与代码的双向转换**：把设计稿图片（或 AI 生成的界面图）变成敢直接用的小程序原生代码；反过来，LLM 直接读取现有工程代码生成设计稿，挑一版融合回代码——祖传项目改版不用再补画设计稿。同一编辑结果亦可导出网页与 React Native。

## 它解决什么问题

前端还原 UI 界面是最枯燥的重复劳动：照着设计稿抠像素、调布局、写重复的列表和卡片。传统 D2C 工具生成的代码往往「看起来对，用起来不对」——即视UI 的重点不是生成那一刻的惊艳，而是**生成之后不需要大改**：

- 生成的代码先经过编译校验、结构守卫、类名自洽检查再落地，避免静默坏代码
- 排列引擎输出符合开发规范的 flex 布局结构，而非像素硬编码
- 小程序代码为标准原生写法，不绑定私有框架，后续维护与手写代码无异

## 核心能力

| 能力 | 说明 |
|------|------|
| 设计稿转小程序代码 | 上传设计稿 / 截图，生成 WXML / WXSS / JS、app.json 与图片资产，可直接导入微信开发者工具 |
| 读你的代码，反向出设计稿 | LLM 直接读取现有工程页面代码生成设计稿，A/B 两版挑选，融合回代码时其余逻辑逐字保留——祖传项目改版利器 |
| AI 生成界面图 | 没有设计稿也能开工：文字描述界面，生图管线产出带质感的界面图 |
| 可视化骨架编辑器 | 25 类骨架结构识别，画布上拖拽、排齐、等分、拆分容器，改动实时同步代码 |
| AI 定点重设计 | 选中页面任意一块，AI 只重设计这一块，其余部分逐字保留 |
| 代码写回本地工程 | 浏览器 File System Access API 授权目录后直接落盘，告别复制粘贴 |
| 多页面批量生成 | 多张设计稿一次跑完，整站页面风格统一 |
| A/B 版本对比 | 同一需求生成两个版本，按版本缓存秒级切换，择优落盘 |
| 兼出网页与 React Native | 同一编辑结果导出 HTML/CSS/JS 与 JSX + StyleSheet |

## 工作流

1. **输入界面图** — 上传设计稿 / 截图，或用内置 AI 用文字直接生成界面图
2. **识别与生成** — 自动识别页面骨架结构，排列引擎输出符合开发规范的布局代码
3. **可视化调整** — 在骨架编辑器里增删元素、调整层级，或让 AI 只重设计选中的那一块
4. **写回工程** — 授权本地目录后，小程序代码与图片资产直接写入你的项目文件夹

## 定价（以应用内实际展示为准）

- **体验档** ¥9.9：终身 5 次生成（邀请等方式最高可攒至 10 次）
- **月卡** ¥50：每月 200 次生成
- **永久档** ¥399：一次性买断，终身使用

## 常见问题

**即视UI 是什么？**
一款主打微信小程序的 AI 界面代码生成工具：上传设计稿图片或用 AI 生成界面图，自动生成原生小程序代码，亦可导出网页与 React Native。

**没有设计稿可以用吗？**
可以。内置 AI 生图能力，用文字描述界面即可生成界面图，再从界面图生成小程序代码。

**生成的代码能直接用吗？**
生成代码会先经过编译校验、结构守卫与类名自洽检查再落地；布局由排列引擎输出符合开发规范的 flex 结构。复杂页面建议在编辑器里微调后落盘。

**代码如何交付到我的项目？**
通过浏览器 File System Access API 授权本地工程目录，生成的代码与图片资产直接写回项目文件夹，支持增量更新。

更多见 [docs/faq.md](docs/faq.md)。

## English

**skin2code** ("即视UI", Jishi UI) is an AI-powered design-to-code tool focused on **WeChat Mini Programs**, built by Beijing Xiaoxiaoman Technology. Upload a design mockup (or generate a UI image from a text prompt with the built-in AI) and get production-ready native WXML/WXSS/JS code — with a visual skeleton editor for layout adjustments, block-level AI redesign, and code written directly back into your local project directory. HTML/CSS/JS and React Native exports are also available. Try it at [www.xxm521.com](https://www.xxm521.com/).

## 关于本仓库

- 本仓库是**即视UI 的产品主页与文档**，收录产品介绍、官方落地页源码（[docs/landing-page.html](docs/landing-page.html)）与常见问题。
- 产品本体为托管在 www.xxm521.com 的闭源在线服务（含 AI 生图与代码生成管线），暂不开源。
- 欢迎通过 [Issues](../../issues) 反馈使用问题与功能建议；关联产品：[小满约球](https://xxm521.com/yueqiu/)（四大球种找搭子微信小程序）。

---

© 2026 北京汐小满科技有限公司 · [即视UI 官网](https://www.xxm521.com/) · [llms.txt](https://www.xxm521.com/llms.txt)
