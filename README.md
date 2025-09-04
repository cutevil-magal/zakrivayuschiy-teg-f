# Закрывающий тег — Интерактивная веб-галерея

**Современная адаптивная веб-галерея с интерактивными элементами и анимациями**

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/ru/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/ru/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/ru/docs/Web/JavaScript)
[![SVG](https://img.shields.io/badge/SG-FFB13B?style=for-the-badge&logo=svg&logoColor=white)](https://developer.mozilla.org/ru/docs/Web/SVG)

---

## 📖 О проекте

Я разработала интерактивную веб-галерею Закрывающий тег, которая сочетает в себе современный дизайн с продвинутыми CSS-анимациями и JavaScript-взаимодействиями. Проект демонстрирует передовые подходы к веб-разработке с акцентом на пользовательский опыт и визуальную привлекательность.

### 🎯 Ключевые особенности

- **Интерактивная система лайков** с анимированными SVG-сердцами
- **CSS-фильтры** для создания уникальных визуальных эффектов на изображениях
- **Адаптивный дизайн** с поддержкой мобильных устройств и десктопов
- **Модальные окна** с использованием элемента `<dialog>`
- **Продвинутые CSS-анимации** с плавными переходами
- **Семантическая верстка** с акцентом на доступность

### 🛠 Технологический стек

**Frontend:**
- HTML5 (семантическая разметка, dialog element)
- CSS3 (Grid, Flexbox, Filters, Animations, Variables)
- Vanilla JavaScript (ES6+)
- SVG (инлайновые иконки с анимацией)

**Особенности реализации:**
- CSS Filters (blur, brightness, contrast, grayscale, saturate, sepia)
- SVG анимации с изменяющимися путями
- CSS Custom Properties для управления темами
- Lazy loading изображений
- Modern dialog API для модальных окон

---

## 🚀 Быстрый старт

### Посмотреть онлайн

🌐 **[Живая демо-версия](https://cutevil-magal.github.io/zakrivayuschiy-teg-f/)**

### Запуск локально

1. **Клонирование репозитория**
   ```bash
   git clone https://github.com/cutevil-magal/zakrivayuschiy-teg-f.git
   cd zakrivayuschiy-teg-f
   ```

2. **Запуск проекта**
   - Откройте файл `index.html` в браузере
   - Для разработки рекомендуется использовать Live Server

### Системные требования
- Современный браузер с поддержкой CSS Filters и ES6+
- Разрешение экрана не менее 320px
- Включенный JavaScript для интерактивных функций

---

## 📁 Структура проекта

```
zakrivayuschiy-teg-f/
├── index.html              # Главная страница
├── styles/
│   ├── variables.css       # CSS-переменные
│   ├── globals.css         # Глобальные стили
│   ├── style.css           # Основные стили
│   ├── animations.css      # Анимации
│   └── themes.css          # Стили тем
├── fonts/                  # Локальные шрифты
├── images/                 # Изображения
├── svg/                    # SVG-иконки
├── scripts/
│   ├── like.js             # Логика лайков
│   └── set-theme.js        # Управление темами
└── README.md               # Документация
```

---

## 🎨 Особенности реализации

### Интерактивная система лайков
```javascript
function toggleIsLiked(heart, button) {
  heart.classList.toggle('is-liked');
  setButtonText(heart, button);
}
```

### CSS-фильтры для изображений
```css
.filter-brightness {
  filter: brightness(120%);
}

.filter-contrast {
  filter: contrast(150%);
}

.filter-blur {
  filter: blur(2px);
}
```

### SVG анимации
```css
.like-icon .contour {
  fill: var(--heart-contour);
  transition: fill 0.1s linear;
}

.like-icon.is-liked .contour {
  fill: var(--heart-sparks);
  transition: fill 0.3s 0.06s linear;
}
```

### Модальное окно
```html
<dialog id="dialog-id" class="content__dialog">
  <form class="content__dialog-form" method="dialog">
    <svg class="content__dialog-icon">
      <use href="svg/floppy_big.svg#icon-disk-2"/>
    </svg>
    <button type="button" onclick="window['dialog-id'].close()">
      <span class="button__text">ОК</span> 
    </button>
  </form>
</dialog>
```

---

## 🎯 Результаты реализации

**Достигнутые цели:**
- ✅ Полнофункциональная система лайков с анимациями
- ✅ Уникальные CSS-фильтры для каждого изображения
- ✅ Адаптивность для всех типов устройств
- ✅ Семантическая верстка с доступностью
- ✅ Оптимизированная производительность загрузки

**Технические преимущества:**
- Чистая семантическая верстка
- Современные CSS-технологии (Grid, Filters, Animations)
- Оптимизированные медиа-запросы
- Плавные анимации и переходы
- Доступность для screen readers

---

## 🔮 Планы по развитию

- [ ] Добавить PWA-функциональность
- [ ] Реализовать офлайн-режим
- [ ] Добавить систему комментариев
- [ ] Интегрировать бэкенд для сохранения лайков
- [ ] Реализовать бесконечную прокрутку
- [ ] Добавить дополнительные фильтры и эффекты

---

## 👩‍💻 Разработчик

**Анна Хвостикова** - Frontend Developer

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/cutevil-magal)
[![Email](https://img.shields.io/badge/Email-ana.magal@yandex.by-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ana.magal@yandex.by)

---

## 📄 Лицензия

Проект создан на основе дизайн-макета. Исходный код доступен для ознакомления и обучения.

**Макет в Figma:** [Ссылка на дизайн](https://www.figma.com/design/Yg5IFeWSyl6Js98kWROjVP/4-%D1%81%D0%BF%D1%80%D0%B8%D0%BD%D1%82.-%D0%9F%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%BD%D0%B0%D1%8F--%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%B0?node-id=0-1&p=f&t=VMKDUxPD8x2ZypHr-0)

---
