---
## Front matter
title: " Индивидуальный проект. Этап 3."
subtitle: "Использование Hydra"
author: "Диана Алексеевна Садова"

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

# Цель работы

Разобратся в работе Hydra и взломать пользовательскую запись на DVWA.

# Последовательность выполнения работы

1. Скачать словарь можно с GitHub. Архив весит 50.8мб. (рис. [-@fig:001]).

![Скачиваем словать](image/1.png){#fig:001 width=90%}

2. Разархивируем его на рабочий стол  (рис. [-@fig:002]), (рис. [-@fig:003]).

![Открываем сам арфив](image/3.png){#fig:002 width=90%}

![Файл на рабочем столе](image/4.png){#fig:003 width=90%}

3. Переходим в окно DVWA и открываем панель кода страници (Важно: перед открытием обновите страницу). Нам нужна вкладка Cookies. Находим PHPSESSID и копируем строку Value (рис. [-@fig:004]).

![PHPSESSID и Value](image/6.png){#fig:004 width=90%}

4. Переходим в консоль и используем заготовленую строку с ТУИС для работы Hydra. Добавляем на место PHPSESSID, полученный из предыдущего шага, код и запускаем программу. У нас должно вывестись логин и пароль от пользователя (меня) к сайту DVWA (рис. [-@fig:005]).

![Пароль для сайта](image/7.png){#fig:005 width=90%}

5. Проверяем правильность пароля и логина (рис. [-@fig:006]).

![Пароль подходит](image/5.png){#fig:006 width=90%}

# Выводы

Мы смогли разобратся с работой Hydra и достать пароль и логин пользователя (меня).

# Список литературы{.unnumbered}

::: {#refs}
:::
