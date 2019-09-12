# Введение в анализ данных

Привет. Это репозиторий курса "Введение в анализ данных" на экономическом факультете МГУ. Здесь будут выкладываться некоторые домашние задания.

## Первое домашнее задание (срок: 23:59 9 сентября)

1. Установите последнюю версию R на свою операционную систему по [ссылке](https://cran.rstudio.com)

2. Скачайте RStidio Open Source Edition по [ссылке](https://www.rstudio.com/products/RStudio)

3. Выполните следующие команды в RStudio

```R
install.packages("swirl")
library(swirl)
swirl::install_course_url('https://raw.githubusercontent.com/go95/big_data_intro/master/student_files/R_Programming.zip')
swirl()
```

Таким образом вы установите интерактивную домашнюю работу, которую вам необходимо пройти. Как ее сдать, выясните в конце работы, только пожалуйста, представьтесь интерактивной программе своим настоящим именем. :)



Из предложенных tutorials рекомендуется пройти:
1. Basic Building Blocks (оценивается 1 балл)
2. Workspace and Files (оценивается 1 балл)
3. Sequences of Numbers (оценивается 1 балл)
4. Vectors (оценивается 1 балл)
5. Missing Values (оценивается 1 балл)
6. Subsetting Vectors (оценивается 1 балл)
7. Matrices and Data Frames (оценивается 1 балл)
9. Functions (оценивается 1 балл)
12. Looking at Data (оценивается 1 балл)


## Второе домашнее задание (срок: 23:59 19 сентября) (5 баллов)

Это первая часть длинного проекта, на основе которого мы будем учиться писать чистый код и использовать функции в R

0. Вам понадобится установить пакет

```
install.packages('lintr')
```

1.Скачайте данные с публикациями Atila Abdulkadiroglu из Duke University c помощью команды

```R
articles <- read.csv(url("https://raw.githubusercontent.com/go95/big_data_intro/master/Abdulkadiroglou.csv"))
```

2. Посчитайте Индекс Хирша для Atila Abdulkadiroglu

> Учёный имеет индекс h, если h из его Np статей цитируются как минимум h раз каждая, в то время как оставшиеся (Np — h) статей цитируются не более чем h раз каждая.

Ваш код должен иметь формат .R, должен проходить проверку на Tidyverse Style Guide. Вы можете это проверить с помощью команды:

```R
library(lintr) # импорт (активация) пакета
lint("your_file.R")
```

Ваш код должен считать все промежуточные результаты, импортировать все необходимые пакеты с помощью команды library, не содержать команд install.package и запускаться из файла с помощью команды

```R
source('your_file.R')
```

В качестве результата эта команда должна печатать одно число: Индекс Хирша Atila Abdulkadiroglu

3. Сдать код: https://goo.gl/forms/F7mzTH6jESmY2AMj1 


## Acknowledgments

Some of the Home Assignments are borrowed from John Hopkins Univerity course in Data Science from Coursera. We thank Roger D. Peng et al. for distributing their Home Assignments under permissive licence.
