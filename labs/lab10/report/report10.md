---
## Front matter
title: "Отчёт по лабораторной работе №10"
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

Приобрести навыки написания программ для работы с файлами.

# Выполнение лабораторной работы

1.  Создаём каталог для лабораторной работы, переходим в него и создаём файл lab10-1.asm и ещё 2 текстовых файла.

![Создание каталога, переход в него, создание файла](image/pic1.png){width=70%}

2.  Вводим текст программы из листинга 10.1.

![Введённый текст программы](image/pic2.png){width=70%}

3.  Создаём исполняемый файл и тестируем.

![Работа программы](image/pic3.png){width=70%}

4.  Изменяем права доступа. При попытке запустить файл видим ошибку.

![Запуск файла с измененными правами доступа](image/pic5.png){width=70%}

5.  Изменяем права доступа к файлу lab10-1.asm. Программа не может запуститься, т.к. тип файла не распознан.

![Попытка запуска lab10-1.asm](image/pic6.png){width=70%}

6.  Меняем права доступа в соответствии с таблицей (14 вариант).

![Изменение прав доступа и проверка](image/pic7.png){width=70%}

## Выполнение самостоятельной работы

![Текст программы](image/pic8.png){width=70%}

![Работа программы](image/pic9.png){width=70%}

# Выводы

Были освоены навыки написания программ с использованием файлов.

