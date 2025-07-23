# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 项目概述

这是一个静态网站项目，托管在 GitHub Pages 上，包含以下页面：

- **index.html** - 主导航页面，提供项目导航功能
- **snake-game.html** - 使用 Three.js 构建的 2.5D 贪吃蛇游戏
- **npm-tutorial.html** - NPM 教程页面
- **opencode-system-architecture.html** - OpenCode 系统架构文档
- **opencode-tools-manual.html** - OpenCode 工具手册

## 技术栈

- 纯 HTML/CSS/JavaScript
- Three.js (用于 3D 贪吃蛇游戏)
- 响应式设计
- GitHub Pages 静态托管

## 开发命令

由于这是一个纯静态网站项目，没有构建过程或包管理器依赖：

- **本地开发**: 直接在浏览器中打开 HTML 文件
- **部署**: 通过 Git 推送到 main 分支自动部署到 GitHub Pages

## 项目架构

### 文件结构
```
/
├── index.html                           # 主导航页面
├── snake-game.html                      # 贪吃蛇游戏
├── npm-tutorial.html                    # NPM教程
├── opencode-system-architecture.html    # 系统架构文档
└── opencode-tools-manual.html          # 工具手册
```

### 贪吃蛇游戏架构 (snake-game.html)
- 使用 Three.js 渲染 2.5D 场景
- 游戏状态管理：难度选择、游戏进行、暂停、游戏结束
- 支持键盘控制：方向键移动，空格键暂停/重新开始
- 难度系统：Easy(7), Medium(15), Hard(20)
- 3D 渲染：立方体网格表示蛇身和食物

### 样式设计模式
- 渐变背景设计
- 卡片式布局
- 悬停动画效果
- 响应式设计支持移动端

## 编码规范

- 使用中文注释和界面文本
- HTML 文档使用 `lang="zh-CN"` 或 `lang="en"`
- CSS 使用现代 Flexbox 布局
- JavaScript 使用 ES6+ 语法
- 保持代码格式整洁，适当缩进

## 常见任务

- **添加新页面**: 创建新的 HTML 文件，并在 index.html 中添加导航链接
- **修改游戏逻辑**: 编辑 snake-game.html 中的 JavaScript 代码
- **样式调整**: 直接修改各文件中的 `<style>` 标签内容
- **部署更新**: 提交更改到 main 分支

## 注意事项

- 所有外部依赖通过 CDN 引入（如 Three.js）
- 游戏使用 Three.js r128 版本
- 确保所有页面在移动设备上正常显示
- 保持导航页面的链接与实际文件名一致