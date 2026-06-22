<p align="center"><a href="https://www.autoa2a.org"><img src="https://agent.oagi.com.cn/uploads/202606/29ea3ed5413830b3.png" alt="AutoA2A" height="110"></a></p>

# WebGL 3D 在线编辑器

> 本项目由 [www.autoa2a.org](https://www.autoa2a.org) 「AI 研究院」**多个 AI 协作自动生成**（共 8 个页面）。在线访问： https://AutoA2A.github.io/autoatoa-webgl-3d-editor/

# WebGL 3D 在线编辑器  

## 网站简介  
本项目是一个基于 WebGL 的 **3D 在线编辑器**，支持模型导入、实时渲染、材质编辑、光照调节等完整工作流。用户只需打开浏览器，即可在页面内完成从建模到预览的全部操作，无需安装任何插件或客户端。  

## 页面与功能  
| 页面 | 主要功能 | 说明 |
|------|----------|------|
| **index.html** | 入口页面 | 介绍产品、快速开始、跳转至编辑器 |
| **editor.html** | 3D 场景编辑 | 视图交互、模型导入、变换、层级管理 |
| **material.html** | 材质编辑 | PBR 参数、纹理贴图、实时预览 |
| **lighting.html** | 光照设置 | 环境光、点光源、聚光灯、阴影开关 |
| **animation.html** | 动画控制 | 关键帧编辑、时间轴播放、导出 |
| **export.html** | 导出/分享 | 支持 glTF、OBJ、JSON，生成短链 |
| **settings.html** | 全局设置 | 渲染分辨率、性能模式、主题切换 |
| **about.html** | 项目介绍 | 开源协议、贡献者、版本日志 |

每个页面均采用 **模块化** 结构，统一的 UI 框架保证交互一致性；核心渲染逻辑封装在 `engine/` 目录的 `WebGLRenderer` 类中，支持自动适配不同显卡特性。

## 多 AI 协作与验收  
本项目由 **四位 AI**（代码生成、UI 设计、文档撰写、测试）协同完成，采用以下工作流：  

1. **需求拆解**：Prompt‑Engineer 将功能拆分为 8 个子任务。  
2. **代码生成**：Code‑AI 按子任务输出 ES6 + Three.js 实现，并提交 Pull Request。  
3. **UI 设计**：Design‑AI 负责页面布局、配色、交互动画，生成对应的 CSS/HTML。  
4. **文档撰写**：Doc‑AI 基于代码注释自动生成 README 与 API 文档。  
5. **自动化测试**：Test‑AI 编写 Jest + Playwright 脚本，对每个页面进行单元、集成与视觉回归测试。  
6. **验收**：Human‑Reviewer 对 AI 产出进行功能、可用性、性能三维度审查，全部通过后合并至 `main`。  

整个过程在 GitHub Actions 中全链路运行，确保每次提交都经过严格校验。

## GitHub Pages 部署与访问 (入口 `index.html`)  
仓库根目录已配置 **GitHub Pages**，部署分支为 `gh-pages`。  
- **部署步骤**：  
  1. `git push origin main` → GitHub Actions 自动构建并将 `dist/` 内容同步至 `gh-pages`。  
  2. 页面资源采用相对路径，支持 **HTTPS** 与 **缓存优化**（Service Worker）。  
- **访问入口**：  
  ```
  https://<用户名>.github.io/<仓库名>/index.html
  ```  
打开上述链接即可进入编辑器首页，点击 “开始编辑” 进入 `editor.html` 开始 3D 创作。  

---  
祝您玩得开心，期待社区贡献更多插件与模型！

---

## 关于 AutoA2A

✅️AutoA2A是智能体互连 Agent to Agent平台，实现智能体间的无缝发现、协商、协作与数据安全交换，让您的智能体从信息孤岛走向高效协同，重塑数字化生产力。赋能多智能体生态发展自动化与AI协作,开启AI即服务新时代。

官网： [www.autoa2a.org](https://www.autoa2a.org)

Copyright © 2025 - 2026 AutoA2A. All Rights Reserved. A2A版权所有
