---
## Front matter
title: "Отчёт по лабораторной работе №3"
subtitle: "Дисциплина: архитектура компьютера"
author: "Цоппа Ева Эдуардовна"

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
lot: true # List of tables
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
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
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
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---


**1 Цель работы**

Целью данной работы является освоение процедуры оформления отчетов с
помощью легковесного языка разметки Markdown.

**\
**
**2 Задание**

1\. Установка необходимого ПО.

2.Заполнение отчета по выполнению лабораторной работы №3 с помощью языка
разметки Markdown.

3\. Задание для самостоятельной работы.
**3 Теоретическое введение**

Markdown -- легковесный язык разметки, созданный с целью обозначения
форматирования в простом тексте, с максимальным сохранением его
читаемости человеком, и пригодный для машинного преобразования в языки
для продвинутых публикаций. Внутритекстовые формулы делаются аналогично
формулам LaTeX. В Markdown вставить изображение в документ можно с
помощью непосредственного указания адреса изображения. Синтаксис
Markdown для встроенной ссылки состоит из части \[link text\],
представляющей текст гиперссылки, и части (file-name.md) -- URL-адреса
или имени файла, на который дается ссылка. Markdown поддерживает как
встраивание фрагментов кода в предложение, так и их размещение между
предложениями в виде отдельных огражденных блоков. Огражденные блоки
кода -- это простой способ выделить синтаксис для фрагментов кода.


**4 Выполнение лабораторной работы**

**4.1 Установление необходимого ПО**

**4.1.1 Установка TeX Live**

