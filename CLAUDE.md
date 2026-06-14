# CLAUDE.md — Репозиторий ai-client-return-system

## Владелец
Ольга — специалист по созданию системы возврата клиентов для косметологов под ключ. Telegram: @olga1222. GitHub: volha703-max (email: volha703@gmail.com).

## Позиционирование проекта «Косметолог»
- **Кто:** Специалист по созданию системы возврата клиентов для косметологов под ключ
- **Что делает:** Создаёт сайты, квизы, чат-боты, автоматические напоминания — всё без участия клиента
- **Кому:** Косметологи, владельцы кабинетов и небольших студий
- **Боль клиента:** Клиенты приходят один раз и не возвращаются
- **Результат:** Система, которая возвращает клиентов автоматически
- **Язык:** Никаких слов «AI», «CRM», «воронка», «лид» — только понятные термины и результаты

## GitHub
- Репозиторий: https://github.com/volha703-max/ai-client-return-system
- Ветка: main
- GitHub Pages включён, источник: branch main, папка /
- PAT токен сохранён в C:\Users\Lenovo\.git-credentials

## Живые ссылки
### Портфолио
- Главная: https://volha703-max.github.io/ai-client-return-system/index.html
- Визитка личная: https://volha703-max.github.io/ai-client-return-system/vizitka_kalkulyator.html
- Калькуляторы: https://volha703-max.github.io/ai-client-return-system/landing_kalkulyator.html

### Проект «Косметолог»
- Лендинг: https://volha703-max.github.io/ai-client-return-system/landing-cosmetolog.html
- Визитка: https://volha703-max.github.io/ai-client-return-system/vizitka-cosmetolog.html

## Технические правила
- Каждая страница — один самодостаточный HTML-файл (CSS и JS внутри)
- Никаких внешних библиотек и CDN — только чистый HTML/CSS/JS
- `vizitka-cosmetolog.html` большой (base64 фото) — читать только нужные части с offset/limit
- **После любых изменений: git add + commit + push**
- Рабочая папка: `c:\Users\Lenovo\OneDrive\Документы\Projects\ai-client-return-system`

## Документация по проектам
- [plan-portfolio.md](plan-portfolio.md) — план портфолио-сайта
- [plan-cosmetolog.md](plan-cosmetolog.md) — план AI-системы для косметолога
- [project-cosmetolog.md](project-cosmetolog.md) — описание продукта для косметологов
- [brief.md](brief.md) — полное ТЗ на лендинг: 10 секций, тексты, дизайн, аудитория
- [research.md](research.md) — исследование рынка: конкуренты, тренды, экспертные оценки

---

## Текущее состояние проекта (обновлено 2026-06-14)

### Что уже сделано

**Главный файл — `index.html`** (активная разработка, все изменения только сюда):
- Полный лендинг-портфолио Ольги: 13 секций
- Секции: Nav → Hero → Статистика → Проблема → Решение → Процесс → Кейсы → Тарифы → Обо мне → Отзывы → FAQ → Форма → Финальный CTA → Footer
- Фото Ольги Жебрик встроено в base64 (~200 KB)
- Дизайн: светлая кремовая тема (#F7F4EF), акцент #B88A7A, стиль Aesop/Rhode
- Анимации: scroll-reveal, параллакс на фото, градиентный заголовок (gradientShift)
- Интерактивность: счётчики статистики, кнопка «Наверх», гамбургер-меню с X-анимацией, форма с анимацией успеха
- Адаптив от 320px, приоритет мобильная версия

**Остальные файлы:**
- `landing-cosmetolog.html` — ЗАМОРОЖЕН, не трогать без явной просьбы
- `vizitka-cosmetolog.html` — готов, содержит base64-фото (читать с offset/limit!)
- `vizitka_kalkulyator.html` — готов
- `landing_kalkulyator.html` — готов

### Что ещё не сделано (следующие шаги)
- Telegram-бот с квизом и формой заявки
- Реальные кейсы и отзывы (когда появятся клиенты)
- Страница «Обо мне» отдельная

### Правила взаимодействия с Ольгой
- Новичок в VS Code и Claude Code — объяснять каждый шаг простыми словами
- Git делать самому после каждого изменения (не давать команды пользователю)
- Сначала описывать план, потом делать
- Все ответы и вопросы — на русском языке
- Без эмодзи в ответах

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
