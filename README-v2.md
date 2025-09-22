# 谷语日签 v2 - 娃包轻陪伴OC

一个全新的四宫格交互式日签生成器，专为CP漫展设计。

## ✨ 新版本特性

- 🎯 **四宫格布局** - 清晰的交互流程，从触发到结果
- 🎨 **渐进式引导** - 逐步引导用户完成操作
- 📱 **响应式设计** - 完美适配手机和桌面
- 🎲 **智能占卜** - 基于图片颜色生成个性化日签
- 🎁 **无料领取** - 集成无料领取信息展示
- 💾 **一键保存** - 生成的日签可直接下载

## 🎯 交互流程

### 1. 交互触发环节（左上角）
- 图片上传界面
- 支持点击选择和拖拽上传
- 预览上传的图片
- "开始抽取日签"按钮

### 2. 交互引导环节（右上角）
- **放置娃包**：引导用户将娃包放在指定位置
- **站立位置**：引导用户站在指定位置
- 两个引导内容依次出现，增强仪式感

### 3. 引导等待环节（左下角）
- 旋转加载动画
- "正在分析你的今日运势……"提示
- 营造神秘感和期待感

### 4. 结果获取环节（右下角）
- 生成的日签图片展示
- 无料领取信息说明
- 保存和重新抽取按钮

## 🌐 在线访问

**项目地址**: https://herlsHu.github.io/cpomikuji/

## 🚀 部署到GitHub Pages

### 方法一：使用GitHub Actions（推荐）

1. 将代码推送到GitHub仓库
2. 进入仓库设置 (Settings) → Pages
3. 选择 Source 为 "GitHub Actions"
4. 推送代码后，GitHub Actions会自动部署
5. 等待部署完成，访问 `https://你的用户名.github.io/cpomikuji`

### 方法二：手动部署

1. Fork 这个仓库
2. 进入仓库设置 (Settings) → Pages
3. 选择 Source 为 "Deploy from a branch"
4. 选择 Branch 为 "main" 或 "master"
5. 选择 Folder 为 "/ (root)"
6. 点击 Save
7. 等待几分钟，访问 `https://你的用户名.github.io/cpomikuji`

## 📁 文件结构

```
cpomikuji/
├── index-v2.html              # v2版本主页面
├── index.html                 # v1版本主页面
├── public/                    # 静态资源文件夹
│   ├── 定稿1（for 前端）.svg  # 模板1
│   └── 定稿2（for 前端）.svg  # 模板2
├── fonts/                     # 字体文件
│   ├── 方正标雅宋繁体.TTF
│   └── 方正标雅宋简体.TTF
├── .github/
│   └── workflows/
│       └── deploy.yml         # GitHub Actions部署配置
├── package.json               # 项目配置
├── vercel.json                # Vercel部署配置（可选）
├── README-v2.md               # v2版本说明文档
└── README.md                  # v1版本说明文档
```

## 🎨 技术特点

- **四宫格布局** - 使用CSS Grid实现响应式四宫格
- **渐进式动画** - 引导内容依次出现，增强用户体验
- **完全独立** - 不依赖任何外部CSS/JS文件
- **内联样式** - 所有样式都在HTML内部
- **现代CSS** - 使用Flexbox和Grid布局
- **原生JavaScript** - 无框架依赖，纯原生JS
- **Canvas绘图** - 使用HTML5 Canvas API生成图片
- **SVG集成** - 支持SVG模板作为背景

## 🔧 自定义

### 修改引导内容
在 `index-v2.html` 中找到引导环节的HTML，可以修改：
- 娃包放置的引导文字
- 站立位置的引导文字
- 图标和样式

### 修改无料领取信息
在 `index-v2.html` 中找到 `.gift-info` 部分，可以修改：
- 无料领取的说明文字
- 样式和颜色

### 修改词库
在 `index-v2.html` 中找到 `wordBank` 对象，可以修改：
- `yi` - 宜的内容
- `ji` - 忌的内容  
- `lucky_items` - 幸运物
- `lucky_places` - 幸运地
- `omikuji` - 签文
- `warm_tips` - 温馨提醒

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

**谷语日签 v2** - 让每一次占卜都充满仪式感 ✨
