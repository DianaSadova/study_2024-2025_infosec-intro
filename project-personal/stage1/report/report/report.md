---
## Front matter
title: " Индивидуальный проект. Этап 1."
subtitle: "Установка Kali Linux"
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

Целью данной работы является установка системы Kali Linux

# Последовательность выполнения работы

Устанавливаем виртуальную машину (рис. [-@fig:001]).

![Устонавливаем новую виртуальную машину](image/1.png){#fig:001 width=90%}

Устанавливаем основную память, жёсткий диск, процессор(рис. [-@fig:002]).

![Устонавливаем основную систему](image/2.png){#fig:002 width=90%}

Снимаем галочку с "Гибкий диск" (рис. [-@fig:003]).

![Устонавливаем основную систему](image/3.png){#fig:003 width=90%}

Устанавливаем оптичиский диск, заранее скаченый(рис. [-@fig:004]).

![Устонавливаем основную систему](image/4.png){#fig:004 width=90%}

Проверяем настройки сети и тип подключения. Он должен быть NAT(рис. [-@fig:005]).

![Устонавливаем основную систему](image/5.png){#fig:005 width=90%}

Запускаем систему и начинаем установку Kali, я устонавливала через графический интерфейс(рис. [-@fig:006]).

![Запускаем систему](image/6.png){#fig:006 width=90%}

Выбераем язык (рис. [-@fig:007]).

![Выбераем язык ](image/7.png){#fig:007 width=90%}

Настраиваем клавиотуру (рис. [-@fig:008]).

![Настраиваем клавиотуру](image/8.png){#fig:008 width=90%}

Выбераем имя компьютора в сети. Я оставила изночальное "vbox"(рис. [-@fig:009]).

![Выбераем имя компьютора в сети](image/9.png){#fig:009 width=90%}

Создаем учетную запись пользователя (рис. [-@fig:010]),(рис. [-@fig:011]).

![Создаем учетную запись](image/10.png){#fig:010 width=90%}

![Установка пароля для root](image/11.png){#fig:011 width=90%}

Выбераем режим как мы будем использовать диск. У меня авто (рис. [-@fig:012]).

![Выбераем режим как мы будем использовать диск](image/12.png){#fig:012 width=90%}

Сохраняем изменения (рис. [-@fig:013]).

![Сохраняем изменения ](image/13.png){#fig:013 width=90%}

Устанавливаем системного загрузчика GRUB (рис. [-@fig:014]),

![Устанавливаем системного загрузчика GRUB](image/15.png){#fig:014 width=90%}

Указываем на наше устройстко для полной загрузки (рис. [-@fig:015]).

![Указываем на наше устройстко для полной загрузки](image/16.png){#fig:015 width=90%}

Завершаем установку Kali Linux (рис. [-@fig:016]).

![Завершаем установку](image/17.png){#fig:016 width=90%}

Заходим и автаризуемся в нашей новой вертуальной машине. Установка завершена (рис. [-@fig:017]).

![Заходим и автаризуемся в вертуальной машине](image/18.png){#fig:017 width=90%}

# Выводы

Мы приобрели практические навыки установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.

# Список литературы{.unnumbered}

::: {#refs}
:::
