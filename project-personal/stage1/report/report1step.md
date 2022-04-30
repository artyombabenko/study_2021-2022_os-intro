---
## Front matter
title: "Индивидуальный проект"
subtitle: "Этап 1"
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

Разместить на Github Pages заготовку для персонального сайта.

# Ход работы

1. Я установил hugo и добавил его в PATH (рис.1).

![](image/2022-04-30%20(10).png){ width=100% }

*Рис.1. Проверка версии hugo*

2. Захожу на гитхаб и нажимаю "Использовать этот шаблон"(рис.2)

![](image/2022-04-30%20(11).png){ width=100% }

*Рис.2. Использовать этот шаблон*

3. Создаю репозитории и даю им имена mysite и artyombabenko.github.io (рис.3).

![](image/2022-04-30%20(12).png){ width=100% }

*Рис.3. Создание одного из репозиториев*

4. Клонирую репозиторий с шаблоном (рис.4).

![](image/2022-04-30%20(13).png){ width=100% }

*Клонирование репозитория с шаблоном*

5. Делаю коммит и загружаю на сервер (рис.5)

![](image/2022-04-30%20(15).png){ width=100% }

*Рис.5. Коммит и загрузка на сервер*

6. С помощью команды hugo собираю сайт

![](image/2022-04-30%20(16).png){ width=100% }

*Рис.6. Сборка сайта*

7. В папке public появилось много файлов для моего сайта (рис.7).

![](image/2022-04-30%20(18).png){ width=100% }

*Рис.7. Наличие большого количества файлов сборки*

8. Загружаю всё это на сервер (рис.8).

![](image/2022-04-30%20(19).png){ width=100% }

*Рис.8. Загрузка файлов сборки на сервер*

9. Захожу на получившийся недоделанный сайт - https://artyombabenko.github.io/ - и просматриваю его. Заготовка сайта готова (рис.9).

![](image/2022-04-30%20(20).png){ width=100% }

*Рис.8. Получившаяся версия сайта. Конец первого этапа*

# Выводы

Я научился размещать на Github Pages заготовку (шаблон hugo) для персонального сайта.


