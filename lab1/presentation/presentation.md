---
## Front matter
lang: ru-RU
title: Использование Git репозитория
date: 12 February, 2020

## Formatting
mainfont: Times New Roman
romanfont: Times New Roman
sansfont: Times New Roman
monofont: Times New Roman
toc: false
slide_level: 2
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
aspectratio: 43
section-titles: true
---

## Что же такое GitHub и Git

- GitHub — онлайн-хостинг репозиториев, который обладает функциями контроля версий и управления.

- Git - Это инструмент, который реализовает распредления контроля версий

## Репозитории
Репозиторий - это файловая система, в которой находятся:
1. Файлы конфигураций
2. Файлы операций
Репозитории бывают:
1. Локальные
2. Удаленные

# Команды в git
## Основные команды
- branch
- init
- add
- commit
- push
- remote

## branch
Это своего рода “менеджер веток”.
Он может
1. Переменовать
2. Удалять
3. Добовлять
4. Перечесляет все "ветки"

## init
 Это команда создает директорию .git для работы с git системой

## add
Эта команда добавляет в буфер определенный файлы
К примеру: git add README.md
Также можно перечислять друг за другом другие файлы
К примеру: git add README.md Main.java

## commit
Эта команда для записи индексированных изменений в репозиторий Git
Для того чтобы она работала нужны файлы в буфере add

## remote
Эта команда подключает созданые репозиторий на платформе GitHub
Пример: git remote add origin <Путь директории>

## push
Эта команда отправляет файлы и комментарии файлов на сервера GitHub
Пример:git push -u origin <Ветка>


## Спасибо за внимание
> Панкратьев Александр НФИбд-02-18
