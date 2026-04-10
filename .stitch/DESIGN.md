# Design System — АО «Победит»

> **Статус:** черновик на основе visual direction. Обновить после первой генерации home screen в Stitch (запусти skill `design-md` и уточни токены по скриншоту).

---

## 1. Design Direction

**Industrial Corporate B2B — Engineering Precision**

Сайт АО «Победит» визуально транслирует: зрелость, надёжность, инженерную точность и промышленный масштаб. Это не стартап, не SaaS, не маркетинговый лендинг. Это корпоративный сайт серьёзного производителя с 70-летней историей, продуктовым каталогом в ядре и B2B-аудиторией, которая принимает технические и коммерческие решения.

**Что делает этот стиль правильным именно для АО «Победит»:**
- Завод производит прецизионные промышленные материалы — визуальный язык должен отражать точность и строгость
- Аудитория — инженеры, технологи, закупщики, снабженцы — профессионалы, которые доверяют данным, а не украшениям
- 70+ лет истории требуют визуальной зрелости, а не трендовости
- B2B-сделки строятся на доверии — дизайн должен его формировать с первого экрана

---

## 2. Typography

### Typeface
- **Primary:** Inter (или аналог — IBM Plex Sans, Roboto) — геометрический гротеск, высокая читаемость, технический характер
- **Tabular / Technical data:** Inter с включёнными tabular figures (`font-variant-numeric: tabular-nums`) — для таблиц, характеристик, цифровых данных
- Никаких serif, рукописных или декоративных шрифтов

### Type Scale (базовый размер — 16px)

| Назначение | Размер | Weight | Line-height |
|---|---|---|---|
| H1 (hero) | 56–64px | 700 | 1.1 |
| H2 (section) | 36–42px | 700 | 1.2 |
| H3 (subsection) | 24–28px | 600 | 1.3 |
| H4 (card title) | 18–20px | 600 | 1.4 |
| Body (основной) | 16–18px | 400 | 1.6 |
| Body small | 14px | 400 | 1.5 |
| Label / caption | 12px | 500 | 1.4 |
| Technical data | 14–16px | 400–500 | 1.5 |

### Принципы типографики
- Заголовки — крупные, уверенные, с минимальным межстрочным интервалом
- Текст — плотный, информационно насыщенный, без избыточного воздуха внутри параграфов
- Uppercase — только для labels, nav-items и коротких технических меток
- Letter-spacing для заголовков: -0.02em (tight); для labels uppercase: +0.08em

---

## 3. Color Palette

### Core Palette

| Роль | Название | HEX | Применение |
|---|---|---|---|
| Background (dark) | Midnight Navy | `#0B1728` | Hero background, dark секции, footer |
| Background (light) | Off-White | `#F5F5F3` | Основной фон страниц |
| Background (mid) | Slate 50 | `#F0F2F5` | Зебра-фон карточек, разделители секций |
| Primary text | Near Black | `#111827` | Основной текст на светлом фоне |
| Secondary text | Steel Gray | `#6B7280` | Подзаголовки, описания, meta |
| Muted text | Light Gray | `#9CA3AF` | Captions, disabled, placeholder |
| Accent (primary) | Industrial Amber | `#D97706` | Primary CTA, активные ссылки, highlights |
| Accent (secondary) | Steel Blue | `#2563EB` | Secondary CTA, ссылки в тексте |
| Border | Hairline | `#E5E7EB` | Разделители, бордюры карточек |
| Border (dark) | Dark Divider | `#1E2D42` | Разделители на тёмном фоне |
| Success | — | `#16A34A` | Статусы, индикаторы наличия |
| Warning | — | `#CA8A04` | Предупреждения |

### Принципы контрастов
- Основной текст на белом/off-white: контраст ≥ 7:1 (WCAG AAA)
- Accent на белом: контраст ≥ 4.5:1 (WCAG AA)
- Белый текст на Midnight Navy: контраст ≈ 15:1
- CTA-кнопки: всегда высококонтрастная пара (фон/текст)
- Никаких светло-серых текстов на белом фоне — только Steel Gray #6B7280 и темнее

---

## 4. Spacing System

Базовая единица: **8px**

| Токен | Значение | Применение |
|---|---|---|
| `space-1` | 4px | Micro gaps — между иконкой и меткой |
| `space-2` | 8px | Базовый gap — padding внутри badge/tag |
| `space-3` | 12px | Внутренний padding малых элементов |
| `space-4` | 16px | Стандартный internal padding |
| `space-6` | 24px | Gap между элементами в строке |
| `space-8` | 32px | Вертикальный rhythm внутри секции |
| `space-12` | 48px | Отступ между крупными элементами |
| `space-16` | 64px | Секционный отступ (padding-top/bottom) |
| `space-24` | 96px | Большой секционный отступ (hero, featured) |
| `space-32` | 128px | Максимальный секционный отступ |

---

## 5. Grid & Layout

### Container
- Max-width: **1280px** (с padding по 40px на каждую сторону)
- На мобильном: padding 16–20px
- Центрирование по горизонтали

### Grid
- Base grid: **12 колонок**, gap 24px
- Sectional layouts:
  - 3 равные колонны (4-4-4) — каталожные направления, преимущества
  - 2 колонны (8-4 или 7-5) — контент + sidebar, текст + CTA
  - 4 колонны (3-3-3-3) — отраслевые иконки, мелкие факты
  - Full-width — hero, CTA band, footer
- На планшете: 2 колонны (6-6)
- На мобильном: 1 колонна (12)

