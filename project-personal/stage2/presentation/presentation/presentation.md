---
## Front matter
lang: ru-RU
title: Индивидуальный проект. Этап 2.
subtitle: Установка DVWA
author:
  - Cадова Д. А.
institute:
  - Российский университет дружбы народов, Москва, Россия

## i18n babel
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

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Садова Диана Алексеевна
  * студент бакалавриата
  * Российский университет дружбы народов
  * [113229118@pfur.ru]
  * <https://DianaSadova.github.io/ru/>

:::
::::::::::::::

# Вводная часть

## Актуальность

- Устанавливаем DVWA для работы с безопасностью сайта.

## Цели и задачи

- Установите DVWA в гостевую систему к Kali Linux.

## Материалы и методы

- Источники Интернета.

## Содержание исследования

- Перейдите в каталог www 

![Переходим в каталог html](image/1.png)

##

- Клонируйте репозиторий git:

![Клонируем репридиторий](image/2.png)

##

Измените права доступа к папке установки 

![Изменяем права доступа](image/3.png)

##

Перейдите к файлу конфигурации в каталоге установки:

![Переходим в нужный файл](image/4.png)

##

Скопируйте файл конфигурации и переименуйте его:

![Копируем файл конфигурации и переименовываем](image/5.png)

##

Откройте файл настроек и измените пароль на что-то более простое для ввода (я изменю пароль на pass):

![Открываем файл и редактируем пароль](image/6.png)

##

На следующем снимке экрана показано содержимое файла конфигурации, включая всю информацию о базе данных:

![Открываем файл и редактируем пароль](image/7.png)

##

Установите mariadb:

![Проверяем обнавления](image/8.png)

##

![Устанавливаем доп программы](image/9.png)

##

Запустите базу данных:

![Запускаем базу данных](image/10.png)

##

Войдите в базу данных (пароля нет, поэтому просто нажмите Enter при появлении запроса)

![Заходим в базу данных](image/11.png)

##

Создайте пользователя базы данных. Нужно использовать те же имя пользователя и пароль, которые использовались в файле конфигурации (см. скрин выше):

![Создаем пользователя базы данных](image/12.png)

##

Предоставьте пользователю все привилегии:

![Передаем пользователю привелегии](image/13.png)

##

Пришло время перейти в каталог apache2 для настройки сервера Apache:

![Переходим в каталог apache2](image/14.png)

##

Откройте для редактирования файл php.ini, чтобы включить следующие параметры: allow_url_fopen и allow_url_include.

![Редактируем файл php.ini](image/15.png)

##

![Редактируем файл php.ini](image/16.png)

##

Запустите сервер Apache:

![Запускаем сервер Apache](image/17.png)

##

Если все сделали правильно, то можно открыть DVWA в браузере, введя в адресной строке следующее:

![Вводим адрис DVWA в браузере](image/18.png)

##

Если открылась страница настройки, это означает, что вы успешно установили DVWA на Kali Linux 

![Окно DVWA на Kali Linux](image/19.png)

## Результаты

- Мы смогли установить DVWA в гостевую систему к Kali Linux.

