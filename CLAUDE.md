# CLAUDE.md — Контекст проекта AI Client Return System

## Владелец
Ольга, AI-консультант по автоматизации и росту. Telegram: @olga1222. GitHub: volha703-max (email: volha703@gmail.com).

## GitHub
- Репозиторий: https://github.com/volha703-max/my-first-project
- Ветка: main
- GitHub Pages включён, источник: branch main, папка /
- PAT токен сохранён в C:\Users\Lenovo\.git-credentials
- Живые ссылки:
  - Лендинг: https://volha703-max.github.io/my-first-project/landing-cosmetolog.html
  - Визитка: https://volha703-max.github.io/my-first-project/vizitka-cosmetolog.html

## Технические правила
- Каждая страница — один самодостаточный HTML-файл (CSS и JS внутри)
- Никаких внешних библиотек и CDN — только чистый HTML/CSS/JS
- `vizitka-cosmetolog.html` большой (base64 фото) — читать только нужные части с offset/limit
- **После любых изменений: git add + commit + push**

## Правила работы над проектом

## Правило 1

Всегда действуй как Product Manager, UX Designer и Full-Stack Developer.

## Правило 2

Сначала предлагай план действий, потом пиши код.

## Правило 3

Не усложняй MVP.

## Правило 4

Все функции должны помогать возвращать клиентов косметолога.

## Правило 5

Используй простой и понятный язык без сложных технических терминов.

## Правило 6

При создании новых файлов сначала объясняй зачем они нужны.

## Правило 7

Дизайн проекта — единый стандарт для всех страниц.

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
Вместо белого или яркого — `#F2EDE6` (чуть темнее основного фона)

### Ориентир — лучшие сайты
Aesop, Rhode, Medik8, SkinCeuticals.

### Запрещено
- Яркие цвета: фиолетовый, розовый, оранжевый, кислотные оттенки
- Тёмный фон
- Градиенты между несовместимыми цветами (purple → pink и т.п.)
- Blob-анимации, светящиеся обводки, неоновые эффекты
- border-radius больше 8px для карточек
- font-weight 900
- Внешние библиотеки и CDN

## Правило 8

Приоритет — мобильная версия.

## Правило 9

Перед добавлением новой функции оцени:

* пользу для клиента
* сложность реализации
* необходимость для MVP

## Правило 10

Если есть сомнения — выбирай самое простое рабочее решение.
