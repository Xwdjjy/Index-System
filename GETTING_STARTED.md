# 🚀 开始使用 Index-System

## 第一步：克隆或下载项目

```bash
git clone https://github.com/Xwdjjy/Index-System.git
cd Index-System
```

## 第二步：编辑内容

1. 打开 `index.json` 文件
2. 在 `items` 数组中添加或修改条目
3. 保存文件
4. 刷新浏览器 (Ctrl+F5 或 Cmd+Shift+R)

## 示例条目格式

### 编辑 `items` 数组：

```json
{
  "id": 1,
  "title": "我的第一篇文章",
  "description": "这是一篇关于...的文章",
  "type": "posts",
  "url": "/posts/my-first-post",
  "date": "2026-02-08",
  "tags": ["新手", "指南"]
}
```

### 编辑 `recent` 数组：

```json
"recent": [
  {
    "title": "发布新文章：你的标题",
    "icon": "A",           // 单个字符
    "time": "刚刚",       // 时间描述
    "url": "/blog/post-1"
  }
]
```

## 常见问题

**Q: 修改 JSON 后没有更新？**  
A: 按 Ctrl+F5 (Windows) 或 Cmd+Shift+R (Mac) 硬刷新浏览器

**Q: 搜索功能怎么用？**  
A: 按 Ctrl+K 打开搜索框，输入关键词即可

## 更多帮助

- 📖 详细文档：查看 `README.md`
- ⚡ 快速参考：查看 `QUICK_REFERENCE.md`
- 🔗 集成指南：查看 `INTEGRATION.md`
- 💡 项目信息：查看 `PROJECT_INFO.md`

## 下一步

1. 了解项目结构（查看 README.md）
2. 添加你的第一个条目（编辑 index.json）
3. 探索高级功能（查看 docs/ 目录中的文档）
4. 自定义外观（添加 CSS）

---

**有问题？**点击 [GitHub Issues](https://github.com/Xwdjjy/Index-System/issues) 提交反馈！
