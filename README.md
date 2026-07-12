# AetherTab

![Preview](gif/anime.gif)

> Кастомизируемая стартовая страница для новой вкладки браузера.

---

## Что это и зачем нужно

**AetherTab** — это альтернатива стандартной «пустой» новой вкладке браузера. Вместо
бесполезного белого экрана или навязчивой ленты новостей вы открываете личное
пространство: живой аниме-фон, погоду, быстрый поиск, любимые ссылки, заметки и
музыку — всё в одном месте, без регистрации и серверов.

Проект задуман как **полностью локальный и приватный**: вся конфигурация хранится
в `localStorage` прямо в браузере, никакие данные никуда не отправляются. Один
HTML-файл — и страница готова. Это удобно тем, кто хочет видеть нужную информацию
сразу при открытии вкладки, не разводя отдельных вкладок и расширений.

Отдельная фишка — встроенный **СДВГ-режим**: хаотичный набор мини-игр и видео,
который помогает переключить внимание или просто отвлечься на пару минут, не
уходя со стартовой страницы.

---

## Как пользоваться

Самый простой способ — поставить расширение
[Custom New Tab URL](https://chromewebstore.google.com/detail/custom-new-tab-url/mmjbdbjnoablegbkcklggeknkfcjkjia)
и указать в его настройках ссылку на страницу:

[https://tronxer.github.io/aethertab/](https://tronxer.github.io/aethertab/)

Либо просто откройте `index.html` локально (см. «Локальный запуск»).

---

## Возможности

- **Аниме GIF-фон** — сетка превью + своя загрузка
- **Погода** (wttr.in) + прогноз на 2 дня
- **Поиск Google** с автодополнением (JSONP + подсказки Wikipedia)
- **Иконки быстрого доступа** с favicon, несколько панелей, drag-n-drop, удаление
- **Заметки** с drag-n-drop и курсами валют
- **Музыкальный плеер** (Web Audio API, lofi + загрузка своих треков), громкость
  задаётся ползунком (0 — выключено)
- **Эффекты частиц** — сакура, дождь, снег, огонь, неон, пепел
- **Часы** с отдельным попапом настроек и перетаскиваемым виджетом
- **Стеклянный дизайн** (glassmorphism) + прозрачный режим
- **Режим редактирования** — долгое нажатие или кнопка-карандаш
- **Экспорт / импорт настроек** (все настройки в localStorage)
- Настройки сохраняются между сессиями

---

## СДВГ-режим 🎮

В настройках есть блок **«СДВГ мод»**:
- Кнопка активации с подтверждением (`Вы уверены?`)
- После включения по экрану летает кнопка, которую нужно поймать и кликнуть 5 раз
- Затем запускается хаотичный набор окон-игр (без меню и пауз):

| Игра | Управление |
|------|-----------|
| 🐍 Змейка (с порталами по краям) | Стрелки / WASD |
| 🐸 Doodle Jump | ← → / A D, прыжок авто |
| 1024 | Стрелки / WASD |
| 🟦 Тетрис | ← → / A D, ↓ / S, Пробел — дроп |
| 👾 Пакман | Стрелки / WASD |
| 🦖 Динозаврик | Пробел / ↑ / W — прыжок |
| 🔫 Бак Шот Рулет | кнопки «Себе» / «Боту» |
| ▶️ Видео (Subway Surfers + мойка) | — |
| 🎬 Локальный клип, GIF iShowSpeed, GIF Brian | — |

- Окна перетаскиваются за заголовок, закрываются крестиком, при генерации
  не накладываются друг на друга
- Клик по окну поднимает его на передний план
- Медиа (GIF/видео) хранятся локально в папке `gif/`
- Отключение режима — кнопка «умоляю нажми» в настройках

---

## Локальный запуск

Просто откройте `index.html` в браузере. Для корректной работы внешних ресурсов
(погода, поиск) рекомендуется локальный сервер:

```bash
python -m http.server
```

Затем откройте `http://localhost:8000`.

---

# AetherTab (English)

![Preview](gif/anime.gif)

> A customizable new-tab start page for your browser.

---

## What is it and why

**AetherTab** is an alternative to the browser's default blank new-tab page. Instead of
an empty white screen or an intrusive news feed, you get a personal space: a live
anime GIF background, weather, instant search, your favorite links, notes and music —
all in one place, with no sign-up and no servers.

The project is built to be **fully local and private**: all configuration lives in the
browser's `localStorage`, and nothing is sent anywhere. A single HTML file is all you
need. It's perfect for anyone who wants the right information at a glance every time
they open a tab, without juggling separate extensions.

A special feature is the built-in **ADHD mode**: a chaotic set of mini-games and videos
that helps you switch focus or just take a short break without leaving the start page.

---

## How to use

The easiest way is to install the
[Custom New Tab URL](https://chromewebstore.google.com/detail/custom-new-tab-url/mmjbdbjnoablegbkcklggeknkfcjkjia)
extension and set its start URL to:

[https://tronxer.github.io/aethertab/](https://tronxer.github.io/aethertab/)

Or just open `index.html` locally (see "Run locally").

---

## Features

- **Anime GIF background** — preview grid + upload your own
- **Weather** (wttr.in) + 2-day forecast
- **Google search** with autocomplete (JSONP + Wikipedia suggestions)
- **Quick-access icons** with favicons, multiple panels, drag-n-drop, removable
- **Notes** with drag-n-drop and currency rates
- **Music player** (Web Audio API, lofi + upload your own tracks), volume slider
  (0 = off)
- **Particle effects** — sakura, rain, snow, fire, neon, ash
- **Clock** with its own settings popup and a draggable widget
- **Glassmorphism design** + transparent mode
- **Edit mode** — long press or the pencil button
- **Export / import settings** (everything in localStorage)
- Settings persist across sessions

---

## ADHD mode 🎮

The settings panel has an **"ADHD mode"** section:
- An activation button with a confirmation (`Are you sure?`)
- After enabling, a floating button flies around the screen — catch and click it 5 times
- Then a chaotic set of game windows launches (no menu, no pause):

| Game | Controls |
|------|---------|
| 🐍 Snake (with edge portals) | Arrows / WASD |
| 🐸 Doodle Jump | ← → / A D, auto jump |
| 1024 | Arrows / WASD |
| 🟦 Tetris | ← → / A D, ↓ / S, Space — hard drop |
| 👾 Pac-Man | Arrows / WASD |
| 🦖 Dino | Space / ↑ / W — jump |
| 🔫 Buckshot Roulette | "Self" / "Bot" buttons |
| ▶️ Video (Subway Surfers + carpet wash) | — |
| 🎬 Local clip, iShowSpeed GIF, Brian GIF | — |

- Windows are dragged by their header, closed with the × button, and never overlap
  on spawn
- Clicking a window brings it to the front
- Media (GIF/video) is stored locally in the `gif/` folder
- Disable via the "please click" button in settings

---

## Run locally

Just open `index.html` in your browser. For external resources (weather, search) to
work reliably, a local server is recommended:

```bash
python -m http.server
```

Then open `http://localhost:8000`.
