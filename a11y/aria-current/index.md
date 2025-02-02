---
title: "`aria-current`"
description: "ARIA-атрибут для того, чтобы рассказать пользователям вспомогательных технологий о текущем, выбранном элементе."
authors:
  - doka-dog
keywords:
  - доступность
  - ARIA
  - ARIA-атрибут
related:
  - a11y/aria-intro
  - a11y/aria-attrs
  - a11y/aria-activedescendant
tags:
  - doka
  - placeholder
---

## Кратко

[Состояние виджета](/a11y/aria-attrs/#atributy-vidzhetov) из [WAI-ARIA](/a11y/aria-intro/#specifikaciya). Означает, что пользователь сейчас находится на определённом элементе из группы других.

## Пример

```html
<nav aria-label="Хлебные крошки">
  <ul>
    <li>
      <a href="../../../">Породы собак</a>
    </li>
    <li>
      <a href="../../">Ирландские породы</a>
    </li>
    <li>
      <a href="./" aria-current="page">Ирландский волкодав</a>
    </li>
  </ul>
</nav>
```

## Как пишется

Добавьте к тегу атрибут `aria-current` с одним из значений:

- `page` — текущая страница из нескольких.
- `step` — текущий шаг из нескольких.
- `location` — текущее положение на странице, экране или в контексте выполнения какого-то действия.
- `date` — текущая дата из календаря.
- `time` — текущее время из расписания.
- `true` — текущий элемент из группы других.
- `false` (по умолчанию) — этот элемент из группы сейчас не текущий.

Атрибут можно использовать для всех тегов и [ролей](/a11y/aria-roles/).

## Как понять

На сайтах часто встречаются хлебные крошки, пагинация и большие формы, которые делятся на несколько шагов. Выбранная страница или шаг обычно визуально выделяются цветом или по-другому. `aria-current` работает так же. Атрибут сообщает пользователям вспомогательных технологий какая ссылка из хлебных крошек выбрана или на каком шаге они находятся.
