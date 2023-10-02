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
  
- Цель работы

- Задание 1. Выбрать одну из компьютерных игр, привести скриншот её геймплея и краткое описание концепта игры. Выбрать одну из игровых переменных в игре (ресурсы, внутри игровая валюта, здоровье персонажей и т.д.), описать её роль в игре, условия изменения / появления и диапазон допустимых значений. Постройть схему экономической модели в игре и указать место выбранного ресурса в ней.
  
- Задание 2. С помощью скрипта на языке Python заполните google-таблицу данными, описывающими выбранную игровую переменную в выбранной игре (в качестве таких переменных может выступать игровая валюта, ресурсы, здоровье и т.д.). Средствами google-sheets визуализируйте данные в google-таблице (постройте график, диаграмму и пр.) для наглядного представления выбранной игровой величины.
  
- Задание 3. Оформить отчет в виде документации на github.
  
- Выводы.

## Цель работы
Научиться передавать в Unity данные из Google Sheets с помощью Python.

## Задание 1
### Выбрать одну из компьютерных игр, привести скриншот её геймплея и краткое описание концепта игры. Выбрать одну из игровых переменных в игре (ресурсы, внутри игровая валюта, здоровье персонажей и т.д.), описать её роль в игре, условия изменения / появления и диапазон допустимых значений. Постройть схему экономической модели в игре и указать место выбранного ресурса в ней.
Ход работы:  
 При помощи личного опыта и ресурса **https://dota2.fandom.com/ru/wiki/Dota_2_Вики** было создано описание концепта игры и роли золота в игре. Тажке была построена схема экономической модели в игре:
 
 Dota 2 — многопользовательская командная компьютерная игра в жанре MOBA, разработанная и изданная корпорацией Valve. Игра изображает сражение на карте особого вида: 

1) **Командная игра**: "Dota 2" является командной игрой, где две команды, (Свет и Тьма), соревнуются друг с другом. Каждая команда состоит из пяти игроков, и целью игры является разрушение главного здания противника, которая называется "Древний" (Ancient). 

  

2) **Роли и герои**: Игроки выбирают персонажей, каждый из которых обладает уникальными способностями и ролями. Роли включают в себя трёх кор-героев (carry) и двух саппорт-героев (support). Комбинирование различных героев и их способностей играет важную роль в стратегии. 

  

3) **Линии и фазы игры**: Игра разделена на три линии (верхняя, средняя и нижняя) и лес (jungle), где герои сражаются за опыт и золото. Фазы игры включают в себя начальную игру, среднюю игру и конечную игру, и стратегии могут различаться в зависимости от этапа. 

  

4) **Инвентарь и предметы**: Герои могут приобретать предметы и снаряжение, чтобы улучшить свои характеристики и способности. Создание правильной комбинации предметов является важной частью игровой стратегии. 

  

5) **Эскалация битв**: В "Dota 2" часто происходят большие сражения между командами". Эти массовые битвы создают динамичную и захватывающую игровую атмосферу. 

  

В "Dota 2" стратегия, навык и командное взаимодействие играют решающую роль, и игра предлагает глубокий и конкурентный игровой опыт для игроков со всего мира. 

  

 ![image](https://github.com/parallaxD/DA-in-GameDev-lab2/assets/81700733/342fb9a1-0bc1-473a-ac8a-ecd3c18786cd)


  

Ресурс для рассмотрения в рамках данной работы - **золото**. 

Золото играет критическую роль, так как это один из основных игровых ресурсов, который влияет на успех команды. Золото используется для приобретения предметов, улучщающих персонажей, позволяет герою возродиться мгновенно. 


Добыча золота- один из важнейших аспектов игры. 

 

1) **Источники золота**: 

- Убийство крипов (подвластных и неподвластных игрокам). 

- Убийство героев вражеской команды (125 + (УровеньУбитогоГероя × 8) + ЗначениеСерииУбийств). 

- Разрушение вражеских строений. 

- Каждый игрок пассивно получает 1  надёжного золота каждые 0,67 секунды (начиная с 0:00 по игровому времени), что в итоге даёт 90  золота в минуту в начале игры. Это периодическое золото увеличивается со временем игры.	 

 | Время в игре (мин.) | Золота в минуту (ед.) |
 | ------ | ------ |
 | 0:00 | 90 | 
 | 12:00 | 94.8 |
 | 30:00 | 99.8 |
 | 45:00 | 105.5 |
 | 62:00 | 112.8 |
 | 87:00 | 120.5 |
 | 112:00 | 129 |
 | 140:00 | 139 |
 | 175:00 | 150.5 |
 

- Подбор рун богатства. 

- Некоторые игровые способности дают героям золото. 

- Продажа предметов. 

	 

2) **Потеря золота**: 

	Основное применение золота состоит в покупке предметов. Игрок с наибольшим количеством золота способен купить самые могущественные предметы, и, тем самым, иметь очень сильного героя. Предметы, покупаемые каждым игроком, зависят от его роли в команде и множества других факторов. 

	Каждый раз, когда герой умирает, он теряет **Общая ценность**/40 золота. 

	“Выкуп”: герой может моментально возродиться за 200 + **Общая ценность** / 13 золота. 

 

3) **Диапазон значений**: от 0 до 99999. 



## Задание 2
### С помощью скрипта на языке Python заполните google-таблицу данными, описывающими выбранную игровую переменную в выбранной игре (в качестве таких переменных может выступать игровая валюта, ресурсы, здоровье и т.д.). Средствами google-sheets визуализируйте данные в google-таблице (постройте график, диаграмму и пр.) для наглядного представления выбранной игровой величины.




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
