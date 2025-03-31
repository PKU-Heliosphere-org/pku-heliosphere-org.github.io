# PKU-Heliosphere-org 项目展示页面

这是PKU-Heliosphere-org组织的GitHub Pages站点，用于展示组织内各个日球层和空间物理学相关项目。

## 部署说明

1. 在PKU-Heliosphere-org组织中创建名为`PKU-Heliosphere-org.github.io`的仓库：
   - 这个特殊名称的仓库会自动成为组织的GitHub Pages站点
   - 将本项目文件推送到该仓库的main分支
   - GitHub会自动将其部署为组织页面

2. 在组织设置中确认GitHub Pages已启用：
   - 进入组织设置页面
   - 找到Pages设置选项
   - 确认main分支被选为源分支
   - 确认根目录(/)被选为发布源

2. 自定义域名（可选）：
   - 在Pages设置中添加自定义域名
   - 配置DNS记录
   - 等待DNS生效

## 维护说明

### 添加新项目

要添加新的项目展示，请在`index.html`文件中的`projects`区域添加新的项目卡片：

```html
<div class="project-card">
    <h3>项目名称</h3>
    <p>项目描述</p>
    <div class="tags">
        <span class="tag">标签1</span>
        <span class="tag">标签2</span>
    </div>
</div>
```

### 更新样式

所有样式都在`styles.css`文件中定义。要修改页面外观，编辑相应的CSS类即可。

### 添加新功能

1. 项目预览：可以添加项目截图和演示
2. 详细文档：可以为每个项目创建单独的详情页
3. 互动演示：可以添加在线演示功能

## 文件结构

```
.
├── index.html      # 主页面
├── styles.css      # 样式文件
└── README.md       # 说明文档
```

## 本地测试

可以使用以下命令在本地预览页面：

```bash
# 使用Python启动一个简单的HTTP服务器
python -m http.server 8000

# 或使用Node.js的http-server
npx http-server
```

然后在浏览器中访问 `http://localhost:8000` 即可预览。

## 贡献指南

1. Fork 本仓库
2. 创建新的分支
3. 提交更改
4. 发起Pull Request

## 联系方式

如有问题或建议，请通过[Issues页面](https://github.com/PKU-Heliosphere-org/PKU-Heliosphere-org.github.io/issues)反馈，或联系组织管理员。