---
## Front matter
title: "Отчёт по лабораторной работе №9"
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

Приобрести навыки написания программ с использованием подпрограмм. Ознакомиться с методами отладки при помощи GDB.

# Выполнение лабораторной работы

## Реализация подпрограмм в NASM

1.  Создаём каталог для лабораторной работы, переходим в него и создаём файл lab09-1.asm.

![Создание каталога, переход в него, создание файла](image/pic1.png){width=70%}

2.  Вводим текст программы из листинга 9.1.

![Введённый текст программы](image/pic2.png){width=70%}

3.  Создаём исполняемый файл и тестируем.

![Работа программы](image/pic3.png){width=70%}

4. Изменяем текст программы, создаём подпрограмму _subcalcul.

![Изменённый файл](image/pic37.png){width=70%}

![Работа новой программы](image/pic4.png){width=70%}

## Отладка программам с помощью GDB

5.  Создаём файл lab09-2.asm.

![Создание файла](image/pic5.png){width=70%}

6.  Записываем в файл листинг.

![Lab09-2.asm](image/pic6.png){width=70%}

7.  Получаем исполняемый файл.

![Компиляция и трансляция с параметрами](image/pic7.png){width=70%}

8. Запускаем отладчик, запускаем в нём программу.

![Отладчик](image/pic8.png){width=70%}

9. Ставим breakpoint на _start.

![Брейкпоинт](image/pic9.png){width=70%}

10. Смотрим дисассимилированный код программы, переключаем отображение.

![Дисассимилированный код](image/pic10.png){width=70%}

11. Включаем режим псевдографики.

![Режим псевдографики](image/pic11.png){width=70%}

### Добавление точек остановки

12. Ставим точку остановки и выводим о них. Видим 2 точки: первая, которую мы поставили в пункте 9, и новую.

![Точки остановки](image/pic12.png){width=70%}

### Работа с данными программы в GDB

13. Просматриваем содержимое регистров.

![Содержимое регистров](image/pic13.png){width=70%}

14. Выполняем инструкции stepi (si).

![Инструкции si](image/pic14.png){width=70%}

15. Смотрим значение переменной по имени и адресу.

![Просмотр значений переменных](image/pic16.png){width=70%}

16. Изменяем значения у переменных (букву).

![Изменение значений](image/pic18.png){width=70%}

17. Просматриваем регистр edx в hex,bin,char.

![Значения регистра в разных регистрах](image/pic19.png){width=70%}

18. Меняем значения регистра ebx. В первый раз мы ввели вернулся номер по таблице ASCII у символа '2'. Во второй раз само число.

![Изменение значений регистра](image/pic21.png){width=70%}

19. Завершаем выполнение программы и выходим через quit.

![Завершение программы](image/pic22.png){width=70%}

### Обработка аргументов командной строки в GDB

20. Копируем файл с предыдущей лабораторной работы. Создаём исполняемый файл.

![Копирование файла](image/pic23.png){width=70%}

21. Загружаем программу с аргументами в gdb, ставим точку остановки и запускаем.

![Запуск через gdb](image/pic24.png){width=70%}

22. Смотрим позиции стека. Разница в 4 обусловлена размером каждой позиции в 4 байта.

![Просмотр элементов стека](image/pic25.png){width=70%}

## Выполнение самостоятельной работы

1.  Меняем текст предыдущего задания. Отправляем вычисление функции в отдельную подпрограмму _calc.

![Измененная программа](image/pic26.png){width=70%}

![Работа программы](image/pic27.png){width=70%}

2.  Пишем в файл заданный листинг.

![Заданный текст](image/pic28.png){width=70%}

![Неправильная работа программы](image/pic29.png){width=70%}

3.  Запускаем отладчик и находим ошибку. Команда mul умножает на значение регистра и перезаписывает результат в eax (а не в ebx). Меняем ebx на eax.

![Проблема](image/pic32.png){width=70%}

![Правильная программа](image/pic33.png){width=70%}

2.  Проверяем работу.

![Работа программы](image/pic34.png){width=70%}

# Выводы

Были изучены подпрограммы и отладчик. Получены практические навыки их применений.

