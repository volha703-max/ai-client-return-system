# CLAUDE.md — Контекст проекта для Claude

## Кто владелец
Ольга. Telegram: @olga1222. GitHub: volha703-max (email: volha703@gmail.com).

## Что за проект
Личный портфолио-сайт на GitHub Pages. Набор HTML-страниц без фреймворков — чистый HTML/CSS/JS.

## Живые ссылки
- Главная (все проекты): https://volha703-max.github.io/my-first-project/
- Визитка: https://volha703-max.github.io/my-first-project/vizitka.html
- Лендинг (калькуляторы): https://volha703-max.github.io/my-first-project/landing.html
- Лендинг (AI-консультант): https://volha703-max.github.io/my-first-project/ai-consultant.html

## Файлы проекта
- `index.html` — главная страница-портфолио с карточками всех проектов
- `vizitka.html` — личная визитка с фото (base64), 3D-tilt, анимацией
- `landing.html` — лендинг "Умные калькуляторы для бизнеса"
- `ai-consultant.html` — лендинг "AI-консультант по автоматизации"
- `photo_nobg.jpg` — фото Ольги с удалённым фоном (через rembg)

## Стиль и цвета (единый для всех страниц)
- Фон: #020d0d
- Акценты: #00e5c3 (бирюза), #00ff88 (зелёный), #0099ff (синий)
- Блобы: #005544, #003366, #00442a
- Градиент: linear-gradient(120deg, #00e5c3, #00ff88 45%, #0099ff 80%, #00e5c3)
- Фоновая анимация: плавающие математические/AI символы на canvas
- Шрифт: 'Segoe UI', system-ui, sans-serif

## GitHub
- Репозиторий: https://github.com/volha703-max/my-first-project
- Ветка: main
- GitHub Pages включён, источник: branch main, папка /
- PAT токен сохранён в C:\Users\Lenovo\.git-credentials

## Важные правила
- Все новые страницы делать в том же тёмном стиле (бирюза/зелёный/синий)
- После изменений всегда делать git add + commit + push
- После push добавлять новую карточку в index.html
- vizitka.html очень большой файл (base64 фото) — читать только нужные части с offset/limit