![Screenshot_210](https://github.com/evatsoppa/study_2023-2024_arh-pc/assets/145338773/3ea4f083-b62f-4a0c-b3bb-f32ff47224e7)


Рис.4.1. Установка TeX Live

![Screenshot_211](https://github.com/evatsoppa/study_2023-2024_arh-pc/assets/145338773/f022a2c8-0dd1-45f8-a683-7acb2a6aa000)


Рис.4.2. Установка TeX Live

**4.1.2 Установка pandoc**

![Screenshot_212](https://github.com/evatsoppa/study_2023-2024_arh-pc/assets/145338773/a18f02e4-4ad6-4bea-be53-b46fc9b0824c)


Рис.4.3. Установка pandoc

![Screenshot_213](https://github.com/evatsoppa/study_2023-2024_arh-pc/assets/145338773/cd157b10-7a06-47db-8116-07181512d0e0)

Рис.4.4. Установка pandoc

**4.2 Заполнение отчета по выполнению лабораторной работы №3 с помощью
языка разметки Markdown**

Открываю терминал. Перехожу в каталог курса, сформированный при
выполнении прошлой лабораторной работы (рис. [4.5).](#_bookmark16)

![Screenshot_214](https://github.com/evatsoppa/study_2023-2024_arh-pc/assets/145338773/de241f39-8b6a-4a78-a8b1-7535b7431867)


Рис.4.5. Перемещение между директориями

Обновляю локальный репозиторий, скачав изменения из удаленного
репозитория с помощью команды git pull (рис. [4.6).](#_bookmark17) Так,
как я запускала уже эту команду, мне высветилось "Уже актуально"

![Screenshot_275](https://github.com/evatsoppa/study_2023-2024_arh-pc/assets/145338773/06a04228-4ced-4cd6-9b1a-6638de972ccd)

Рис.4.6. Распаковка архивов

Перехожу в каталог с шаблоном отчета по лабораторной работе №3 с помощью
cd (рис. 4.7.)

![Screenshot_215](https://github.com/evatsoppa/study_2023-2024_arh-pc/assets/145338773/17c54593-9960-4e2d-8bb9-bd8e23fc3b4a)


Рис.4.7. Перемещение между директориями

Компилирую шаблон с использованием Makefile, вводя команду make
(рис.[4.8).](#_bookmark19)

![Screenshot_216](https://github.com/evatsoppa/study_2023-2024_arh-pc/assets/145338773/da922879-e6d3-43d0-8737-fae63bd2da5d)


Рис.4.8. Компиляция шаблона

Открываю сгенерированный файл report.docx LibreOffice (рис.
[4.9).](#_bookmark20)

![Screenshot_217](https://github.com/evatsoppa/study_2023-2024_arh-pc/assets/145338773/a1f715d3-41da-4fed-9131-427b4fae184d)


Рис.4.9. Открытие файла docx

Открываю сгенерированный файл report.pdf (рис. [4.10).](#_bookmark21)
Убедилась, что все правильно сгенерировалось.

![Screenshot_218](https://github.com/evatsoppa/study_2023-2024_arh-pc/assets/145338773/614ad1d8-ef53-40d1-9832-82b95b36e8bd)


Рис.4.10. Открытие файла pdf

Удаляю полученные файлы с использованием Makefile, вводя команду make
clean (рис. [4.11).](#_bookmark22) С помощью команды ls проверяю,
удалились ли созданные файлы.

![Screenshot_219](https://github.com/evatsoppa/study_2023-2024_arh-pc/assets/145338773/5418ff79-978d-48ea-989d-402c17dbd375)


Рис.4.11. Удаление файлов

Открываю файл report.md с помощью любого текстового редактора mousepad
(рис. [4.11).](#_bookmark23)

![Screenshot_220](https://github.com/evatsoppa/study_2023-2024_arh-pc/assets/145338773/810600ce-1d3d-4da8-b413-04086b684810)


Рис.4.12. Открытие файла rm

Я хочу, чтобы у меня на всякий случай сохранился шаблон отчета, поэтому
копирую файл с новым названием с помощью утилиты cp (рис.
[4.13).](#_bookmark24)

![Screenshot_221](https://github.com/evatsoppa/study_2023-2024_arh-pc/assets/145338773/cac0380a-cd03-4608-86c3-fc439c5c45dc)


Рис.4.13. Копирование файла с новым именем

Начинаю заполнять отчет с помощью языка разметки Markdown в скопирован
ном файле (рис. [4.14).](#_bookmark25)

![Screenshot_222](https://github.com/evatsoppa/study_2023-2024_arh-pc/assets/145338773/57136d85-0e47-4f70-ac47-30702d525629)


Рис.4.14. Заполнение отчета

Компилирую файл с отчетом. Загружаю отчет на GitHub.

**4.3 Задание для самостоятельной работы**

1\. Перехожу в директорию lab03/report с помощью cd, чтобы там заполнять
отчет по третьей лабораторной работе (рис. [4.15).](#_bookmark27)

![Screenshot_223](https://github.com/evatsoppa/study_2023-2024_arh-pc/assets/145338773/c0e49324-67d8-4b48-8120-206d4a6fcf0f)


Рис.4.15. Перемещение между директориями

Копирую файл report.md с новым именем для заполненния отчета (рис.
[4.16).](#_bookmark28)

![Screenshot_224](https://github.com/evatsoppa/study_2023-2024_arh-pc/assets/145338773/47f059ed-c183-4523-ba66-7ec2b9f08d5b)


Рис.4.16. Копирование файла

Открываю файл с помощью текстового редактора mousepad и начинаю
заполнять отчет (рис. [4.17).](#_bookmark29)

![Screenshot_225](https://github.com/evatsoppa/study_2023-2024_arh-pc/assets/145338773/2cc4f784-729c-4eb9-9793-5d4dd0c46e5a)


Рис.4.17. Работа над отчетом

Удаляю предыдущий файл отчета, чтобы при компиляции он мне не мешал
(рис. [4.18).](#_bookmark30)

![Screenshot_226](https://github.com/evatsoppa/study_2023-2024_arh-pc/assets/145338773/93cff4ea-3214-4ae1-816c-563495b5f04b)

Рис.4.18. Удаление предыдущих файлов

Компилирую файл с отчетом по лабораторной работе (рис.
[4.19).](#_bookmark31)

![Screenshot_228](https://github.com/evatsoppa/study_2023-2024_arh-pc/assets/145338773/949ee771-1ed1-4e0b-9080-91c967dfc83e)



Рис.4.19. Компиляция файлов

2\. Удаляю лишние сгенерированные файлы report.docx и report.pdf
[(4.20).](#_bookmark32)

![Screenshot_229](https://github.com/evatsoppa/study_2023-2024_arh-pc/assets/145338773/f44598ab-b0aa-41e9-8f1b-14d22e7d7be2)


Рис.4.20. Удаление лишних файлов

Добавляю изменения на GitHub с помощью комнадой git add и сохраняю изме-
нения с помощью commit [(4.21).](#_bookmark33)

![Screenshot_230](https://github.com/evatsoppa/study_2023-2024_arh-pc/assets/145338773/5821ab0a-17dd-4590-9241-c41232e996ee)


Рис.4.21. Добавление файлов на GitHub

Отправлялю файлы на сервер с помощью команды git pull
[(4.22).](#_bookmark34)

![Screenshot_274](https://github.com/evatsoppa/study_2023-2024_arh-pc/assets/145338773/e889028f-ea21-4f0c-b618-0d91f08eb3a8)

Рис.4.22. Отправка файлов


**5 Выводы**

> В результате выполнения данной лабораторной работы я освоила процедуры
> оформления отчетов с помощью легковесного языка разметки Markdown.

**6 Список литературы**

1\) Архитектура ЭВМ
