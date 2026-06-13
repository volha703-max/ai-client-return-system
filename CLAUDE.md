# CLAUDE.md — Репозиторий my-first-project

## Владелец
Ольга, AI-консультант по автоматизации и росту. Telegram: @olga1222. GitHub: volha703-max (email: volha703@gmail.com).

## GitHub
- Репозиторий: https://github.com/volha703-max/my-first-project
- Ветка: main
- GitHub Pages включён, источник: branch main, папка /
- PAT токен сохранён в C:\Users\Lenovo\.git-credentials

## Живые ссылки
### Портфолио
- Главная: https://volha703-max.github.io/my-first-project/index.html
- Визитка личная: https://volha703-max.github.io/my-first-project/vizitka_kalkulyator.html
- Калькуляторы: https://volha703-max.github.io/my-first-project/landing_kalkulyator.html

### Проект «Косметолог»
- Лендинг: https://volha703-max.github.io/my-first-project/landing-cosmetolog.html
- Визитка: https://volha703-max.github.io/my-first-project/vizitka-cosmetolog.html

## Технические правила
- Каждая страница — один самодостаточный HTML-файл (CSS и JS внутри)
- Никаких внешних библиотек и CDN — только чистый HTML/CSS/JS
- `vizitka-cosmetolog.html` большой (base64 фото) — читать только нужные части с offset/limit
- **После любых изменений: git add + commit + push**
- Рабочая папка: `c:\Users\Lenovo\OneDrive\Документы\Projects\my-first-project`

## Документация по проектам
- [plan-portfolio.md](plan-portfolio.md) — план портфолио-сайта
- [plan-cosmetolog.md](plan-cosmetolog.md) — план AI-системы для косметолога
- [project-cosmetolog.md](project-cosmetolog.md) — описание продукта для косметологов

---

## Дизайн — Портфолио (тёмная тема)

Применяется к: `index.html`, `vizitka_kalkulyator.html`, `landing_kalkulyator.html`

### Цвета
```css
:root {
  --bg:     #020d0d;   /* тёмный фон */
  --text:   #e0fff8;   /* светлый текст */
  --accent: #00e5c3;   /* бирюза */
  --green:  #00ff88;   /* зелёный */
  --blue:   #0099ff;   /* синий */
  --blob1:  #005544;
  --blob2:  #003366;
  --blob3:  #00442a;
}
```

### Градиент
```css
linear-gradient(120deg, #00e5c3, #00ff88 45%, #0099ff 80%, #00e5c3)
```

### Шрифт
```css
font-family: 'Segoe UI', system-ui, sans-serif;
```

### Стиль
- Тёмный фон, светлый текст
- Бирюзово-голубые акценты
- Плавающие символы на canvas
- Адаптивная вёрстка от 320px

---

## Дизайн — Косметолог (светлая тема)

Применяется к: `landing-cosmetolog.html`, `vizitka-cosmetolog.html`

### CSS-переменные (копировать в каждую страницу)
```css
:root {
  --bg:     #F7F4EF;   /* светлый кремовый фон */
  --text:   #3A3A3A;   /* тёмно-серый текст */
  --accent: #B88A7A;   /* пудрово-бежевый акцент */
  --soft:   #E7D6CF;   /* мягкий бежевый */
  --muted:  #9A8880;   /* приглушённый текст */
  --card:   #FFFFFF;   /* белые карточки */
  --border: #EDE6DF;   /* очень светлая рамка */
}
```

### Шрифт
```css
font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', system-ui, sans-serif;
```

### Типографика
- Заголовки: font-weight 700 (не 900), letter-spacing -0.5px...-1.5px
- Подписи/лейблы: font-size 10–11px, font-weight 600, letter-spacing 2.5–3px, uppercase, color var(--accent)
- Основной текст: font-weight 400, line-height 1.65–1.75
- Приглушённый текст: color var(--muted)

### Карточки
```css
background: var(--card);
border: 1px solid var(--border);
border-radius: 4px;
box-shadow: 0 2px 40px rgba(184,138,122,0.08);
```

### Кнопки
```css
background: var(--accent);
color: #FFFFFF;
border-radius: 2px;
padding: 16px 40px;
font-weight: 600;
font-size: 15px;
transition: background 0.2s, transform 0.2s;
/* hover: background #a57a6b, transform: translateY(-2px) */
```

### Разделители
```css
width: 36–40px; height: 1–2px;
background: var(--accent);
opacity: 0.45;
```

### Анимации
- Только тихий fadeIn: `opacity 0 → 1` + `translateY(18px) → 0`
- Длительность 0.6–0.8s ease
- Scroll-reveal для секций: `opacity 0 → 1`, `translateY(24px) → 0`, transition 0.65s

### Секции с другим фоном
Вместо белого — `#F2EDE6` (чуть темнее основного фона)

### Ориентир
Aesop, Rhode, Medik8, SkinCeuticals.

### Запрещено для косметолога
- Яркие цвета: фиолетовый, розовый, оранжевый, кислотные оттенки
- Тёмный фон
- Градиенты между несовместимыми цветами
- Blob-анимации, светящиеся обводки, неоновые эффекты
- border-radius больше 8px для карточек
- font-weight 900

---

## Общие правила работы

1. Действуй как Product Manager, UX Designer и Full-Stack Developer
2. Сначала предлагай план, потом пиши код
3. Не усложняй MVP
4. Простой язык без технического жаргона
5. Перед новым файлом — объясни зачем он нужен
6. Приоритет — мобильная версия
7. Если есть сомнения — выбирай самое простое рабочее решение
