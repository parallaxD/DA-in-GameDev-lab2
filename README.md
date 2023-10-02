# АНАЛИЗ ДАННЫХ И ИСКУССТВЕННЫЙ ИНТЕЛЛЕКТ [in GameDev]
Отчет по лабораторной работе #1 выполнил(а):
- Куплевацкий Денис Игоревич
- РИ220931

Отметка о выполнении заданий (заполняется студентом):

| Задание | Выполнение | Баллы |
| ------ | ------ | ------ |
| Задание 1 | * | 60 |
| Задание 2 | * | 20 |
| Задание 3 | * | 20 |

знак "*" - задание выполнено; знак "#" - задание не выполнено;

Работу проверили:
- к.т.н., доцент Денисов Д.В.
- к.э.н., доцент Панов М.А.
- ст. преп., Фадеев В.О.

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

Структура отчета

- Данные о работе: название работы, фио, группа, выполненные задания.
- Цель работы.
- Задание 1. Написать программу Hello World на Python с запуском в Jupiter Notebook.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Задание 2. Написать программу Hello World на C# с запуском на Unity.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Задание 3. Оформить отчет в виде документации на github.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Выводы.

## Цель работы
Установить необходимое программное обеспечение, которое пригодится для создания интеллектуальных моделей на Python. Рассмотреть процесс установки игрового движка Unity для разработки игр.

## Задание 1
### Написать программу Hello World на Python с запуском в Jupiter Notebook.
Ход работы:
- С сайта https://www.anaconda.com был установлен дистрибутив Anaconda. Через anaconda-navigator был запущен инструмент Jupyter Notebook. В окне браузера была создана папка DataAnalysis и файл HelloWorld.ipynb внутри неё.
В файл была вписана команда **print('Hello World')**

![image](https://github.com/parallaxD/DA-in-GameDev-lab1/assets/81700733/11c8d099-5c07-4d7b-9c7b-41e8b01f7f41)

![image](https://github.com/parallaxD/DA-in-GameDev-lab1/assets/81700733/eb2735d0-dc29-457c-b3d0-04b010630aeb)

![image](https://github.com/parallaxD/DA-in-GameDev-lab1/assets/81700733/17a4dfca-e274-47cc-aac9-8fc41d05964f)


## Задание 2
### Написать программу Hello World на C# с запуском на Unity.

- С сайта https://unity.com был установлен игровой движок **Unity** и приложение **Unity Hub**.
- Создан пустой 3D-проект под названием Data Analysis In GameDev.
- На сцене был создан пустой объект под названием **HelloWorldWriter**
- Была создана папка **Scripts** и скрипт в ней под названием **HelloWorldWriter**
- Скрипт был прикреплен к объекту **HelloWorldWriter**
- В методе Start() был реализован вывод сообщения "Hello World" в консоль Unity с помощью класса Debug и метода Log().

![image](https://github.com/parallaxD/DA-in-GameDev-lab1/assets/81700733/56280e0b-9da9-453f-96f2-137b574f0aa6)

![image](https://github.com/parallaxD/DA-in-GameDev-lab1/assets/81700733/894fdb64-d627-47e0-9ebc-744e6d471886)

![image](https://github.com/parallaxD/DA-in-GameDev-lab1/assets/81700733/9c4c1ad9-c3e0-418b-b717-10083f930865)


```C#

using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class HelloWorldWriter : MonoBehaviour
{
    void Start()
    {
        Debug.Log("Hello World");
    }
}

```

## Задание 3
### Оформить отчет в виде документации на github.

- Из документа #Workshop#1 (полученного с сайта https://bigdigital-gamelab.ru/analiz-dannyh/) был получен шаблон отчёта по лабораторной работе.
- Шаблон был скопирован в личный репозиторий.
- В шаблон были внесены изменения в таблицу **отметка о выполнении заданий** и в **ФИО**, приведены ход и результаты выполнения заданий.

![image](https://github.com/parallaxD/DA-in-GameDev-lab1/assets/81700733/836077db-19d7-4078-a956-438ddf787a65)

![image](https://github.com/parallaxD/DA-in-GameDev-lab1/assets/81700733/6a498529-0e41-4bad-944b-63fc4bc9a6a2)




## Выводы

В результате выполнения работы на компьютер был установлен дистрибутив **Anaconda** и игровой движок **Unity**. Кроме того, через **Anaconda Navigator** я запустил **Jupyter** и написал программу, выводящую сообщение "Hello World".
В Unity я создал скрипт, выводящий в консоль сообщение "Hello World."
Также оформил свой первый отчёт по работе.

В итоге, было установлено всё необходимое программное обеспечение для работы на курсе, а также было проведено знакомство с ним.

| Plugin | README |
| ------ | ------ |
| Dropbox | [plugins/dropbox/README.md][PlDb] |
| GitHub | [plugins/github/README.md][PlGh] |
| Google Drive | [plugins/googledrive/README.md][PlGd] |
| OneDrive | [plugins/onedrive/README.md][PlOd] |
| Medium | [plugins/medium/README.md][PlMe] |
| Google Analytics | [plugins/googleanalytics/README.md][PlGa] |

## Powered by

**BigDigital Team: Denisov | Fadeev | Panov**
