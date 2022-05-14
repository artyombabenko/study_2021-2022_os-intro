---
## Front matter
title: "Индивидуальный проект"
subtitle: "3 этап"
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

Добавить к сайту достижения и написать посты.

# Ход работы

1. Я добавил на сайт информацию о своих навыках (рис.1).

![](image/2022-05-14_19-43-24.png){ width=100% }

*Рис.1. Мои навыки*

2. Добавил информацию об опыте (рис.2).

![](image/2022-05-14_19-43-34.png){ width=100% }

*Рис.2. Мой опыт*

3. Добавил информацию о достижениях (рис.3).

![](image/2022-05-14_19-43-37.png){ width=100% }

*Рис.3. Мои дипломы*

4. Написал пост на одну из трёх данных тем по выбору (рис.4).

![](image/2022-05-14_19-43-57.png){ width=100% }

*Рис.4. Пост на тему по выбору*


5. Написал пост о прошедшей неделе (рис.5).

![](image/2022-05-14_19-44-12.png){ width=100% }

*Рис.5. Пост о том, как прошла моя неделя*

6. Ввёл необходимые команды в командной строке, чтобы мои изменения загрузились на GitHub и все могли увидеть обновлённый сайт (рис.6).

![](image/2022-05-14_19-45-37.png){ width=100% }

*Рис.6. Данные обновились*

# Вывод

Я научился добавлять на сайт свои достижения и писать посты на различные темы.