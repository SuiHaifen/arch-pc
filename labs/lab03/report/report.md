---
## Front matter
title: "Отчёт по лабораторной работе 3"
subtitle: "Архитектура компьютеров"
author: "Сюй Хайфэн"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
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

Овладевание процессом оформления отчетов с использованием простого языка разметки Markdown.

# Ход работы

Установил программы pandoc и TexLive по указаниям в лабораторной работе. 

Открыл терминал.

Перешел в каталог курса, который был сформирован при выполнении лабораторной работы №3. Обновил локальный репозиторий, скачав изменения из удаленного репозитория.

Перешел в каталог с шаблоном отчета по лабораторной работе №3. (рис. [-@fig:001])

![Каталог с шаблоном отчета](image/01.png){ #fig:001 width=70%, height=70% }

Выполнил компиляцию шаблона с использованием Makefile. 
Для этого ввел команду make. (рис. [-@fig:002])
После успешной компиляции были сгенерированы файлы report.pdf и report.docx. 
Открыл и проверил корректность полученных файлов. (рис. [-@fig:003])

![Использую Makefile](image/02.png){ #fig:002 width=70%, height=70% }

![экспортированные файлы](image/03.png){ #fig:003 width=70%, height=70% }

Удалил полученные файлы с использованием Makefile. 
Для этого ввел команду make clean. (рис. [-@fig:004])
Проверил, что после выполнения этой команды файлы report.pdf и report.docx были удалены.

![Удалены docx и pdf](image/04.png){ #fig:004 width=70%, height=70% }

Открыл файл report.md с помощью текстового редактора gedit. 
Внимательно изучил структуру этого файла. 
(рис. [-@fig:005])

![Шаблон отчета ](image/05.png){ #fig:005 width=70%, height=70% }

Заполнил отчет и скомпилировал его с использованием Makefile. 
Проверил корректность полученных файлов. 
(рис. [-@fig:006])

![Заполнил отчет ](image/06.png){ #fig:006 width=70%, height=70% }

Сделал самостоятельное задание.
Заполнил отчет в формате Markdown для лабораторной номер 2.
(рис. [-@fig:007], рис. [-@fig:008])

![Заполнил отчет ](image/07.png){ #fig:007 width=70%, height=70% }

![Компиляция отчета](image/08.png){ #fig:008 width=70%, height=70% }

Загрузил файлы на Github.

# Выводы

В ходе работы мы изучили синтаксис языка разметки Markdown и научились создавать структурированные отчеты с его помощью.