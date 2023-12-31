# WorkShop5
# АНАЛИЗ ДАННЫХ И ИСКУССТВЕННЫЙ ИНТЕЛЛЕКТ [in GameDev]
Отчет по лабораторной работе #5 выполнил(а):
- Коротаева Екатерина Андреевна
- РИ-220930

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

## Цель работы
Познакомиться с программными средствами для создания системы машинного обучения и ее интеграции в Unity.

## Задание 1
### Найдите внутри C# скрипта “коэффициент корреляции” и сделать выводы о том, как он влияет на обучение модели.
Ход работы: Проанализировать скрипт RollerAgent.cs, найти в нем коэффициент корреляции и провести анализ.
  
Коэффициент корреляции определяет, насколько близко объект должен находиться к цели, чтобы считаться успешным.
- Увеличение сделает задачу более легкой, т.к. объект находиться дальше от цели, чтобы сработал SetReward.
- Увеличение сделает задачу более сложной, т.к. объект находиться ближе к цели, чтобы сработал SetReward.
  
![image](https://github.com/MsKat04/WorkShop5/assets/116561169/46f27b69-ac71-4f46-8544-8cd250fa4386)

## Задание 2
### Изменить параметры файла yaml-агента и определить какие параметры и как влияют на обучение модели. Привести описание не менее трех параметров.

### Рассмотрим на примере rollerball_config.

![image](https://github.com/MsKat04/WorkShop5/assets/116561169/a94f90e6-5b18-42c8-9c0d-84d009c4ff66)



Здесь я нашла 3 параметра:

- batch_size. Параметр определяет велечину, она используется для одного обновления модели. Уменьшив значение до 3, обучение стало проводится хуже.
  
- learning_rate. Параметр устанавливает скорость обучения, которая определяет скорость адаптации к данным. Если значение этого параметра слишком низкое, то обучение будет происходить медленно, но стабильно. В то же время, слишком высокое значение параметра может привести к неравномерному обучению.

- num_epoch. Определяет, сколько раз модель обрабатывает данные обучения в каждой эпохе. Изменив параметр несколько раз, я пришела к выводу: увеличение данного параметра приводит к повышению точности обучения, однако сопровождается увеличением времени, необходимого для обучения.

## Задание 3
### А) Приведите примеры, для каких игровых задач и ситуаций могут использоваться примеры 1 и 2 с ML-Agent’ом.
### Б) В каких случаях проще использовать ML-агент, а не писать программную реализацию решения? 

### Ответ на вопрос А
- Искусственный интеллект для NPC;
- Генерация игровых уровней;
- Автоматизации тестирования игры;

### Ответ на вопрос Б
- Обучать можно на протяжении длительного времени;
- Вычисление тяжелых операций(расчет кратчайшего пути из точки А в точку В);

## Выводы

Я впервые ознакомилась с ML-агентом и изучила процесс обучения объектов в Unity, так же провела некоторые эксперименты с различными значениями параметров, чтобы понять, как они влияют на процесс обучения.

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
