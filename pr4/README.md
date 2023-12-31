# Практическое работа 4
БИСО-01-20 Калбак

# Исследование метаданных DNS трафика

## Цель работы

1.  Закрепить практические навыки использования языка программирования R
    для обработки данных;
2.  Закрепить знания основных функций обработки данных экосистемы
    `tidyverse` языка R;
3.  Закрепить навыки исследования метаданных DNS трафика.

## Исходные данные

1.  ОС Windows 10
2.  RStudio Desktop
3.  Интерпретатор языка R 4.3.0
4.  Пакет `dplyr`
5.  Файл `dns.log`
6.  Файл `header.csv`

## Общая ситуация

Вы исследуете подозрительную сетевую активность во внутренней сети
Доброй Организации. Вам в руки попали метаданные о DNS трафике в
исследуемой сети. Исследуйте файлы, восстановите данные, подготовьте их
к анализу и дайте обоснованные ответы на поставленные вопросы
исследования.

## Ход выполнения работы

### Подготовка данных

Дл начала устанавливаем пакет`dplyr` с помощью
`install.packages('dplyr')`.\`

После этого подключаем пакет к текущему проекту. Также подключаем
библиотеки.

``` r
library(dplyr)
```

    Warning: package 'dplyr' was built under R version 4.3.2


    Attaching package: 'dplyr'

    The following objects are masked from 'package:stats':

        filter, lag

    The following objects are masked from 'package:base':

        intersect, setdiff, setequal, union

``` r
library(readr)
```

    Warning: package 'readr' was built under R version 4.3.2

``` r
library(jsonlite)
```

    Warning: package 'jsonlite' was built under R version 4.3.2

#### 1. Импортируйте данные DNS

#### 2. Добавьте пропущенные данные о структуре данных (назначении столбцов)

#### 3. Преобразуйте данные в столбцах в нужный формат

### Анализ

#### 4. Сколько участников информационного обмена в сети Доброй Организации?

#### 5. Какое соотношение участников обмена внутри сети и участников обращений к внешним ресурсам?

#### 6. Найдите топ-10 участников сети, проявляющих наибольшую сетевую активность.

#### 7. Найдите топ-10 доменов, к которым обращаются пользователи сети и соответственное количество обращений

#### 8. Опеределите базовые статистические характеристики (функция summary()) интервала времени между последовательным обращениями к топ-10 доменам.

#### 9. Часто вредоносное программное обеспечение использует DNS канал в качестве канала управления, периодически отправляя запросы на подконтрольный злоумышленникам DNS сервер. По периодическим запросам на один и тот же домен можно выявить скрытый DNS канал. Есть ли такие IP адреса в исследуемом датасете?

### Обогащение данных

#### 10. Определите местоположение (страну, город) и организацию-провайдера для топ-10 доменов. Для этого можно использовать сторонние сервисы, например https://v4.ifconfig.co/.

## Оценка результатов

## Вывод
