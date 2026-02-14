# 🎀 OHKU 可爱小怪物画廊

> 专为 Mac Retina 屏幕优化的高清图片展示网站

![OHKU](https://img.shields.io/badge/OHKU-可爱小怪物-ff69b4?style=for-the-badge)
![Retina Optimized](https://img.shields.io/badge/Retina-Optimized-success?style=for-the-badge)

## ✨ 特性

- 🖥️ **Retina 屏幕完美优化** - 在 Mac 高分辨率显示器上清晰无比
- 📱 **完全响应式** - 适配手机、平板、电脑
- 🎨 **粉色可爱风格** - 符合 OHKU 品牌形象
- ⚡ **快速加载** - 图片懒加载技术
- 💖 **流畅动画** - 丝滑的交互体验

## 🚀 快速开始

### 1. 上传图片

在仓库中创建 `images` 文件夹，上传您的图片：

```bash
ohku-gallery/
├── index.html
├── style.css
├── README.md
└── images/
    ├── monsters-all.jpg
    ├── pink-monster.jpg
    └── ... 更多图片
```

### 2. 修改图片引用

编辑 `index.html`，修改图片路径：

```html
<div class="gallery-item">
    <img src="images/your-image.jpg" alt="描述" loading="lazy">
    <p class="caption">图片说明 💕</p>
</div>
```

### 3. 启用 GitHub Pages

1. 进入仓库的 **Settings** 
2. 找到 **Pages** 选项
3. Source 选择 `main` 分支
4. 点击 **Save**
5. 等待几分钟，访问：`https://lluxixi55-blip.github.io/ohku-gallery/`

## 🎯 Retina 优化说明

### 为什么在 Mac 上看起来模糊？

Mac 的 Retina 显示屏像素密度是普通屏幕的 2-3 倍（DPR = 2 或 3）。如果图片分辨率不够，浏览器放大后会模糊。

### 本项目如何解决？

1. **CSS 优化**
   ```css
   img {
       image-rendering: -webkit-optimize-contrast;
       image-rendering: crisp-edges;
   }
   ```

2. **高分辨率图片**
   - 建议上传至少 **2000px 宽度**的图片
   - 图片质量设置为 **90%** 以上

3. **硬件加速**
   ```css
   transform: translateZ(0);
   -webkit-backface-visibility: hidden;
   ```

### 图片上传建议

| 屏幕类型 | 建议宽度 | 文件大小 |
|---------|---------|----------|
| 普通屏幕 | 1000px | < 500KB |
| Retina 2x | 2000px | < 1MB |
| Retina 3x | 3000px | < 2MB |

## 📸 使用的图片

- OHKU 可爱小怪物玩偶系列
- 高清产品摄影
- 粉色系主题风格

## 🛠️ 技术栈

- HTML5
- CSS3 (Grid + Flexbox)
- Retina 优化技术
- 响应式设计
- GitHub Pages

## 💡 更多自定义

### 更改配色

编辑 `style.css` 中的颜色变量：

```css
/* 主色调 */
background: linear-gradient(135deg, #ffeef8 0%, #ffe0f0 100%);

/* 强调色 */
color: #ff69b4;
```

### 添加更多图片

复制 `gallery-item` 代码块：

```html
<div class="gallery-item">
    <img src="images/new-image.jpg" alt="新图片" loading="lazy">
    <p class="caption">新图片说明 ✨</p>
</div>
```

## 📝 License

MIT License - 随意使用和修改！

## 💖 致谢

感谢 OHKU 品牌提供的可爱玩偶设计灵感！

---

Made with 💕 by lluxixi55-blip | Optimized for Retina Display ✨
