# 谷语日签 - 娃包轻陪伴OC

一个完全静态的H5日签生成器，专为CP漫展设计。

## ✨ 特性

- 🎨 **完全静态** - 单HTML文件，无外部依赖
- 📱 **响应式设计** - 完美适配手机和桌面
- 🖼️ **随机模板** - 支持两个精美SVG模板随机选择
- 🎲 **智能占卜** - 基于图片颜色生成个性化日签
- 💾 **一键保存** - 生成的日签可直接下载
- 🚀 **GitHub Pages** - 可直接部署到GitHub Pages
- 🔤 **方正字体** - 使用方正标雅宋繁体字体

## 🎯 功能说明

1. **随机模板** - 每次生成随机选择两个SVG模板中的一个
2. **精确定位** - 根据SVG模板精确定位文字内容
3. **占卜生成** - 生成宜忌、幸运色、幸运物、幸运地、温馨提醒、签文
4. **结果展示** - 美观的日签展示和保存功能

## 🌐 在线访问

**项目地址**: https://herlsHu.github.io/omikuji/

## 🚀 部署到GitHub Pages

### 方法一：使用GitHub Actions（推荐）

1. 将代码推送到GitHub仓库
2. 进入仓库设置 (Settings) → Pages
3. 选择 Source 为 "GitHub Actions"
4. 推送代码后，GitHub Actions会自动部署
5. 等待部署完成，访问 `https://你的用户名.github.io/omikuji`

### 方法二：手动部署

1. Fork 这个仓库
2. 进入仓库设置 (Settings) → Pages
3. 选择 Source 为 "Deploy from a branch"
4. 选择 Branch 为 "master"
5. 选择 Folder 为 "/ (root)"
6. 点击 Save
7. 等待几分钟，访问 `https://你的用户名.github.io/omikuji`

### 本地测试

```bash
# 使用Python
python -m http.server 8000

# 或使用Node.js
npx serve .

# 然后访问 http://localhost:8000
```

## 📁 文件结构

```
omikuji/
├── index.html                    # 主页面（包含所有CSS和JS）
├── index-backup.html             # 备份文件
├── public/                       # 静态资源文件夹
│   ├── 定稿1（for 前端）.svg     # 模板1
│   └── 定稿2（for 前端）.svg     # 模板2
├── .github/
│   └── workflows/
│       └── deploy.yml            # GitHub Actions部署配置
├── package.json                  # 项目配置
├── vercel.json                   # Vercel部署配置（可选）
└── README.md                     # 说明文档
```

## 🎨 技术特点

- **完全独立** - 不依赖任何外部CSS/JS文件
- **内联样式** - 所有样式都在HTML内部
- **响应式设计** - 支持手机和桌面
- **现代CSS** - 使用Flexbox和Grid布局
- **原生JavaScript** - 无框架依赖，纯原生JS
- **Canvas绘图** - 使用HTML5 Canvas API生成图片
- **SVG集成** - 支持SVG模板作为背景

## 🔧 自定义

### 修改词库
在 `index.html` 中找到 `wordBank` 对象，可以修改：
- `yi` - 宜的内容
- `ji` - 忌的内容  
- `lucky_items` - 幸运物
- `lucky_places` - 幸运地
- `omikuji` - 签文
- `warm_tips` - 温馨提醒

### 添加新模板
1. 将新的SVG文件放入 `public/` 文件夹
2. 在 `templates` 数组中添加新模板路径
3. 确保新模板的文字位置与现有模板一致

### 修改样式
所有CSS都在 `<style>` 标签内，可以直接修改。

## 📱 浏览器支持

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

## 📄 许可证

MIT License

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

---

**谷语日签** - 让每一次占卜都充满惊喜 ✨