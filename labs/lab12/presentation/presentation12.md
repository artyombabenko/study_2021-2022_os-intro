---
## Front matter
lang: ru-RU
title: Лабораторная работа №12. Программирование в командном процессоре ОС UNIX. Расширенное программирование
author: |
	Бабенко Артём Сергеевич, НФИбд-01-21
institute: |
	RUDN University, Moscow, Russian Federation
	
date: 27.05.22

## Formatting
toc: false
slide_level: 2
theme: metropolis
header-includes: 
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
aspectratio: 43
section-titles: true
---

# Цель работы

Изучить основы программирования в оболочке ОС UNIX. Научиться писать более сложные командные файлы с использованием логических управляющих конструкций и циклов.

# Ход работы

1. Написал командный файл, реализующий упрощённый механизм семафоров. Командный файл должен в течение некоторого времени t1 дожидаться освобождения ресурса, выдавая об этом сообщение, а дождавшись его освобождения, использовать его в течение некоторого времени t2<>t1, также выдавая информацию о том, что ресурс используется соответствующим командным файлом (процессом).

![](image/2022-05-27%20(10).png){ width=100% }

*Рис.1. Листинг № 1*

# Ход работы

![](image/2022-05-27%20(13).png){ width=100% }

*Рис.2. Результат выполнения программы*

# Ход работы

2. Реализовал команду man с помощью командного файла. Изучил содержимое каталога /usr/share/man/man1. В нем находятся архивы текстовых файлов, содержащих
справку по большинству установленных в системе программ и команд. Командный
файл должен получать в виде аргумента командной строки название команды и в виде
результата выдавать справку об этой команде или сообщение об отсутствии справки,
если соответствующего файла нет в каталоге man1.

![](image/2022-05-27%20(14).png){ width=100% }

*Рис.3. Листинг № 2*

# Ход работы

![](image/2022-05-27%20(15).png){ width=100% }

*Рис.4. Результат выполнения программы*

# Ход работы

3. Используя встроенную переменную $RANDOM, написал командный файл, генерирующий случайную последовательность букв латинского алфавита.

![](image/2022-05-27%20(16).png){ width=100% }

*Рис.5. Листинг № 3*

# Ход работы

![](image/2022-05-27%20(17).png){ width=100% }

*Рис.6. Результат выполнения программы*

# Вывод

Я изучил основы программирования в оболочке ОС UNIX. Научился писать более сложные командные файлы с использованием логических управляющих конструкций и циклов.
