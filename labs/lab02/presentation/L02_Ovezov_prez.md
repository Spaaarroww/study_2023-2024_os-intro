﻿Лабораторная работа№2![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.001.png)

Операционные системы

Овезов Мерген

3марта 2023

Российский университет дружбы народов, Москва, Россия

1/13

<a name="_page1_x0.00_y0.48"></a>[Цель работы](#_page1_x0.00_y0.48)![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.002.png)


Цель работы![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.003.png)

Цель данной лабораторной работы – изучение идеологии и применения средств контроля версий, освоение умения по работе с git.

2/13

<a name="_page3_x0.00_y0.48"></a>[Задание](#_page3_x0.00_y0.48)![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.004.png)


Задание![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.005.png)

1\.Создать базовую конфигурацию для работы c git 2.Создать ключ SSH 3.Создать ключ GPG 4.Настроить подписи Git 5.Зарегистрироваться на GitHub 6.Создать локальный каталог для выполнения заданий по предмету # Теоретическое введение

Основные команды git

Перечислим наиболее часто используемые команды git. 

Создание основного дерева репозитория:

git init

Получение обновлений (изменений) текущего дерева из центрального репозитория: 

git pull

Отправка всех произведённых изменений локального дерева в центральный репо3/з1и3 т

<a name="_page5_x0.00_y0.48"></a>[Выполнениелабораторнойработы](#_page5_x0.00_y0.48)![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.006.png)

Установкапрограммного обеспечения![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.007.png)

Установка необходимого программного обеспечения git и gh через терминал с помощью команд: dnf install git и dnf install gh (рис.1).

![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.008.png)

Рис.1:Рис 1

4/13![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.009.png)

Базовая настройка git![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.010.png)

Задаю в качестве имени и email владельца репозитория свои имя,фамилию и электронную почту(рис 2)

![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.011.png)

Рис.3:Рис 2

Настраиваю utf-8 в выводе сообщений git дли их корректного отображения![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.012.png)

Рис.4:Рис 3

Начальной ветке задаю имя master

5/13![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.013.png)

Создание ключа SSH![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.014.png)

Создаю ключ ssh размером 4096 бит по алгоритму rsa

![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.015.jpeg)

Рис.7:Рис 6 6/13


Создание Ключа GPG![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.016.png)

Генерирую ключ GPG,затем выбираю тип ключа RSA and RSA, задаю макс. длину ключа;4096,оставляю неограниченный срок действия ключа. Далее отвечаю на вопросы программы о личной информации

7/13![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.017.jpeg)

Регистрация на GitHub![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.018.png)

У меня уже был создан аккаунт на Github, соответственно, основные данные аккаунта я так же заполнил и проводил его настройку, поэтому просто вхожу в свой аккаунт

![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.019.png)

Рис.10:Рис 9

8/13

Добавление ключа GPG в GitHub![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.020.png)

Вывожу список созданных ключей в терминал, ищу в результате запроса отпечаток ключа (последовательность байтов для идентификации более длинного, по сравнению с самим отпечатком, ключа), он стоит после знака слеша, копирую его в буфер обмена

![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.021.png)

Рис.11:Рис 10

Ввожу в терминале команду,с помощью которой копирую сам ключ GPG в буфер обмена, за это отвечает утилита xclip.

9/13![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.022.png)

НастроитьподписиGit![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.023.png)

Настраиваю автоматические подписи коммитов git: используя введенный ранее email, указываю git использовать его при создании подписей коммитов.

![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.024.png)

Рис.14:Рис 13

10/13

Настройкаgh![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.025.png)

Начинаю авторизацию в gh, отвечаю на наводящие вопросы от утилиты, в конце выбираю авторизоваться через браузер

![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.026.png)

Рис.15:Рис 14

Завершаю авторизацию на сайте

11/13![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.027.png)

Создание репозитория курса на основе шаблона![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.028.png)

Сначала создаю директорию с помощью утилиты mkdir и флага -p, кторый позволяет установить каталоги на всем указанном пути. После этого с помощью утилиты cd перехожу в только что созданную директорию “Операционные системы”. Далее в терминале ввожу команду gh repo create study\_2023-2024\_os-intro –template yamadharma/course-derctory-student-trmplate–public, чтобы создать репозиторий на основе шаблона репозитория. После этого клонирую репозиторий к себе в директорию, я указываю ссылку с протоколом https, а не ssh, потому что при авторизации в gh выбрала протокол https

![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.029.png) 12/13


Выводы![](Aspose.Words.95f02a6c-532c-46cd-8a9e-349b1d2e89f9.030.png)

При выполнении данной лабораторной работы я изучил идеологию и применение средств контроля версий, освоил умение по работе с git.
13/13
