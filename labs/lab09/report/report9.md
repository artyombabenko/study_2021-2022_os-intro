---
## Front matter
title: "Лабораторная работа №9"
subtitle: "Текстовой редактор emacs"
author: "Бабенко Артём Сергеевичы"

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

Познакомиться с операционной системой Linux. Получить практические навыки работы с редактором Emacs.

# Теоретическое введение

Буфер — объект, представляющий какой-либо текст. Буфер может содержать что угодно, например, результаты компиляции программы или встроенные подсказки. Практически всё взаимодействие с пользователем, в том числе интерактивное, происходит посредством буферов.

Фрейм соответствует окну в обычном понимании этого слова. Каждый фрейм содержит область вывода и одно или несколько окон Emacs.

Окно — прямоугольная область фрейма, отображающая один из буферов. Каждое окно имеет свою строку состояния, в которой выводится следующая информация: название буфера, его основной режим, изменялся ли текст буфера и как далеко вниз по буферу расположен курсор. Каждый буфер находится только в одном из возможных основных режимов. Существующие основные режимы включают режим Fundamental (наименее специализированный), режим Text, режим Lisp, режим С, режим Texinfo и другие. Под второстепенными режимами понимается список режимов, которые включены в данный момент в буфере выбранного окна.

Область вывода — одна или несколько строк внизу фрейма, в которой Emacs выводит различные сообщения, а также запрашивает подтверждения и дополнительную информацию от пользователя.

Минибуфер используется для ввода дополнительной информации и всегда отображается в области вывода.

Точка вставки — место вставки (удаления) данных в буфере

# Ход работы

1. Установил редактор emacs (рис.1).

![](image/2022-05-20.png){ width=100% }

*Рис.1. Установка редактора emacs*

2. Создал файл lab09.sh, ввёл данный текст и сохранил файл  (рис.2).

![](image/2022-05-20%20(1).png){ width=100% }

*Рис.2. Текст файла*

3. Проделал с текстом стандартные процедуры редактирования (рис.3).

![](image/2022-05-20%20(2).png){ width=100% }

*Рис.3. Текст после всех изменений*

4. Научился использовать команды по перемещению курсора (рис.4).

![](image/2022-05-20%20(3).png){ width=100% }

*Рис.4. Перемещение курсора в начало строки*

5. Научился управлять буферами (рис.5).

![](image/2022-05-20%20(4).png){ width=100% }

*Рис.5. Переключение между буферами*

6. Разделил фрейм на 4 части, в каждом из окон открыл новый файл и написал несколько строк текста (рис.6).

![](image/2022-05-20%20(5).png){ width=100% }

*Рис.6. Управление окнами*

6. Испробовал два режима поиска, научился переключаться между результатами поиска и делать замену (рис.7).

![](image/2022-05-20%20(6).png){ width=100% }

*Рис.7. Переключение между результатами поиска*

# Выводы

Я получил практические навыки работы с редактором Emacs.

# Контрольные вопросы

1. Emacs (редактор макросов) - это семейство текстовых редакторов, которые характеризуются своей расширяемостью. Руководство по наиболее широко используемому варианту, GNU Emacs, описывает его как "расширяемый, настраиваемый, самодокументируемый редактор отображения в реальном времени".

3. Буфер — объект, представляющий какой-либо текст. Окно — прямоугольная область фрейма, отображающая один из буферов.

5. По умолчанию при открытии Emacs создает два буфера — scratch и Messages.

7. C-x 3

8. Для настройки Emacs используется специальный файл, который обычно находится в каталоге пользователя и называется .emacs. В этом файле содержатся выражения на Emacs Lisp, которые устанавливают значения переменных, загружают нужные пакеты и выполняют другие действия.