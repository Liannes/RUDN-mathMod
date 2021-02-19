---
# Front matter
lang: ru-RU
title: "Отчёт по лабораторной работе"
subtitle: "Лабораторная №1"
author: "Панкратьев Александр Владимироваич"

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: Times New Roman
romanfont: Times New Roman
sansfont: Times New Roman
monofont: Times New Roman
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: lualatex
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Понять и научится решать задачи о погоне


# Задание

1. Записать  уравнение,  описывающее  движение  катера,  с  начальными условиями  для  двух  случаев.
2. Постройте траекторию движения катера и лодки для двух случаев.
3. Найдите точку пересечения траектории катера и лодки

# Теоретическая справка

* Теорема пифагора имеет вид
$a^2 + b^2 = c^2$
* Радиальная скорость - это скорость, с которой катер удаляется от полюса
* Тангенциальная  скорость – это  линейная  скорость  вращения  катера ﻿относительно  полюса.


# Выполнение лабораторной работы

Записываю данные, которые данны в задаче (рис. -@fig:001)

![Данные из задачи](image\1.png){#fig:001 width=70%}

Составляю уравнения описывающее движение катера (рис. -@fig:002) и (рис. -@fig:003)

![Уравение для k-x](image\2.1.png){#fig:002 width=70%}

![Уравение для k+x](image\2.2.png){#fig:003 width=70%}

Использую теорему Пифагора для построение тракетории (рис. -@fig:004)

![Вычисления для нахождения траектории](image\3.png){#fig:004 width=70%}

Использую Scilab Online для вычисления троектории и нахождении точки пересечения (рис. -@fig:005)

![Онлайн среда](image\0001.png){#fig:005 width=70%}

Заменяю переменные из шаблона и нахожу пересечения двух лодок по 1 случаю (рис. -@fig:006)

![Полученные данные при 1 случаи](image\4.png){#fig:006 width=70%}

Догоняем лодку где-то на 90 км от старта

Нахожу пересечения двух лодок по 2 случаю (рис. -@fig:007)

![Полученные данные при 2 случаи](image\5.png){#fig:007 width=70%}

# Вывод

Я научился решать задачи о погони и использовать среду Scilab.
