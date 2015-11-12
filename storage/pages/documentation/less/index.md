---
title: LESS  
description: На этой странице предоставлено описание LESS-файлов и CSS-стилей, используемых в Bitrix Quick Start
template: index

---

# Организация LESS-кода

<a href="https://github.com/pafnuty/bqs-site/blob/dev/content/documentation/less/index.md" class="btn btn-mini" target="_blank">Редактировать страницу</a>
</div>

### Навигация по компонентам
- [Переменные](/documentation/less/variables)
- [Миксины](/documentation/less/mixins)
- [Сетка](/documentation/less/grid)
- [Типографика](/documentation/less/typography)
- [UI (кнопки, формы)](/documentation/less/ui)
- [Таблицы](/documentation/less/tables)
- [Helpers](/documentation/less/helpers)

### Структура и предназначение LESS-файлов в проекте

Имя файла **следует начинать с двухзначной цифры**, после которой идёт тире и пояснительное название файла, понятное для человека.
Это даёт возможность нормального восприятия структуры файлов и приводит структуру проектов в общий порядок.

- **00-09** — файлы, которые не попадают в результирующий CSS (миксины, переменные и т.д.).
- **10-19** — файлы, которые обязательно должны присутствовать, задают костяк шаблона (сетка, кнопки, иконки, формы и т.д.) и оформляют стандартные элементы html.
- **20-79** — различные дополнительные файлы, отвечающие за оформление конкретных кусков вёрстки (меню, модальные окна, слайдеры, хлебные крошки, каталог и т.д.)
- **80-main.less** - основной файл стилей сайта, сюда как правило пишется всё, что относится к конкретному сайту, это уникальный для каждого проекта файл, если куски кода кочуют в этом файле из проекта в проект - значит надо выносить их в отдельный файлы в пределах имён 20-79.
- **90-helpes.less** — Различные хелперы и прочие стили, подгрузка которых должна происходить после основных.
- **template_styles.less** — сюда импортируются необходимые файлы и имено он компилится в одноименный CSS-файл. 

*При разработке допускается совпадение чисел в наименовани файлов.*



