---
title: Язык разметки Markdown
subtitle: Данный пост является демо-версией. В нём изложена краткая информацию о языке разметки Markdown.
summary: Данный пост является демо-версией. В нём изложена краткая информацию о языке разметки Markdown.
authors:
  - Никита Демидович
tags: []
categories: []
projects: []
date: '2023-04-08T00:00:00Z'
lastMod: '2023-04-08T00:00:00Z'
image:
  caption: ''
  focal_point: ''
---

## Базовые сведения о Markdown

Чтобы создать заголовок, используйте знак #, например:

```# This is heading 1
## This is heading 2
### This is heading 3
#### This is heading 4
```

Чтобы задать для текста полужирное начертание, заключите его в двойные звездочки:

This text is **bold**.

Чтобы задать для текста курсивное начертание, заключите его в одинарные звездочки:

This text is *italic*.

Чтобы задать для текста полужирное и курсивное начертание, заключите его в тройные звездочки:

This is text is both ***bold and italic***.

Упорядоченный список можно отформатировать с помощью соответствующих цифр:

1. First instruction

   1. Sub-instruction

   1. Sub-instruction

1. Second instruction

Неупорядоченный (маркированный) список можно отформатировать с помощью звездочек или тире:

* List item 1
* List item 2
* List item 3

Синтаксис Markdown для встроенной ссылки состоит из части `[link text]`, представляющей текст гиперссылки, и части (file-name.md) – URL-адреса или имени файла, на который дается ссылка:

`[link text](file-name.md)`

или

`[link text](http://example.com/ "Необязательная подсказка")`

Markdown поддерживает как встраивание фрагментов кода в предложение, так и их размещение между предложениями в виде отдельных огражденных блоков. Огражденные блоки кода — это простой способ выделить синтаксис для фрагментов кода. Общий формат огражденных блоков кода:

``` language
your code goes in here
```

## Оформление формул в Markdown

Ниже приведены пример оформления формул:

`$\sin^2 (x) + \cos^2 (x) = 1$` - $\sin^2 (x) + \cos^2 (x) = 1$.
со ссылкой в тексте «Смотри формулу ({-eq. 4.1}).» записывается как:
```$$
\sin^2 (x) + \cos^2 (x) = 1
$$ {#eq:eq1}
```

## Оформление изображений в Markdown

В Markdown вставить изображение в документ можно с помощью непосредственного указания адреса изображения. Синтаксис данной команды выглядит следующим образом:

`![Подпись к рисунку](/путь/к/изображению.jpg "Необязательная подсказка") {#fig:fig1 width="70%"}`

Здесь:

- в квадратных скобках указывается подпись к изображению.

- в круглых скобках указывается URL-адрес или относительный путь изображения, а также (необязательно) всплывающую подсказку, заключённую в двойные или одиночные кавычки.

- в фигурных скобках указывается идентификатор изображения (#fig:fig1) для ссылки на него по тексту и размер изображения относительно ширины страницы (width=90%).

Ссылка на изображение (рис. 4.1) может быть оформлена следующим образом:
`(рис. [-@fig:fig1])`
