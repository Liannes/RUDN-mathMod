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

Рассмотреть модель взаимодействия двух видов типа «хищник — жертва». Вариант 37.


# Задание

Для модели «хищник-жертва»:

$\begin{cases} \frac{dx}{dt}=-ax(t)+bx(t)y(t)\\\frac{dy}{dt}=cy(t)-dx(t)y(t) \end{cases}$

Построить график зависимости численности хищников от численности жертв, а также графики изменения численности
хищников и численности жертв при следующих начальных условиях: $x_{0}=9, y_{0}=18$. Найти стационарное состояние системы.
Значения коэффициентов: a=0.79, b=0.078, c=0.77, d=0.076

# Теоретическая справка

Простейшая модель взаимодействия двух видов типа «хищник — жертва» - или модель Лотки-Вольтерры основывается на
следующих предположениях:
1. Численность популяции жертв x и хищников y зависят только от времени
(модель не учитывает пространственное распределение популяции на
занимаемой территории)
2. В отсутствии взаимодействия численность видов изменяется по модели
Мальтуса, при этом число жертв увеличивается, а число хищников падает
3. Естественная смертность жертвы и естественная рождаемость хищника
считаются несущественными
4. Эффект насыщения численности обеих популяций не учитывается
5. Скорость роста численности жертв уменьшается пропорционально
численности хищников


$\begin{cases} \frac{dx}{dt}=ax(t)-bx(t)y(t)\\\frac{dy}{dt}=-cy(t)+dx(t)y(t) \end{cases}$

В этой модели x – число жертв, y - число хищников. Коэффициент a
описывает скорость естественного прироста числа жертв в отсутствие хищников, с
- естественное вымирание хищников, лишенных пищи в виде жертв. Вероятность
взаимодействия жертвы и хищника считается пропорциональной как количеству
жертв, так и числу самих хищников (xy). Каждый акт взаимодействия уменьшает
популяцию жертв, но способствует увеличению популяции хищников (члены -bxy
и dxy в правой части уравнения).

Математический анализ этой (жесткой) модели показывает, что имеется
стационарное состояние (рис. -@fig:001, А), всякое же другое начальное состояние (B)
приводит к периодическому колебанию численности как жертв, так и хищников,
так что по прошествии некоторого времени система возвращается в состояние B.

![Модель Лотки-Вольтерры](image/4.png){#fig:001 width=70%}



# Выполнение лабораторной работы

Для работы я использовал язык Python. Я задал необходимые начальные параметры и определил
систему дифференциальных уравнений, описывающую изменение популяций.

## Изменение численности хищников и жертв

На рис. -@fig:002 показан график изменения численности хищников и жертв с течением времени

![Графики изменеия численности популяций](image/1.png){#fig:002 width=70%}

Как видно из рисунка, популяции циклически увеличиваются и уменьшаются одна за другой.

## Зависимость численности хищников от численности жертв.

На рис. -@fig:003 показан график зависимости численности хищников от численности жертв. Как видно из
рисунка, цикл не статический, с каждым оборотом амплитуда увеличивается, то есть максимальное количество особей
на каждом новом шаге становится больше, а минимальное количество меньше.

![График зависимости численности хищников от численности жертв](image/2.png){#fig:003 width=70%}

## Стационарное состояние системы.

На рис. -@fig:004 показан график стационарного состояния системы, то есть при каждом новом обороте цикла общее
количество особей сохраняется. Это положение системы достигается при $x_{0}=13, y_{0}=18$.

![График стационарного состояния системы хищник-жертва](image/3.png){#fig:004 width=70%}

# Вывод

Я построил и проанализировал модель взаимодействия двух видов типа «хищник — жертва».
