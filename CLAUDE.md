# CLAUDE.md — my-first-project (ai-client-return-system)

*Профиль Ольги и общие правила: `Projects/_docs/user-profile.md`*
*Дизайн-система: `Projects/_brand-cosmetolog/design-system.md`*

---

## GitHub
- Репозиторий: https://github.com/volha703-max/ai-client-return-system
- Ветка: main
- GitHub Pages включён, источник: branch main, папка /

## Живые ссылки

### Портфолио Ольги (светлая тема)
- Главная: https://volha703-max.github.io/ai-client-return-system/index.html

### Калькуляторы (тёмная тема — бирюза)
- Визитка: https://volha703-max.github.io/ai-client-return-system/vizitka_kalkulyator.html
- Лендинг: https://volha703-max.github.io/ai-client-return-system/landing_kalkulyator.html

### Проект «Косметолог» (светлая тема)
- Лендинг: https://volha703-max.github.io/ai-client-return-system/landing-cosmetolog.html
- Визитка: https://volha703-max.github.io/ai-client-return-system/vizitka-cosmetolog.html

## Технические правила
- Каждая страница — один самодостаточный HTML-файл (CSS и JS внутри)
- Никаких внешних библиотек и CDN — только чистый HTML/CSS/JS
- `vizitka-cosmetolog.html` большой (base64 фото) — читать с offset/limit!
- После любых изменений: git add + commit + push
- Рабочая папка: `C:\Users\Lenovo\OneDrive\Документы\Projects\my-first-project`

## Файлы проекта

| Файл | Статус | Тема |
|---|---|---|
| `index.html` | Активная разработка | Светлая — портфолио Ольги |
| `landing-cosmetolog.html` | ЗАМОРОЖЕН — не трогать | Светлая — для косметолога |
| `vizitka-cosmetolog.html` | Готов (base64 фото!) | Светлая — для косметолога |
| `vizitka_kalkulyator.html` | Готов | Тёмная — калькулятор |
| `landing_kalkulyator.html` | Готов | Тёмная — калькулятор |

## Что сделано в index.html
- Лендинг-портфолио Ольги: 13 секций
- Nav → Hero → Статистика → Проблема → Решение → Процесс → Кейсы → Тарифы → Обо мне → Отзывы → FAQ → Форма → Footer
- Фото Ольги встроено в base64 (~200 KB)
- Адаптив от 320px, приоритет мобильная версия

## Что ещё не сделано
- Telegram-бот с квизом и формой заявки
- Реальные кейсы и отзывы (когда появятся клиенты)
- Страница «Обо мне» отдельная

## Документация
- [brief.md](brief.md) — ТЗ на лендинг
- [research.md](research.md) — исследование рынка
