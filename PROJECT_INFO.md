# 项目信息 (Project Information)

## 项目概述

**Index-System** 是一个从 [Xwdjjy.github.io](https://github.com/Xwdjjy/Xwdjjy.github.io) 项目中分离出来的独立的索引管理系统。

## 历史背景

- **原始位置**：Xwdjjy.github.io 项目的 `src/` 目录
- **分离时间**：2026年2月
- **分离原因**：
  - 索引系统逻辑完整、功能独立
  - 支持在多个项目中使用
  - 便于单独维护和版本管理
  - 提供更灵活的集成方式
  - 上面都是瞎扯，其实就是发现做都做了，不如分离出来
## 项目结构

```
Index-System/
├── index.html                 # 主索引页面
├── index.json                 # 条目数据文件（核心数据库）
├── QUICK_REFERENCE.md         # 快速参考指南
├── INTEGRATION.md             # 集成指南（新）
├── package.json               # 项目配置（新）
├── PROJECT_INFO.md            # 项目信息（本文件）
├── LICENSE                    # Apache 2.0 许可证
├── README.md                  # 项目主文档
├── js/
│   └── index-manager.js       # 核心脚本（动态加载和管理）
├── projects/
│   └── gender-prediction/
│       └── index.html         # 示例项目页面
└── docs/                      # 完整文档
    ├── START_HERE.md          # 入门指南
    ├── INDEX_GUIDE.md         # 详细使用指南
    ├── WORKFLOW_DIAGRAM.md    # 工作流程和架构
    ├── IMPLEMENTATION_SUMMARY.md  # 实现细节
    └── COMPLETION_CHECKLIST.md    # 完成清单
```

## 技术栈

- **前端**：HTML5, CSS3, Vanilla JavaScript
- **数据**：JSON
- **部署**：Static Site（可托管在 GitHub Pages、Vercel 等）
- **兼容性**：所有现代浏览器

## 许可证

本项目采用 **Apache License 2.0** 许可证，保持与原项目一致。

详见 [LICENSE](./LICENSE) 文件。

## 与原项目的关系

### Xwdjjy.github.io 项目
- 包含个人介绍网页
- Index-System 是其重要的功能模块

### Index-System 项目（本项目）
- 独立的索引管理系统
- 已在 Xwdjjy.github.io 中使用
- 也可以在其他项目中独立使用
- 可以通过子模块方式保持同步更新

## 使用场景

✅ **个人网站** - 管理文章、项目、文档索引  
✅ **文章系统** - 文章目录和分类管理  
✅ **项目集合** - 多个项目的统一展示  
✅ **知识库** - 文档和资源索引  
✅ **作品集** - 展示设计、开发作品  
✅ **资源管理** - 组织和共享各类资源  

## 开发指南

### 添加内容

1. 编辑 `index.json`
2. 在 `items` 数组中添加新条目
3. 刷新浏览器查看效果

### 提交更改

```bash
git add index.json
git commit -m "feat: 添加新条目"
git push origin main
```

### 提交功能请求
说明你想要的新功能和使用场景

## 相关链接

- **GitHub 仓库**：[Xwdjjy/Index-System](https://github.com/Xwdjjy/Index-System)
- **原始项目**：[Xwdjjy/Xwdjjy.github.io](https://github.com/Xwdjjy/Xwdjjy.github.io)
- **在线演示**：https://Xwdjjy.github.io/src/index.html（使用原项目的版本）

## 常见问题

**Q: 可以用于商业项目吗？**  
A: 可以，遵守 Apache 2.0 许可证即可

**Q: 如何定制样式？**  
A: 修改或新增 CSS，在 index.html 中引入自定义样式

**Q: 支持数据库连接吗？**  
A: 目前使用静态 JSON，但可以修改脚本连接到 API 端点

## 版本信息

| 版本  | 日期       | 说明                              |
|-------|------------|-----------------------------------|
| 1.0.0 | 2026-02-08 | 从 Xwdjjy.github.io 分离的独立版本 |

## 联系方式

- GitHub: [@Xwdjjy](https://github.com/Xwdjjy)
- 项目 Issues: [Index-System Issues](https://github.com/Xwdjjy/Index-System/issues)

---

感谢使用 Index-System！如有任何问题或建议，欢迎提交 Issue 或 Pull Request。
