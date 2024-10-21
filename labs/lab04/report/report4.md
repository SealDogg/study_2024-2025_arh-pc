---
## Front matter
title: "Отчёт по лабораторной работе №4"
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

Научится компилировать и собирать программы, написанные на ассемблере NASM

# Выполнение лабораторной работы

1.	Создаём каталог для работы с программами на языке ассемблера NASM.

![Создание каталога для работы](image/pic1.png)

2. 	Создаём текстовый файл с именем *hello.asm*.

![Создание файла с помощью *touch*](image/pic2.png)

3.  Открываем созданный файл с помощью *gedit*.

![Открытый файл *hello.asm*](image/pic3.png)

4.  Вводим заданный текст.

![Готовый текстовый файл](image/pic4.png)

5.  Выполняем трансляцию с помощью *nasm*.

![Объектный файл](image/pic5.png)

6.  Снова выполняем трансляцию, но с другими параметрами.

![Объектный файл и файл листинга](image/pic6.png)

7.  Переходим к компоновке. Используем *ld*.

![Готовый исполняемый файл](image/pic7.png)

8.  Используем компоновку с другими параметрами. Получаем исполняемый файл с другим названием.

![Другой исполняемый файл](image/pic8.png)

9.  Запускаем файл.

![./hello и вывод](image/pic9.png)

# Выполнение самостоятельной работы

1.  Копируем *hello.asm* и переименовываем в *lab04.asm*.

![Копирование *hello.asm*](image/pic10.png)

2.  Открываем с помощью *gedit* файл *lab04.asm*. Меняем *Hello world!* на *Меркулов Ярослав*.

![Файл *lab04.asm*](image/pic11.png)

3.  Оттранслируем и скомпонуем файл.

![Трансляция и компоновка](image/pic12.png)

4.  Запускаем получившийся файл.

![Работа программы](image/pic13.png)

5.  Копируем текстовые файлы в локальный репозиторий.

![Копирование файлов](image/pic14.png)

6.  Проверяем наличие файлов.

![Проверка наличия файлов](image/pic15.png)

7.  Загружаем всё на *Github*.

![Загрузка на *Git*](image/pic16.png)

# Выводы

Были получены знания и умения по работе с NASM (компиляции и сборки).