### Section Rhythm
- Каждая секция: `padding-top: 80px; padding-bottom: 80px`
- Hero: `padding-top: 120px; padding-bottom: 120px`
- Между хедером и первой секцией — 0 (hero идёт к краям)
- Footer: `padding-top: 64px; padding-bottom: 48px`

---

## 6. Navigation

### Global Header
- Sticky, фиксированная высота: 64–72px
- Фон: white с `box-shadow: 0 1px 0 #E5E7EB` (hairline border снизу)
- При скролле: усиленная тень (elevation 2)
- Логотип: слева, wordmark "АО Победит"
- Nav-links: горизонтально, uppercase 12–13px, letter-spacing +0.08em, weight 500
- Active state: accent underline (2px, accent color)
- CTA-кнопка: крайний правый, solid-primary
- Никаких mega-menu с декоративными элементами — только чёткие выпадающие списки если нужно

### Footer
- Тёмный фон (Midnight Navy)
- 4-колоночная сетка: Продукция / Компания / Документация / Контакты
- Белый текст, пониженная непрозрачность для secondary
- Подвал: copyright + legal links
- Адрес: Владикавказ, РСО-Алания

---

## 7. Cards

### Каталожные карточки (product/category)
- Фон: white
- Border: 1px solid `#E5E7EB`
- Border-radius: **4px** (строгий, не pill)
- Padding: 24–32px
- Shadow: `0 1px 3px rgba(0,0,0,0.08)` (минимальная)
- Hover: border-color → accent, box-shadow усиливается
- Структура: заголовок → техническое описание → CTA-ссылка
- Никаких иллюстраций или декоративных изображений внутри каталожных карточек

### Информационные карточки (отрасли, преимущества)
- Фон: `#F0F2F5` (Slate 50) или white
- Minimal border или без border
- Иконка (24–32px, line-style, accent color) + заголовок + текст
- Border-radius: 4–6px

### Технические карточки (данные продукта)
- Таблица или structured list
- Mono-spaced figures для чисел
- Hairline borders между строками

---

## 8. CTA Buttons

| Вариант | Фон | Текст | Border | Применение |
|---|---|---|---|---|
| Primary | `#D97706` (Amber) | White | none | Главный призыв (Запросить КП, Смотреть каталог) |
| Secondary | transparent | `#111827` | 1.5px `#111827` | Альтернативный призыв |
| Ghost (dark bg) | transparent | White | 1.5px white | CTA на тёмных секциях |
| Destructive | `#DC2626` | White | none | Только для критических действий |

### Геометрия кнопок
- Border-radius: **3–4px** — строгий прямоугольник, не rounded pill
- Padding: `12px 24px` (medium), `14px 32px` (large, hero CTA)
- Font: 14–16px, weight 600, uppercase или sentence case
- Никаких иконок внутри основных CTA (исключение: стрелка-→ в текстовых ссылках)

---

## 9. Tables & Technical Blocks

### Таблицы данных
- Full-width в контейнере
- Header row: `#F0F2F5` фон, weight 600, uppercase 12px
- Строки: zebra (`#FFFFFF` / `#F5F5F3`)
- Border: `1px solid #E5E7EB` для всех ячеек
- Числа: tabular-nums, right-aligned
- Текст: left-aligned
- Min-width на числовых колонках — без переносов

### Технические блоки (характеристики продукта)
- Definition list или 2-column grid: название параметра / значение
- Параметр: Gray 600, 14px
- Значение: Near Black, 15px, semi-bold
- Моноширинный шрифт для марок, артикулов, ГОСТ-номеров

### Блоки документации
- Иконка типа файла (PDF, DOC) + название + размер + кнопка "Скачать"
- Строчный layout, border-bottom hairline между позициями

---

## 10. Industrial B2B Design Principles (для Stitch prompts)

При генерации каждого нового экрана использовать следующий блок:

```
DESIGN SYSTEM (REQUIRED for АО Победит):
- Typography: Inter or geometric sans-serif. H1: 56px/700. H2: 38px/700. Body: 17px/400.
- Colors: Background #F5F5F3 (light) or #0B1728 (dark). Text #111827. Secondary #6B7280. Accent #D97706 (amber).
- Spacing: 8px grid. Section padding 80px vertical. Container max 1280px, 40px side padding.
- Grid: 12-col, 24px gap. Catalog sections: 3-col equal. Content sections: 8/4 split.
- Cards: white bg, 1px border #E5E7EB, 4px radius, 24–32px padding, minimal shadow.
- CTA buttons: solid amber (#D97706) primary, outline black secondary. 3–4px radius, NOT pill.
- Navigation: sticky 64px header, white bg, hairline border bottom. Logo left, CTA button right.
- Style: industrial corporate B2B — strict, clean, authoritative. NO startup/SaaS vibes. NO gradients. NO decorative blobs. Engineering precision aesthetic.
- Trust elements always visible: 70+ лет / production location / certifications / standards.
```

---

## 11. Что запрещено

- Градиентные mesh-фоны и aurora-эффекты
- Pill-shaped кнопки
- Скруглённые blob-формы как декоративные элементы
- Анимированные particle/geometric backgrounds
- Иконки emoji в контенте
- Stock-photo стиль "улыбающиеся люди в касках"
- Неоновые акценты и glassmorphism
- Декоративные underline-анимации на заголовках
- Шрифты с засечками для основного UI (только для pull-quotes если нужно)
- Любые элементы, ассоциирующиеся с AI-стартапами или tech-компаниями
