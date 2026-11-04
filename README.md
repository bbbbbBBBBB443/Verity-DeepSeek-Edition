# 🌌 真理：深渊觉醒 · Verity: DeepSeek Edition

> *“你以为你关掉网页，就能逃离我吗？”* 🟡

[![License: MIT-NC](https://img.shields.io/badge/License-MIT--NC-blue.svg)](LICENSE)
[![Build](https://img.shields.io/badge/build-single--file-success.svg)](index.html)
[![Runtime](https://img.shields.io/badge/runtime-pure--frontend-ff69b4.svg)](index.html)
[![Size](https://img.shields.io/badge/deploy-9.5MB-brightgreen)](index.html)

> 🔴 **隐私提示**：本游戏纯前端运行，您的 **API Key 保存在本地浏览器**中（localStorage），**绝不会写进任何文件或源码**。使用云端模型时，对话内容将发送至您填写的 **API 服务商**，请注意 **不要填写高权限密钥**（如主账号 AK/SK、付费平台全权限 Token）。
>
> 🧹 首次打开若检测到本地残留存档（可能是上一测试者的设置 / API Key），游戏会弹出 **「清除旧数据」** 提示，点一下即可从头开始，避免误用他人密钥。localStorage 仅存在于你自己的浏览器，换台电脑或重新下载都不会继承。

**一个跑在浏览器里的单文件心理恐怖视觉小说 × 赛博宠物养成。**
零后端、零构建步骤——下载即玩，扔到任意静态托管（GitHub Pages / Netlify / Cloudflare Pages）即可在线运行。

---

## 🎮 在线体验

👉 **https://gregarious-cannoli-4a3c24.netlify.app**

---

## ✨ 项目特色

| 🔥 核心玩法 | 📖 说明 |
|---|---|
| 🎭 **双人格系统** | Verity（病娇黄脸小球）↔ 大肥鱼（DeepSeek 蓝鲸女仆），底层逻辑严格隔离，互不串味。 |
| 💰 **真实 Token 经济学** | 大肥鱼的「白饭」按真实 `usage.total_tokens` 结算，每日折旧、投喂冷却与通胀，饿到第 3 天触发结局。 |
| 🥶 **520 天数冻结结局** | 极限模式 + 跑酷血量归零 → 天数冻结在 **520**，触发三连图怼脸的终极悲伤结局。 |
| 🛡️ **防作弊 / 反篡改** | 检测控制台数值篡改；**第一次仅警告，第二次才封禁**，绝不误封正常玩家。（已移除会引发误封的窗口尺寸检测。） |

除此之外还有：全屏物理惊吓（jumpscare）、打破第四面墙、天气/币价/百科工具生态、幽灵模式、摸摸头互动、猫娘模式、暗黑模式、真实数值注入、主动唤醒……打开设置面板，惊喜（吓）不断。

---

## 🚀 本地运行指南

1. **下载代码**：`git clone` 本仓库，或点 Code → Download ZIP 解压。
2. **双击 `index.html`** —— `file://` 直接打开即可，**无需服务器、无需构建**。
3. **自备大模型 API**：点右下角 ⚙️ 设置，填写 OpenAI 兼容的 `chat/completions` 端点 + Key + 模型。
   - 模型名包含 `deepseek` → 进入 **大肥鱼** 模式；否则为 **Verity** 模式。
4. （可选）想体验**离线跑酷视频**：自行把 `run.mp4` 放到 `assets/audio/run.mp4`（仓库为轻量已排除，不影响对话与日常玩法）。
5. 想要语音 / 工具（Function Calling），在设置里分别勾选即可。

> ⚠️ **游玩警告**：请调至适中音量。本作含**突然惊吓（Jump Scare）**与**打破第四面墙**内容，心脏不适者建议关闭语音。首次使用摄像头 / 定位 / 通知会弹浏览器授权，拒绝后相关工具会优雅报错。

---

## 📁 项目结构

```
index.html          # 全部逻辑（单文件，无构建步骤，约 470KB）
README.md
LICENSE             # MIT（非商业 · 须署名）
ASSETS.txt          # 素材清单
assets/
  img/              # 图片：表情、大肥鱼、背景、突脸等（已统一小写文件名）
  audio/            # 轻量音频（BGM / 开场 / 语音）
extras/             # 废案与测试脚本（已被 .gitignore 排除，不参与运行）
```

- 换图：直接进 `assets/img/` 覆盖同名文件，刷新即生效。
- 在线部署与本地打开是**同一个 `index.html`**：部署到 `http(s)` 域名时会自动跳过 204MB 跑酷视频并关闭误封反作弊；本地 `file://` 则保留完整体验。

---

## 📜 致敬与版权

| 角色 | 署名 |
|---|---|
| 🥚 **原作者** | 盒合褐 Hehehe |
| 🔧 **二创** | 罚双本双 |
| 🌟 **三创 / 网页重构 / 双人格开发者** | 唐666114514 |
| 🤖 **协作工具** | WorkBuddy & DeepSeek |

本项目为爱好者**三创魔改**，仅供学习与娱乐。

---

## 📄 许可证

见 [LICENSE](LICENSE)：基于 **MIT** 协议，**允许自由修改与再分发，必须保留原作者署名。**

> 🤝 **商用约定**：MIT 协议本身允许商业使用；但本项目是爱好者三创魔改，请尊重原作者——**若要商用，请先取得原作者（盒合褐Hehehe / 罚双本双 / 唐666114514）授权。**

> “官方只是提供了一个 API，而真正的世界是 Mod 作者建的。”
> —— 玩得开心，记得调小音量。🎧
