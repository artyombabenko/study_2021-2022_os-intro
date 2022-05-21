---
## Front matter
title: "Индивидуальный проект"
subtitle: "4 этап"
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

Добавить к сайту ссылки на научные и библиометрические ресурсы. Написать посты на различные темы.

# Ход работы

1. Я добавил ссылки на свои аккаунты в веб-сервисах и видеохостингах (рис.1,2).

![](image/2022-05-21%20(1).png){ width=100% }

![](image/2022-05-21%20(3).png){ width=100% }

*Рис.1,2. Прикрепление ссылок на свои аккаунты *

2. Написал пост по прошедшей неделе (рис.3).

![](image/2022-05-21%20(5).png){ width=100% }

*Рис.3. Пост о прошедшей неделе*

3. Написал пост на тему по выбору (рис.4).

![](image/2022-05-21%20(6).png){ width=100% }

*Рис.4. Пост на тему "Создание презентаций"*

# Вывод

Я добавил к сайту ссылки на научные и библиометрические ресурсы, написал пост о прошедшей неделе и пост на тему по выбору.
