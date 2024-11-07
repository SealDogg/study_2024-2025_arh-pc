---
## Front matter
title: "Отчёт по лабораторной работе №5"
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

Приобрести практические навыки по работе с Midnight Commander, а также освоить инструкции mov и int

# Выполнение лабораторной работы

1.	Открываем Midnight Commander.

![Окно Midnight Commander](image/pic1.png)

2. 	Переходим в каталог ~/work/arch-pc.

![Каталог ~/work/arch-pc](image/pic2.png)

3.  Создаём каталог lab05.

![Создание каталога lab05](image/pic3.png)

4.  Создаём файл lab5-1.asm.

![Созданный файл lab5-1.asm](image/pic4.png)

5.  Открываем lab5-1.asm с помощью встроенного редактора.

![Открытый файл lab5-1.asm](image/pic5.png)

6.  Вводим текст программы.

![Готовый файл lab5-1.asm](image/pic6.png)

7.  Просматриваем ещё раз файл.

![Просмотр файла](image/pic7.png)

8.  Транслируем и компонуем объектный файл, запускаем и вводим ФИО.

![Трансляция, компоновка, выполнение](image/pic8.png)

9.  Скачиваем файл in_out.asm и копируем его в наш каталог.

![Копирование](image/pic9.png)

10. Создаём копию файла lab5-1.asm.

![Создание копии](image/pic10.png)

11. Вводим текст в lab5-2.asm.

![Готовый файл lab5-2.asm](image/pic11.png)

12. Транслируем, компонуем, запускаем lab5-2.asm.

![Трансляция, компоновка, выполнение](image/pic12.png)

13. Меняем sprintLF на sprint и смотрим на результат.

![Теперь в одну строку](image/pic13.png)

# Выполнение самостоятельной работы

1.  Копируем lab5-1.asm с новым названием lab5-3.asm.

![Копирование lab5-1.asm](image/pic14.png)

2.  Изменяем программу под заданные условия и тестируем.

![Трансляция, компоновка, запуск](image/pic15.png)

![Текст lab5-3.asm](image/pic16.png)

3.  Копируем lab5-2.asm с новым названием lab5-4.asm.

![Копирование lab5-2.asm](image/pic17.png)

4.  Тестируем.

![Выполнение программы](image/pic19.png)

![Текст lab5-4.asm](image/pic18.png)


# Выводы

Был освоен mc, а также были отработаны инструкции ассемблера mov и int.

