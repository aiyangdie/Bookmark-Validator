<p align="center"><img src="assets/covers/33-Bookmark-Validator.jpg" alt="书签检测 项目封面" width="100%"></p>

<h1 align="center">Bookmark Validator · 书签体检</h1>

<p align="center">导入浏览器书签，批量扫出打不开的链接，一次性清理</p>

<p align="center">
  <a href="http://bookmark.aikex.ink/">在线使用</a>
</p>

## 简介

收藏夹用久了必然堆着一批已经打不开的地址。这个工具直接读取浏览器导出的书签 HTML，逐个探测可用性，把失效链接单独列出来，再导出干净的书签文件。

## 功能

- **拖拽导入**：支持浏览器导出的书签 HTML 文件
- **批量探测**：并发检查每个链接的响应状态
- **死链清单**：把超时、404、重定向异常的条目单独列出
- **导出结果**：保留可用条目，重新生成可导入的书签文件
- **纯前端**：书签文件不上传，本地解析

## 技术栈

HTML5 · JavaScript（DOMParser 解析书签、fetch 探测）· 纯静态部署

## 使用

1. 在浏览器导出书签为 HTML
2. 打开工具，把文件拖入
3. 等待扫描完成，查看失效清单
4. 导出清理后的书签文件，重新导入浏览器

## 项目结构

```
index.html      页面与交互
js/             解析、探测与导出逻辑
css/            样式
```

## 许可证

仓库未附 LICENSE 文件，使用与分发请先联系作者确认。
