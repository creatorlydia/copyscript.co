# 🌟 导航站 - CopyScript

一个现代化的网站导航平台，提供精选的优质网站和工具。

## ✨ 特性

- 🎨 现代化设计，响应式布局
- 🔍 实时搜索功能
- 📱 移动端友好
- 🔗 安全的链接跳转
- 🚀 轻量级，无外部依赖
- 🛡️ 错误处理和安全防护

## 🚀 快速开始

1. 直接在浏览器中打开 `index.html` 文件
2. 或者使用本地服务器：
   ```bash
   # 使用Python启动简单服务器
   python -m http.server 8000
   
   # 或使用Node.js的serve工具
   npx serve .
   ```

## 🔧 功能说明

### 已解决的问题

1. **链接跳转问题** - 使用安全的 `window.open()` 方法，确保链接能够正常打开
2. **分析工具错误** - 将 Google Analytics 和 Microsoft Clarity 的代码注释掉，避免配置错误
3. **JSON解析错误** - 添加错误处理，阻止浏览器扩展引起的错误

### 主要功能

- **分类浏览**: 网站按功能分类组织
- **搜索过滤**: 支持按标题和描述搜索
- **安全跳转**: 所有外部链接在新标签页安全打开
- **响应式设计**: 自适应桌面和移动设备

## 📝 自定义配置

### 添加新网站

在 `index.html` 的 JavaScript 部分找到 `websites` 对象，按以下格式添加：

```javascript
'分类名称': [
    {
        title: '网站名称',
        url: 'https://example.com',
        desc: '网站描述',
        icon: '🎯'  // emoji图标
    }
]
```

### 启用分析工具

如果需要添加网站统计，请：

1. **Google Analytics**: 
   - 获取你的跟踪ID
   - 将 `YOUR_GA_TRACKING_ID` 替换为实际ID
   - 取消相关代码的注释

2. **Microsoft Clarity**:
   - 获取你的项目ID  
   - 将 `YOUR_CLARITY_PROJECT_ID` 替换为实际ID
   - 取消相关代码的注释

## 🔒 安全特性

- URL验证：只允许 http/https 协议
- 新窗口打开：使用 `noopener,noreferrer` 属性
- 错误处理：捕获和处理各种可能的错误
- XSS防护：安全的DOM操作

## 🎨 样式定制

CSS样式都内嵌在HTML文件中，你可以轻松修改：
- 颜色主题
- 字体样式
- 布局间距
- 动画效果

## 📱 浏览器支持

- Chrome (推荐)
- Firefox
- Safari
- Edge
- 移动端浏览器

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

## 📄 许可证

MIT License

---

💡 如果遇到任何问题，请检查浏览器控制台是否有错误信息。 