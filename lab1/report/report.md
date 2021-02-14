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

Научиться использовать git, а также познакомиться
с основными возможностями разметки Markdown для оформления отчётов.


# Задание

Создать Git репозиторий, придерживаясь структуры рабочего пространства.
Написать отчет по лабораторной работе в Markdown.
Загрузить в репозиторий отчёт в формате: docx и pdf.
Сделать презентацию.

# Теоретическая справка

GitHub — онлайн-хостинг репозиториев, обладающий всеми функциями системы контроля версий и функциональностью управления (в него входит всё то, что поддерживает Git). Также он предоставляет разработчикам сохранять их код онлайн, а потом использовать с другими разработчиками

Git — это инструмент, позволяющий реализовать распределённую систему контроля версий.

GitHub — это сервис для проектов

Репозиторий — каталог файловой системы, в котором могут находится: файлы журналов конфигураций и операций, выполняемых над репозиторием, а также сами контролируемые файлы.

Репозиторий бывает:

- локальный (расположен непосредственно в памяти компьютера разработчика).
- удалённый (находится на сервере, может быть приватным – доступным ограниченному числу лиц, и публичным).

# Выполнение лабораторной работы

Создал репозиторий RUDN-mathMod на платформе GitHub (рис. -@fig:001)

![Репозиторий](image\1.png){#fig:001 width=70%}

Создал для своего удобства локальную папку на жестком диске (рис. -@fig:002)

![Папка](image\2.png){#fig:002 width=70%}

Скачиваю с git репозитории для работы с Markdown (рис. -@fig:003)

![Скачиваю репозитории для создания репорта и презентаций](image\3.png){#fig:003 width=70%}

Доделываю репорт и презентацию в программе Atom (рис. -@fig:004)

![Работа в программе Atom ](image\4.png){#fig:004 width=70%}


Переношу и компелирую файлы в скачанных репозиториях (рис. -@fig:005)

![Скомпилирования файлов](image\7.png){#fig:005 width=70%}

Загружаю файлы на платформу GitHub (рис. -@fig:006)

![Загрузка на GitHub](image\6.png){#fig:006 width=70%}

Проверяем появились ли файлы на GitHub (рис. -@fig:007)

![Проверка](image\8.png){#fig:007 width=70%}

# Вывод

Мы научились использовать git, а также познакомились
с основными возможностями разметки Markdown для оформления отчётов.
