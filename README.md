# GlitchRoot

✨ 一个具有 Cyber / Sci-Fi 风格的静态根域名展示页，可作为 **404 页面**、**Error Fallback**、**维护页** 或 **网站入口占位页** 使用。

这个项目包含一个高质量的静态 `index.html`，拥有：

- 霓虹渐变背景 + 网格 + 扫描线效果  
- 3D 卡片跟随鼠标倾斜  
- 故障风格标题（Glitch Effect）  
- 访客 IP 自动检测  
- 随机“宇宙文案”  
- 完全自包含（0 依赖）  
- 支持作为根域名部署、GitHub Pages、Netlify、Vercel、Nginx、Apache 等静态站点

---

## 🌌 预览 Preview

> 你可以在浏览器中直接打开 `index.html` 查看效果。

https://g-huohuo.github.io/GlitchRoot/
<img width="2560" height="1196" alt="image" src="https://github.com/user-attachments/assets/7897a5ff-9ac2-4564-94d0-d307abb713bd" />

---

## 📦 部署方式

### **方式一：直接放到根域名**
将 `index.html` 上传到你的服务器根目录：/var/www/html/index.html

### **方式二：GitHub Pages**
1. Push 到仓库
2. 打开 Settings → Pages
3. Source 选 `main` 分支
4. 保存后即可访问 `https://你的用户名.github.io/GlitchRoot/`

### **方式三：Nginx 作为兜底页**
```nginx
error_page 404 /index.html;
location = /index.html {
    root /path/to/GlitchRoot;
}
