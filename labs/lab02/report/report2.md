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

Получить и закрепить практические навыки по работе со средствами контроля 
версий на примере git, а также изучить идеологию и применение.

# Выполнение лабораторной работы

1.  Создаём учётную запись на github.

![Готовая учётная запись github](image/pic1.png)

2.  Задаём имя пользователя и электронную почту для git.

![Настройка имени пользователя и email](image/pic2.png)

3.  Задаём оставшиеся параметры.

![Настройка параметров git](image/pic3.png)

4.  Создаём SSH ключ.

![Создание SSH ключа](image/pic4.png)

5.  Копируем созданный ключ.

![Копирование ключа с помощью команды](image/pic5.png)

![Добавление ключа на Github](image/pic6.png)

6.  Создаём каталог для предмета «Архитектура компьютера».

![Создание каталога](image/pic7.png)

7.  Создаём репозиторий на основе шаблона.

![Создание репозитория из шаблона](image/pic8.png)

8.  Переходим в каталог курса.

![Переход в каталог курса](image/pic9.png)

9.  Клонируем созданный репозиторий в каталог.

![Клонирование репозитория](image/pic10.png)

10. Переходим в каталог курса и удаляем лишние файлы.

![Работа с каталогом](image/pic11.png)

11. Создаём необходимые каталоги.

![Создание каталогов](image/pic12.png)

12. Отправляем файлы на сервер.

![Отправка файлов на сервер (1)](image/pic13.png)

![Отправка файлов на сервер (2)](image/pic14.png)

13. Проверяем правильность создания иерархии.

![Локальный репозиторий и репозиторйи Github](image/pic15.png)

# Выполнение задания для самостоятельной работы

1.  Копируем отчёты по первой и второй лабораторной работе.

![Копирование файлов отчётов](image/pic16.png)

2.  Подгружаем в репозиторий.

![Синхронизация файлов](image/pic17.png)

# Выводы

Мы научились пользоваться средствами контроля версий (git), 
отработали команды, создали собственный репозиторий на GitHub для хранения 
отчётов по лабораторным работам.

