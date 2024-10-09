---
## Front matter
title: "Отчёт по лабораторной работе №3"
author: "Ярослав Антонович Меркулов"

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
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
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
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Научится работать с языком разметки Markdown и оптимизировать написание отчётов по лабораторным работам.

# Выполнение лабораторной работы

1.	Переходим в каталог курса и обновляем локальный репозиторий командой *git pull*.

![Результат обновления репозитория](image/pic1.png)

2. 	Переходим в каталог с шаблоном отчёта по лабораторной работе и создаём .docx и .pdf с помощью команды *make*.

![Создание файлов с помощью *make*](image/pic2.png)

3.  Удаляем созданные файлы командой *make clean*.

![Удаление созданных файлов с помощью команды *make clean*](image/pic3.png)

4.  Открываем с помощью *gedit* файл *report.md* и ознакамливаемся с содержанием.

![Открытый файл *report.md*](image/pic4.png)

# Выводы

Были получены навыки работы с языком разметки Markdown, созданы отчёты по шаблону.

