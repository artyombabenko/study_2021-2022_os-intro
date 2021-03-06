---
## Front matter
title: "Лабораторная работа №5"
subtitle: "Анализ файловой системы Linux. Команды для работы с файлами и каталогами"
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

Ознакомление с файловой системой Linux, её структурой, именами и содержанием
каталогов. Приобретение практических навыков по применению команд для работы
с файлами и каталогами, по управлению процессами (и работами), по проверке использования диска и обслуживанию файловой системы.

# Теоретическое введение

Для создания текстового файла можно использовать команду touch. Для просмотра файлов небольшого размера можно использовать команду cat. Для просмотра файлов постранично удобнее использовать команду less. Команда head выводит по умолчанию первые 10 строк файла. Команда tail выводит умолчанию 10 последних строк файла. Команда cp используется для копирования файлов и каталогов. Команды mv и mvdir предназначены для перемещения и переименования файлов и каталогов.

Каждый файл или каталог имеет права доступа. Права доступа к файлу или каталогу можно изменить, воспользовавшись командой chmod. Сделать это может владелец файла (или каталога) или пользователь с правами
администратора.

Файловая система в Linux состоит из фалов и каталогов. Каждому физическому носителю соответствует своя файловая система. Для просмотра используемых в операционной системе файловых систем можно воспользоваться командой mount без параметров.

# Ход работы

1. Я выполнил все примеры, приведённые в первой части лабораторной работы(рис.1,2).

![](image/2022-05-05.png){ width=100% }

*Рис.1. Выполнение задания №1. Ввод различных команд*

![](image/2022-05-05%20(1).png){ width=100% }

*Рис.2. Выполнение задания №1. Ввод различных команд (продолжение)*

2. Выполнил задание №2, связанное с созданием, перемещением, копированием и переименованием файлов и каталогов(рис.3).

![](image/2022-05-05%20(6).png){ width=100% }

*Рис.3. Выполнение задания №2.*

3. Создал нужные для задания файлы и директории и с помощью команды chmod присвоил им выделенные права доступа(рис.4).

![](image/2022-05-05%20(2).png){ width=100% }

*Рис.4. Выполнение задания №3.*

4. Далее я проделал приведённые упражнения с помощью известных нам команд(рис.5,6).

![](image/2022-05-05%20(3).png){ width=100% }

*Рис.5. Выполнение задания №4.*

![](image/2022-05-05%20(4).png){ width=100% }

*Рис.6. Выполнение задания №4(продолжение).*

5. Я прочитал man по приведённым командам и кратко их охарактеризовал (рис.7).

![](image/2022-05-05%20(5).png){ width=100% }

*Рис.7. Выполнение задания №5.*

# Контрольные вопросы

1. Ext4 — это результат эволюции Ext3, наиболее популярной файловой системы в Linux. Во многих аспектах Ext4 представляет собой больший шаг вперёд по сравнению с Ext3, чем Ext3 была по отношению к Ext2. Наиболее значительным усовершенствованием Ext3 по сравнению с Ext2 было журналирование, в то время как Ext4 предполагает изменения в важных структурах данных, таких как, например, предназначенных для хранения данных файлов. Это позволило создать файловую систему с более продвинутым дизайном, более производительную и стабильную и с обширным набором функций.

2. Файловая система (ФС) — архитектура хранения данных, которые могут находиться в разделах жесткого диска и ОП. Выдает пользователю доступ к конфигурации ядра. Определяет, какую структуру принимают файлы в каждом из разделов, создает правила для их генерации, а также управляет файлами в соответствии с особенностями каждой конкретной ФС.

ФС Linux — пространство раздела, поделенное на блоки определенного размера. Он определяется кратностью размеру сектора. Соответственно, это могут быть 1024, 2048, 4096 или 8120 байт. Важно помнить, что размер каждого блока известен изначально, ограничен максимальным размером ФС и зависит от требований, которые выдвигает пользователь к каждому из блоков.

Для обмена данными существует сразу два способа. Первый из них — виртуальная файловая система (VFS). С помощью данного типа ФС происходит совместная работа ядра и приложений, установленных в системе. VFS позволяет пользователю работать, не учитывая особенности каждой конкретной ФС. Второй способ — драйверы файловых систем. Именно они отвечают за связь между «железом» и софтом.

3. Монтирование тома.

4. Отсутствие синхронизации между образом файловой системы в памяти и ее данными на диске в случае аварийного останова может привести к появлению следующих ошибок:

1) Один блок адресуется несколькими mode (принадлежит нескольким файлам).

2) Блок помечен как свободный, но в то же время занят (на него ссылается onode).

3) Блок помечен как занятый, но в то же время свободен (ни один inode на него не ссылается).

4) Неправильное число ссылок в inode (недостаток или избыток ссылающихся записей в каталогах).

5) Несовпадение между размером файла и суммарным размером адресуемых inode блоков.

6) Недопустимые адресуемые блоки (например, расположенные за пределами файловой системы).

7) "Потерянные" файлы (правильные inode, на которые не ссылаются записи каталогов).

8) Недопустимые или неразмещенные номера inode в записях каталогов.

5. mkfs - позволяет создать файловую систему Linux.

6. Cat - выводит содержимое файла на стандартное устройство вывода.

7. Cp – копирует или перемещает директорию, файлы.

8. Mv - переименовать или переместить файл или директорию.

9. Права доступа к файлу или каталогу можно изменить, воспользовавшись командой chmod. Сделать это может владелец файла (или каталога) или пользователь с правами администратора.

# Вывод

Я ознакомился с файловой системой Linux, её структурой, именами и содержанием каталогов, а также я приобрёл практические навыки по применению команд для работы с файлами и каталогами, по управлению процессами (и работами), по проверке использования диска и обслуживанию файловой системы.