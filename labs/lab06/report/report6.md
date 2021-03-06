---
## Front matter
title: "Лабораторная работа № 6"
subtitle: "Поиск файлов. Перенаправление ввода-вывода. Просмотр запущенных процессов"
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

Ознакомление с инструментами поиска файлов и фильтрации текстовых данных. Приобретение практических навыков: по управлению процессами (и заданиями), по проверке использования диска и обслуживанию файловых систем.

# Теоретическое введение

Команда find используется для поиска и отображения на экран имён файлов, соответствующих заданной строке символов. Найти в текстовом файле указанную строку символов позволяет команда grep. Команда df показывает размер каждого смонтированного раздела диска. Любую выполняющуюся в консоли команду или внешнюю программу можно запустить
в фоновом режиме. Для этого следует в конце имени команды указать знак амперсанда &. Команда ps используется для получения информации о процессах.

Любой команде, выполняемой в системе, присваивается идентификатор процесса (process ID). Получить информацию о процессе и управлять им, пользуясь идентификатором процесса, можно из любого окна командного интерпретатора.

# Ход работы

1. Я осуществил вход в систему, открыл Terminal. При помощи команды ls -a я записал в файл file.txt названия файлов, содержащихся в каталоге /etc. Дописал в этот же файл названия файлов, содержащихся в моём домашнем каталоге(рис.1).

![](image/2022-05-07%20(9).png){ width=100% }

*Рис.1. Выполнение задания №2*

2. Я вывел имена всех файлов из file.txt, имеющих расширение .conf, после чего записал их в новый текстовой файл conf.txt (рис.2).

![](image/2022-05-07%20(8).png){ width=100% }

*Рис.2. Выполнение задания №3.*

3. Определил, какие файлы в моём домашнем каталоге имеют имена, начинавшиеся с символа c (рис.3).

![](image/2022-05-07%20(10).png){ width=100% }

*Рис.3. Выполнение задания №4.*

4. Вывел на экран (по странично) имена файлов из каталога /etc, начинающиеся с символа h (рис.4).

![](image/2022-05-07%20(11).png){ width=100% }

*Рис.4. Выполнение задания №5.*

5. Запустил в фоновом режиме процесс, который будет записывать в файл ~/logfile файлы, имена которых начинаются с log.

![](image/2022-05-07%20(13).png){ width=100% }

*Рис.5. Выполнение задания №6.*

6. С помощью команды rm я удалил файл ~/logfile (рис.6).

![](image/2022-05-07%20(14).png){ width=100% }

*Рис.6. Выполнение задания №7.*

7. Запустил из консоли в фоновом режиме редактор gedit. Определил идентификатор процесса gedit, используя команду ps, конвейер и фильтр
grep (рис.7).

![](image/2022-05-07%20(15).png){ width=100% }

*Рис.7. Выполнение заданий №8 и №9.*

8. Я выполнил команды df и du, предварительно получив более подробную информацию об этих командах, с помощью команды man (рис.8).

![](image/2022-05-07%20(16).png){ width=100% }

*Рис.8. Выполнение задания №11.*

9. Воспользовавшись справкой команды find, я вывел имена всех директорий, имеющихся в моём домашнем каталоге (рис.9).

![](image/2022-05-07%20(17).png){ width=100% }

*Рис.9. Выполнение задания №12.*

# Контрольные вопросы

1. Standard input, standard output, standard error. 

2. ">" - открыть файл на перезапись, ">>" - на дозапись.

3. Конвейер - направление вывода на вход для следующей команды.

8. Команда find используется для поиска и отображения на экран имён файлов, соответствующих заданной строке символов.

9. Да, можно воспользоваться командой grep.

10. Команда df.

11. Команда du

12. Команда kill.св 

# Вывод

Я ознакомился с инструментами поиска файлов и фильтрации текстовых данных, приобрёл практические навыки: по управлению процессами (и заданиями), по проверке использования диска и обслуживанию файловых систем.