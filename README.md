# 🏛️ National Gallery — Website with JavaScript Art Slider

![Скриншот главной страницы](img/screen.png)

> **Примечание**: Проект не имеет адаптивного дизайна и оптимизирован только для desktop-устройств

### 🛠 Технологии

- HTML5
- CSS3
- JavaScript (нативный слайдер)

### 🎨 Особенности реализации

#### JavaScript слайдер
```javascript
const slides = document.querySelectorAll('.slide');
let currentSlide = 0;

function showSlide(n) {
  slides.forEach(slide => {
    slide.style.display = 'none';
  });
  slides[n].style.display = 'block';
}
```

#### HTML структура
```html
<div class="gallery">
  <div class="slide">
    <img src="art1.jpg" alt="Картина 1">
    <div class="art-description">...</div>
  </div>
  <!-- Другие слайды -->
  <button class="prev">←</button>
  <button class="next">→</button>
</div>
```

### ⚠️ Ограничения

- Только desktop-версия (1280px+)
- Нет touch-поддержки для мобильных устройств
- Фиксированная ширина контейнера

### 🚀 Запуск
1. Клонируйте репозиторий
2. Откройте `index.html` в десктопном браузере

---

<div align="center">
  <sub>Учебный проект | 2023</sub>
</div>
