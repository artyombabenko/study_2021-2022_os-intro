---
## Front matter
title: "Индивидуальный проект"
subtitle: "6 этап"
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

Размещение двуязычного сайта на Github.

# Ход работы

1. Я cделал поддержку английского и русского языков (рис.1).

![](image/2022-06-04%20(7).png){ width=100% }

*Рис.1. Содержимое файла languages.yaml*

2. Разместил элементы сайта и контент на двух языках (рис.2,3).

![](image/2022-06-04%20(8).png){ width=100% }

*Рис.2. Сайт на русском языке*

![](image/2022-06-04%20(12).png){ width=100% }

*Рис.3. Сайт на английском языке*

3. Сделал пост по прошедшей неделе и пост на тему "Система инициализации Upstart" на двух языках (рис.4,5).

![](image/2022-06-04%20(9).png){ width=100% }

*Рис.2. Посты на русском языке*

![](image/2022-06-04%20(10).png){ width=100% }

*Рис.3. Посты на английском языке*

# Выводы

Я научился делать поддержку двух языков и размещать двуязычный сайт на Github.