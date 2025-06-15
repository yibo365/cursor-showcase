# 图片资源目录

此目录用于存放演示文档中使用的图片资源。

## 使用方法

在 Slidev 中引用图片时，使用以下格式：

```markdown
![图片描述](/images/filename.png)
```

或者使用 HTML 标签（支持更多自定义属性）：

```html
<img src="/images/filename.png" alt="图片描述" class="w-full" />
```

## 支持的图片格式

- PNG
- JPG/JPEG  
- WebP
- SVG
- GIF

## 图片 Lightbox 功能

### 基础点击放大

为图片添加点击放大功能：

```html
<img 
  src="/images/example.png" 
  alt="示例图片" 
  class="w-full cursor-pointer hover:opacity-80 transition-opacity" 
  onclick="openLightbox(this)"
/>
```

### 图片画廊（支持左右滑动）

创建图片画廊，支持键盘和鼠标操作：

```html
<div class="image-gallery">
  <img src="/images/img1.jpg" alt="图片1" onclick="openGallery(0)" />
  <img src="/images/img2.jpg" alt="图片2" onclick="openGallery(1)" />
  <img src="/images/img3.jpg" alt="图片3" onclick="openGallery(2)" />
</div>

<script>
const galleryImages = [
  { src: '/images/img1.jpg', alt: '图片1' },
  { src: '/images/img2.jpg', alt: '图片2' },
  { src: '/images/img3.jpg', alt: '图片3' }
];

let currentIndex = 0;

function openGallery(index) {
  currentIndex = index;
  showGalleryImage();
  document.getElementById('gallery-lightbox').classList.remove('hidden');
}

function nextImage() {
  currentIndex = (currentIndex + 1) % galleryImages.length;
  showGalleryImage();
}

function prevImage() {
  currentIndex = (currentIndex - 1 + galleryImages.length) % galleryImages.length;
  showGalleryImage();
}

function showGalleryImage() {
  const img = document.getElementById('gallery-img');
  img.src = galleryImages[currentIndex].src;
  img.alt = galleryImages[currentIndex].alt;
}
</script>
```

## 文件命名规范

建议使用以下命名规范：

- 使用小写字母和连字符
- 避免使用空格和特殊字符
- 示例：`agent-workflow.png`、`cursor-demo-screenshot.jpg`

## 优化建议

1. **图片压缩**：上传前请压缩图片以提高加载速度
2. **适当尺寸**：根据使用场景选择合适的图片尺寸
3. **格式选择**：
   - 照片类图片：使用 JPG
   - 图标、简单图形：使用 PNG 或 SVG
   - 动图：使用 GIF 或 WebP

## 示例
如果您有一个名为 `agent-workflow.png` 的图片文件：
1. 将文件放在：`public/images/agent-workflow.png`
2. 在 slides.md 中引用：`/images/agent-workflow.png`

## 注意事项
- 路径以 `/` 开头（相对于 public 目录）
- 文件名区分大小写
- 建议使用小写文件名和连字符分隔 