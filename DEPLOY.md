# 部署指南

## GitHub Pages 部署步骤

### 1. 准备仓库
```bash
# 初始化Git仓库（如果还没有）
git init

# 添加所有文件
git add .

# 提交更改
git commit -m "Initial commit: 谷语日签静态网页版"

# 添加远程仓库
git remote add origin https://github.com/你的用户名/cp-omikuji.git

# 推送到GitHub
git push -u origin main
```

### 2. 启用GitHub Pages

1. 进入GitHub仓库页面
2. 点击 "Settings" 标签
3. 在左侧菜单中找到 "Pages"
4. 在 "Source" 部分选择 "GitHub Actions"
5. 保存设置

### 3. 自动部署

推送代码到main分支后，GitHub Actions会自动：
- 检出代码
- 配置Pages
- 上传静态文件
- 部署到GitHub Pages

### 4. 访问网站

部署完成后，你的网站将在以下地址可用：
```
https://你的用户名.github.io/cp-omikuji
```

## 本地测试

```bash
# 启动本地服务器
python3 -m http.server 8000

# 在浏览器中访问
open http://localhost:8000
```

## 故障排除

### 如果GitHub Pages没有自动部署：
1. 检查 `.github/workflows/deploy.yml` 文件是否存在
2. 确保仓库有正确的权限设置
3. 查看Actions标签页中的错误信息

### 如果网站无法访问：
1. 检查仓库设置中的Pages配置
2. 确保选择了正确的分支和文件夹
3. 等待几分钟让DNS传播

## 自定义域名（可选）

如果你想使用自定义域名：
1. 在仓库根目录创建 `CNAME` 文件
2. 在文件中写入你的域名（如：`example.com`）
3. 在你的域名DNS设置中添加CNAME记录指向 `你的用户名.github.io`
