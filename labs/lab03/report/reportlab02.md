---
## Front matter
title: "Лабораторная работа №2"
subtitle: "Управление версиями"
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

Изучить идеологию и применение средств контроля версий. Освоить умения по работе с git.

# Теоретическое введение

Markdown — это облегченный язык разметки с синтаксисом форматирования обычного текста. Документация поддерживает разметку Markdown в соответствии с CommonMark и ее синтаксический анализ через подсистему Markdig. Документация также поддерживает пользовательские расширения Markdown, которые предоставляют более обширный контент на сайте документации.

Для записи Markdown можно использовать любой текстовый редактор, но мы рекомендуем Visual Studio Code с расширением Docs Authoring Pack. Расширение Docs Authoring Pack содержит средства редактирования и функции предварительного просмотра, позволяющие увидеть, как будут выглядеть статьи на сайте Документации.

# Выполнение лабораторной работы

1. Устанавливаю git-flow в Fedora Linux (рис.1).

![](image/1.png){ width=100% }

*Рис.1. Установка git-flow*
 
2. Делаю базовую настройку git (рис.2).

![](image/2.png){ width=100% }

*Рис.2. Настройка git*

3. Создаю ключ SSH (рис.3.)

![](image/3.png){ width=100% }

*Рис.3. Создание SSH ключа*

4.	Создаю ключ PGP (рис.4).

![](image/4.png){ width=100% }

*Рис.4. Создание PGP ключа.*

5.	Настраиваю подписи git (рис.5.)

![](image/5.png){ width=100% }

*Рис.5. Настройка автоматических подписей коммитов git*

6. Создаю локальный каталог для выполнения заданий по предмету (рис.6.).

![](image/6.png){ width=100% }

*Рис.6. Создание каталога*

# Выводы

Я изучил идеологию и применение средства контроля версий, а также освоил умения по работе с git.

# Контрольные вопросы

1. Система контроля версий (Version Control System, VCS) — программное обеспечение для облегчения работы с изменяющейся информацией. u VCS позволяет хранить несколько версий одного и того же документа, при необходимости возвращаться к более ранним версиям, определять, кто и когда сделал то или иное изменение, и многое другое.
6. У Git две основных задачи: первая — хранить информацию о всех изменениях в вашем коде, начиная с самой первой строчки, а вторая — обеспечение удобства командной работы над кодом.
9. Ветки нужны, чтобы несколько программистов могли вести работу над одним и тем же проектом или даже файлом одновременно, при этом не мешая друг другу. Кроме того, ветки используются для тестирования экспериментальных функций: чтобы не повредить основному проекту, создается новая ветка специально для экспериментов.