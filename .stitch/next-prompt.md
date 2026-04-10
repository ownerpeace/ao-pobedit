---
page: product-vk6
prev: sitemap
---

Design a **Product Detail Page** for a specific hard alloy grade (`/products/hard-alloys/vk6`) — using ВК6 (VK6) as the example. This page is a technical datasheet + commercial page for procurement engineers deciding whether to order this specific material.

ВК6 is one of the most popular "universal" hard alloys at АО «Победит» — suitable for cutting tools, wear-resistant applications, and some drilling applications. The page should sell the material through **specifications, not marketing copy**.

**DESIGN SYSTEM (REQUIRED — same as all previous pages):**
- Typography: Inter. H1: 40px/700. H2: 24px/700. Body: 16px/400.
- Colors: Background #F5F5F3. Text #111827. Secondary #6B7280. Accent #D97706 (amber).
- Spacing: 8px grid. Section padding 80px vertical. Container max 1280px, 40px side padding.
- Cards: white bg, 1px border #E5E7EB, 4px radius.
- Buttons: solid amber primary, outline black secondary. 3–4px radius, NOT pill.
- Navigation: sticky 64px header. Logo left, CTA right.
- Style: industrial B2B — structured, data-dense, zero decoration.

**PAGE STRUCTURE:**

1. **Sticky Navigation** — same as all pages

2. **Page Header (compact)**
   - Breadcrumb: Главная / Продукция / Твёрдые сплавы / ВК6
   - H1: "ВК6" (or "Твёрдый сплав ВК6")
   - Subtitle: Brief 1-line description — "универсальный вольфрамокобальтовый сплав для режущего инструмента и абразивных процессов"

3. **Quick specs banner (2-column or 4-column grid — critical facts)**
   - Группа: Вольфрамовые (ВК)
   - Состав: WC + Co (тут % если есть, или "состав см. в документах")
   - Твёрдость (HRA): 20–22
   - Плотность (г/см³): 14.9–15.1
   - "Скачать паспорт" button (primary amber)

4. **Description section (2-column)**
   Left: H2 "Описание" + paragraph(s) about the grade
   - When/why to use ВК6
   - Primary industries (режущий инструмент, мерные изделия, абразивные процессы)
   - Advantages over other grades
   
   Right: "Аналоги и эквиваленты" block
   - ISO standard equivalent (if known)
   - Similar grades from other suppliers (if competitive info exists)
   - "Запросить информацию о замене" link

5. **Specifications table**
   - Mechanical properties: твёрдость, TRS, density, grain size
   - Chemical composition: W, Co, total
   - "Полная таблица свойств" expandable or link to PDF

6. **Applications block (3-4 use cases)**
   - Иконка или просто H3 + short description
   - E.g.: "Резцы токарные", "Фрезы концевые", "Сверла спираль", "Пластины для оснащения инструмента"
   - Short 1–2 sentence per application

7. **Available formats / Stock status**
   - Доступные формы: "Пластины напаиваемые (ГОСТ 25395-90)", "Пластины сменные", "Спецформы на заказ"
   - "Посмотреть остатки на складе" → link to `/products/remainders` with filter
   - "В наличии: есть" (if known) or link to sales

8. **Documents & certifications**
   - ГОСТ, паспорт качества, сертификат соответствия
   - "Все документы" button → `/quality` or `/document`

9. **Related products**
   - "Похожие марки сплавов" — grid with 3–4 related grades (ВК3, ВК8, ВК10КС, Т5К10)
   - Each card: grade name, brief use case, "→" link

10. **CTA block (convert to customer)**
    - "Запросить КП на ВК6" (amber) → `/rfq` with prefilled grade
    - "Связаться с отделом продаж" (outline) → `/contacts`

11. **Footer** — same as all pages. No CTA band.

**CONTENT NOTES (ВК6 specifics):**
- Состав: ~94% WC (карбид вольфрама), ~6% Co (кобальт)
- Твёрдость: HRA 20–22 (или примерно такая в зависимости от источника)
- Плотность: ~15 г/см³
- Применение: режущий инструмент, абразивные процессы, дереворежущий инструмент, мерные изделия
- Преимущество над ВК3: более вязкий; над ВК8: более твёрдый

If you don't know exact specs, use plausible industry values for WC/Co hard alloys in this grade class.

**DESIGN NOTES:**
- This is **not a marketing page** — every number and claim must feel factual and verifiable
- Specs table should dominate the page, not description text
- Links to other grades should help users compare, not upsell
- "Скачать" and "Запросить" buttons are the conversion tools — make them visible
- No stock photos, no "happy factory workers" — datasheet + contact form
