---
## Front matter
title: "Индивидуальный проект"
subtitle: "Этап 2"
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

Добавить к сайту данные о себе и написать посты.

# Ход работы

1. Я разместил свою фотографию на сайте (рис.1).

![](image/2022-05-07.png){ width=100% }

*Рис.1. Добавление фотографии*

2. Я разместил краткое описание себя, добавил информацию о своих интересах и образовании (рис.2).

![](image/2022-05-07%20(1).png){ width=100% }

*Рис.2. Размещение информации о себе*

3. Сделал пост о том, как прошла моя прошлая неделя. Рассказал о своих выполненных делах, оценил свою продуктивность и многое другое (рис.3).

![](image/2022-05-07%20(2).png){ width=100% }

*Рис.3. Пост о прошедшей неделе*

4. Написал и добавил пост на тему "Непрерывная интеграция и непрерывное развертывание (CI/CD)" (рис.4,5).

![](image/2022-05-07%20(3).png){ width=100% }

*Рис.4. Пост на тему по выбору*

![](image/2022-05-07%20(5).png){ width=100% }

*Рис.5. Процесс написания поста*

2. Я запушил и закоммитил папку, для того чтобы мой сайт могли видеть все (рис.6,7).

![](image/2022-05-07%20(6).png){ width=100% }

![](image/2022-05-07%20(7).png){ width=100% }

*Рис.6,7. Использование команд add, push и commit*

# Выводы

Я научился добавлять на сайт данные о себе и писать посты.