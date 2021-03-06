# Проект 0. Угадай число

## Оглавление  
[1. Описание проекта](README.md#Описание-проекта)  
[2. Какой кейс решаем?](README.md#Какой-кейс-решаем)  
[3. Краткая информация о данных](README.md#Краткая-информация-о-данных)  
[4. Этапы работы над проектом](README.md#Этапы-работы-над-проектом)  
[5. Результаты](README.md#Результаты)  
[6. Выводы](README.md#Выводы)  


### Описание проекта    
Угадать загаданное компьютером число за минимальное число попыток

:arrow_up:[к оглавлению](README.md#Оглавление)  


### Какой кейс решаем?    
Нужно написать программу, которая угадывает число за минимальное число попыток

**Условия соревнования:**  
- Компьютер загадывает целое число от 1 до 100, и нам его нужно угадать. Под «угадать», подразумевается «написать программу, которая угадывает число».
- Алгоритм учитывает информацию о том, больше ли случайное число или меньше нужного нам.

**Метрика качества**     
Результаты оцениваются по среднему количеству попыток при 1000 повторений

**Что практикуем**     
Учимся писать хороший код на python


### Краткая информация о данных
Для тестирования алгоритмов использовалась последовательность из 1000 псевдослучайных натуральных чисел от 1 до 100
  
:arrow_up:[к оглавлению](README.md#Оглавление)  


### Этапы работы над проектом  
Тестировались 4 алгоритма поиска числа:
 1. Алгоритм случайного угадывания (random_predict)  

    *Случайный перебор чисел из указанного диапазона (как в примере)*

 2. Алгоритм случайного деления интервала (random_division_predict)

    *На первом шаге исходный интервал 1..100 делится на две части случайным образом, на последующих шагах случайным образом делится та часть, которая соответствуем ответу "меньше-больше"*

 3. Алгоритм поиска по разрядам (by_category_predict)

    *Сначала методом подбра определяются десятки, затем единицы искомого числа*


 4. Алгоритм половинного деления (half_division_predict)

    *Используется метод половинного деления, когда на каждой итерации нужная чась последовательности делится пополам*
    

:arrow_up:[к оглавлению](README.md#Оглавление)  


### Результаты:
Тестировались 4 алгоритма поиска числа:
 1. Алгоритм случайного угадывания (random_predict)

    *Алгоритм находит число в среднем за 99 итераций. 0.26559 секунд на 1000 наблюдений*

 2. Алгоритм случайного деления интервала (random_division_predict)

    *Алгоритм находит число в среднем за 8 итераций. 0.02561 секунд на 1000 наблюдений*

 3. Алгоритм поиска по разрядам (by_category_predict)

    *Алгоритм находит число в среднем за 5 итераций. 0.00481 секунд на 1000 наблюдений*


 4. Алгоритм половинного деления (half_division_predict)

    *Алгоритм находит число в среднем за 4 итераций. 0.00233 секунд на 1000 наблюдений*

:arrow_up:[к оглавлению](README.md#Оглавление)  


### Выводы:  
**Наилучшим для решения данной задачи является, как и ожидалось, алгоритм, использующий метод половинного деления**

Впрочем, если распределение чисел в тестируемой последовательности отлично от нормального, результаты могут отличаться от представленных.

:arrow_up:[к оглавлению](README.md#Оглавление)  


Если информация по этому проекту покажется вам интересной или полезной, то я буду очень вам благодарен, если отметите репозиторий и профиль ⭐️⭐️⭐️-дами
