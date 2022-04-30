---
## Front matter
title: "Лабораторная работа №3"
subtitle: "Markdown"
author: "Бабенко Артём Сергеевич"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Научиться оформлять отчёты с помощью легковесного языка разметки Markdown.

# Задание

– Сделайте отчёт по предыдущей лабораторной работе в формате Markdown.

– В качестве отчёта просьба предоставить отчёты в 3 форматах: pdf, docx и md (в архиве,
поскольку он должен содержать скриншоты, Makefile и т.д.)

# Теоретическое введение

Markdown — это облегченный язык разметки с синтаксисом форматирования обычного текста. Документация поддерживает разметку Markdown в соответствии с CommonMark и ее синтаксический анализ через подсистему Markdig. Документация также поддерживает пользовательские расширения Markdown, которые предоставляют более обширный контент на сайте документации.

Для записи Markdown можно использовать любой текстовый редактор, но мы рекомендуем Visual Studio Code с расширением Docs Authoring Pack. Расширение Docs Authoring Pack содержит средства редактирования и функции предварительного просмотра, позволяющие увидеть, как будут выглядеть статьи на сайте Документации.

# Ход работы

1. Открываю шаблон отчёта и пишу название лабораторной работы, своё ФИО, цель работы, теоретическое введение, выводы и контрольные вопросы.

![](image/7.png){ width=100% }

*Рис.1. Заполнение разделов*

2. Описываю ход работы: записываю этапы и прикрепляю скриншоты.

![](image/8.png){ width=100% }

*Рис.2. Описание хода работы*

3. Конвертирую получившийся отчёт в pdf и docx и проверяю, нет ли каких-то недочётов или ошибок.

![](image/9.png){ width=100% }

*Рис.3. Конвертация отчёта в pdf и docx*

# Выводы

Я Научился оформлять отчёты с помощью легковесного языка разметки Markdown и испоьзовать pandoc для конвертации md в pdf и docx.

# Контрольные вопросы

В данной лабораторной работе нет контрольных вопросов.