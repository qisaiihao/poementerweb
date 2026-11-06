# Poementer 官网

这是一个简洁的Poementer应用介绍网站，包含APP下载和网页版体验入口。

## 文件结构

```
├── index.html          # 主页面
├── style.css           # 样式文件
├── app-release.apk     # APK文件（请替换为实际文件）
├── web/                # 网页版应用
│   ├── index.html
│   └── static/
├── nginx.conf          # Nginx配置文件
└── README.md           # 说明文件
```

## 部署到宝塔面板

### 1. 上传文件
将所有文件上传到宝塔面板的网站根目录（通常为 `/www/wwwroot/your-domain.com/`）

### 2. 配置域名
- 在宝塔面板中添加站点
- 将域名指向您的服务器IP
- 上传文件到对应的网站目录

### 3. 配置Nginx
- 将 `nginx.conf` 中的配置添加到宝塔面板的Nginx配置中
- 修改域名和路径为您的实际配置
- 重启Nginx服务

### 4. 替换APK文件
将 `app-release.apk` 替换为您实际的APK文件

### 5. 测试访问
- 访问您的域名查看主页面
- 测试"下载APP"按钮是否正常下载
- 测试"网页体验"按钮是否正常跳转到web目录

## 功能说明

- **主页面**: 黑色背景，白色文字，居中显示"poementer"标题
- **下载入口**: 点击可下载APK文件
- **体验入口**: 点击可进入网页版应用体验
- **响应式设计**: 支持手机和桌面端访问

## 自定义修改

### 修改标题
编辑 `index.html` 中的 `<h1 class="title">poementer</h1>`

### 修改样式
编辑 `style.css` 文件，可以调整：
- 背景颜色
- 文字颜色
- 按钮样式
- 动画效果

### 修改下载链接
编辑 `index.html` 中的 `href="app-release.apk"` 为您的APK文件名

