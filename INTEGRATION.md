# 集成指南 (Integration Guide)

本文档说明如何将 Index-System 集成到其他项目中。

## 📦 安装方式

### 方式 1: 仅复制核心文件（其实只有这一个方法）

可以复制以下关键文件：

```
Index-System/
├── index.html        (从本项目复制)
├── index.json        (从本项目复制，修改URL)
└── js/
    └── index-manager.js  (从本项目复制)
```

## 🔧 配置

### 修改数据源 URL

如果数据存储在其他位置，编辑 `index-manager.js`：

```javascript
// 原始
const jsonUrl = './index.json';

// 修改为你的 URL
const jsonUrl = '/api/index-data.json';
```

### 自定义样式

在 `index.html` 中添加你的 CSS：

```html
<link rel="stylesheet" href="/your-styles.css">
```

### 环境变量

如果需要不同环境的配置，可以在加载脚本前设置：

```html
<script>
  window.INDEX_CONFIG = {
    apiUrl: 'https://api.example.com',
    enableSearch: true,
    theme: 'dark'
  };
</script>
<script src="js/index-manager.js"></script>
```

## 📋 检查清单

- [ ] 复制或链接必要的文件
- [ ] 确认 `index.json` 路径正确
- [ ] 检查相对路径是否正确
- [ ] 在浏览器中测试功能
- [ ] 验证搜索功能正常
- [ ] 测试响应式设计

## 🐛 常见问题

**Q: 加载不出条目？**  
A: 检查 `index.json` 的 URL 是否正确，查看浏览器控制台错误信息

**Q: 样式不正确？**  
A: 确认相对路径正确，检查 CSS 文件加载情况

**Q: 搜索功能不工作？**  
A: 确认 JavaScript 文件已正确加载，检查浏览器控制台