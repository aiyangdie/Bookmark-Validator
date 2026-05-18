# 🔖 Bookmark-Validator

**一键检测浏览器书签存活状态，快速清理失效链接。**

[![在线试用](https://img.shields.io/badge/在线试用-点击体验-blue)](https://aiyangtongxue.github.io/Bookmark-Validator)

![界面截图](第一个版本图片.png)
![界面截图](第二个版本图片.png)

---

## 📌 项目简介

Bookmark-Validator 是一款纯前端书签可用性检测工具，支持 Chrome / Firefox / Edge 等主流浏览器导出的书签文件（`.html`）。所有操作在浏览器本地完成，无需服务器，隐私安全有保障。

项目包含两个版本：
- **基础版**（`index.html`）：上传书签 → 检测 → 查看结果
- **增强版**（`index (2).html`）：在基础版之上，支持一键删除不可用书签、导出清理后的书签文件

---

## ✨ 核心特性

- 🔍 **智能解析** — 自动识别浏览器导出的 Netscape Bookmark 格式
- ⚡ **批量检测** — 逐条检测书签链接的可用性，支持数百个书签
- 📊 **实时进度** — 检测进度百分比 + 进度条实时反馈
- ✅❌ **状态可视化** — 绿色标识可用链接，红色标识失效链接
- 🗑️ **一键清理** — 增强版支持删除所有不可用书签
- 💾 **书签导出** — 增强版支持导出清理后的书签为标准 HTML 格式，可直接导入浏览器
- 🔒 **隐私优先** — 所有操作在浏览器本地完成，不上传任何数据

---

## 🛠️ 技术栈

| 技术 | 用途 |
|------|------|
| HTML5 | 页面结构 |
| CSS3 | 响应式布局、CSS Variables、过渡动画 |
| JavaScript (ES6+) | Fetch API、DOMParser、AbortController、FileReader |
| DOMParser | 解析浏览器书签 HTML 文件 |
| Fetch API (HEAD) | 轻量级链接可用性检测 |
| AbortController | 5 秒超时自动终止请求 |

---

## 🚀 快速开始

### 前置条件

- 现代浏览器（Chrome / Firefox / Edge / Safari）

### 安装步骤

```bash
git clone https://github.com/aiyangtongxue/Bookmark-Validator.git
cd Bookmark-Validator
```

### 运行

直接在浏览器中打开 `index.html` 即可使用，无需任何构建工具或服务器。

### 使用流程

1. 从浏览器导出书签文件（`书签管理器 → 导出书签`）
2. 打开工具页面，上传导出的 `.html` 文件
3. 点击「开始检测」，等待检测完成
4. 根据检测结果清理失效书签（增强版支持一键删除和导出）

---

## 📂 项目结构

```
Bookmark-Validator/
├── index.html              # 基础版 — 书签检测工具
├── index (1).html          # 基础版副本
├── index (2).html          # 增强版 — 支持删除和导出
├── test.txt                # 测试文件
├── 第一个版本图片.png       # 基础版截图
├── 第二个版本图片.png       # 增强版截图
├── CNAME                   # GitHub Pages 自定义域名
└── README.md               # 项目说明
```

---

## 🤝 贡献与许可证

欢迎提交 PR 或 [报告问题](https://github.com/aiyangtongxue/Bookmark-Validator/issues)！

本项目采用 MIT 开源协议，您可以自由使用、修改和分发。

---

*💡 提示：建议定期检测书签，保持收藏夹整洁高效！*
