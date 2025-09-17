# Portfolio Website

موقع شخصي لعرض المشاريع والخبرات والشهادات.

## إضافة الصور والفيديوهات

### صور الشهادات
ضع صور الشهادات في مجلد `images/certificates/`:
- `nti-cybersecurity.jpg` - شهادة الأمن السيبراني من NTI
- يمكن إضافة المزيد من الشهادات بنفس الطريقة

### صور المشاريع (Thumbnails)
ضع صور المشاريع في مجلد `images/projects/`:
- `market-app-thumbnail.jpg` - صورة مشروع Market App
- `zakir-app-thumbnail.jpg` - صورة مشروع Zakir App
- `iot-sensor-thumbnail.jpg` - صورة مشروع IoT Sensor

### فيديوهات المشاريع
ضع فيديوهات المشاريع في مجلد `videos/`:
- `market-app-demo.mp4` - فيديو توضيحي لمشروع Market App
- `zakir-app-demo.mp4` - فيديو توضيحي لمشروع Zakir App
- `iot-sensor-demo.mp4` - فيديو توضيحي لمشروع IoT Sensor

## تنسيقات الملفات المدعومة

### الصور
- JPG/JPEG
- PNG
- WebP

### الفيديوهات
- MP4 (مستحسن)
- WebM (للتوافق مع المتصفحات)

## نصائح للصور والفيديوهات

### الصور
- حجم الصور: 800x600 بكسل أو أكبر
- نسبة العرض إلى الارتفاع: 4:3 أو 16:9
- حجم الملف: أقل من 2MB للصفحة

### الفيديوهات
- مدة الفيديو: 30-60 ثانية
- دقة الفيديو: 720p أو أعلى
- حجم الملف: أقل من 10MB
- تنسيق MP4 مع H.264 للتوافق الأفضل

## كيفية إضافة شهادة جديدة

1. ضع صورة الشهادة في `images/certificates/`
2. افتح `index.html`
3. ابحث عن قسم Experience
4. أضف كود HTML جديد:

```html
<div class="certificate-item">
  <img src="images/certificates/اسم-الشهادة.jpg" alt="وصف الشهادة" class="certificate-img" />
  <p class="certificate-caption">اسم الشهادة</p>
</div>
```

## كيفية إضافة مشروع جديد

1. ضع صورة المشروع في `images/projects/`
2. ضع فيديو المشروع في `videos/`
3. افتح `index.html`
4. ابحث عن قسم Projects
5. أضف كود HTML جديد:

```html
<article class="card">
  <div class="card-media">
    <video class="project-video" controls poster="images/projects/اسم-المشروع-thumbnail.jpg">
      <source src="videos/اسم-المشروع-demo.mp4" type="video/mp4">
      <source src="videos/اسم-المشروع-demo.webm" type="video/webm">
      Your browser does not support the video tag.
    </video>
  </div>
  <div class="card-body">
    <h3>اسم المشروع</h3>
    <p>وصف المشروع</p>
    <div class="card-actions">
      <a href="#" class="btn btn-small">Live</a>
      <a href="#" class="btn btn-small btn-ghost">Source</a>
    </div>
  </div>
</article>
```