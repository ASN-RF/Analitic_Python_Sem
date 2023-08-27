# Семинары. Основы языка Python для аналитиков
## Семинар 1. Оформление ноутбука и закрепление функций и генераторов
**Задача 1.** <br>
*1.1. Соедините два словаря в один.*<br>

```
dict1 = {'One': 1, 'Two': 2, 'Three': 3}
dict2 = {'Four': 4, 'Five': 5, 'Six': 6}
```

*1.2. Напишите функцию, которая на вход принимает два словаря и возвращает один объединенный словарь. !Используйте анотирование типов!*<br>

**Задача 2.** *Напишите функцию, которая из двух списков, делает один словарь, где элементы из первого списка - ключи, а элементы из торого списка - значения.*<br>

```
keys = ['One', 'Two', 'Three']
values = [1, 2, 3]
```

*!Используйте анотирование типов!*<br>

*2.1. Используя цикл for.*<br>

*2.2. Используя dict comprehensions.*<br>

**Задача 3.** *Извлеките только два ключа name и age из представленного словаря.*

```
clien_dict = {
    "name": "John",
    "age": "25",
    "salary": 5000,
    "city": "Moscow"
}
```

*3.1. Напишите функцию с циклом for.*<br>
Функция на вход принимает:<br>
* исходный словарь<br>
* ключи, которые нужно извлечь (аргумент по умолчанию)<br>

На выходе словарь с нужными ключами<br>
*!Используйте аннотирование типов!*<br>

*2.2. Используя dict comprehensions.*<br>

**Задача 4.** <br>
*4.1 Сгенерируйте случайные целые числа от 0 до 100 в количестве 5 штук с помощью модуля random*
● Зафиксируйте псевдогенерацию, чтобы сгенерированные значения всегда были одинаковые
● Используйте list comprehensions

*4.2 Напишите генератор*<br>

Генератор на вход принимает список с данными о клиенте (данные из пункта 4.1)<br>
Внутри генератора реализуйте обход по списку с данными На каждой итерации генератор будет возвращать кортеж из двух элементов:<br>
1. данные по клиенту (в зависимости от итерации, на 0 итерации вернется 0 элемент, на 1 итерации вернется 1 элемент и тд).<br>
2. целочисленное значение, которое показывает, сколько секунд прошло с предыдущей итерации.<br>
Примечание: секунды, которые возвращаются должны показывать время не с начала запуска генератора, а именно то время, которое прошло с
предыдущей итерации. А значит время на первой итерации должно равняться 0. Используйте функцию time из модуля time для подсчета времени.
Чтобы проверить работу таймера, , запустите проход по генератору в цикле с time.sleep(2)

**Задача 5.** <br>
*5.1 Найдите картинку в интернете и прикрепите её в ячейку с текстом.*<br>
*5.2 Создайте следующую таблицу в ячейке с текстом.*<br>

**Задача 6.** <br>
*5.1. Напишите функцию, которая может принимать любое количество трат пользователя и считать сумму и среднее.*<br>
* На вход поступают целочисленные значения в любом количестве.<br>
* На выходе словарь с ключами суммы трат и средней траты.


# Семинар 2. Анализ данных с библиотекой Pandas <br>
**Задача 1.** <br>
*1.1. Скачать данные по ссылке https://gbcdn.mrgcdn.ru/uploads/asset/5348083/attachment/7cfe8f43668ef0df20c7a6554dca48c6.csv* <br> 
*1.2. Считать данные с помощью pandas.* <br>
*1.3. Вывести на экран первые 5 строк.* <br>
*1.4. Посмотреть на описание признаков и на их содержание.* <br>

**Задача 2.** <br>
*2.1. Проведите первичный анализ данных.* <br>
*2.2. Изучите типы данных.*<br>
*2.3. Найдите количество пропущенных ячеек в данных.*<br>
*2.4. Посчитайте основные статистики по всем признакам и поизучайте их.*<br>

**Задача 3.** <br>
*3.1. Ноутбуков от какой компании больше всего в наборе данных?* <br>
*3.2. Какая минимальная и максимальная стоимость у ноутбуков в данных?*<br>
*3.3. Какой самый дорогой ноутбук в данных? Выведите все характеристики только по этому ноутбуку Если таких ноутбуков несколько, то выводите их всех.*<br>

**Задача 4.** <br>
*4.1. Найдите ноутбуки с самой маленькой диагональю в данных?* <br>
Выведите только следующие характеристики:
```
1. Компания
2. Типа ноутбука
3. Диагональ
4. Стоимость
```
*Если таких ноутбуков несколько, то выводите их всех.*<br>

*4.2. Сколько стоит самый дорогой ноутбук у компании HP?*<br>
*4.3. Как много ноутбуков Ultrabook с 8GB RAM?*<br>
*Найдите сколько таких ультрабуков с 8GB ОЗУ в процентном соотношении относительно всех ультрабуков.*


**Задача 5.** <br>
*5.1. Выберите ноутбук клиенту. Клиент хочет подобрать ноутбук с 8GB или 16GB ОЗУ на Windows 10 в стоимости до 500 евро, сколько у него вариантов?* <br>
*5.2. Выберите ноутбук клиенту. Клиент хочет подобрать ноутбук от MSI, с видеокартой Nvidia GeForce GTX 1050 Ti и главное не с диагональю 15.6. В какой ценовой категории вышли подобные ноутбуки?*<br>
*5.3. Что дешевле? В среднем дешевле ноутбуки с CPU Intel Core i7 7700HQ 2.8GHz или с Intel Core i7 7600U 2.8GHz?*<br>

**Задача 6.** <br>
*6.1. Найдите самый легкий ноутбук.* <br>
*!!!Но обратите внимание на тип и представление данных в признаке Weight, если что, замените в строке 'kg' на пустую строку через метод .str.replace()!!!*

# Семинар 3. Изменение таблиц в Pandas <br>
**Задача 1.** <br>
```
1. Скачать данные по ссылке https://gbcdn.mrgcdn.ru/uploads/asset/5348083/attachment/7cfe8f43668ef0df20c7a6554dca48c6.csv
2. Считать данные с помощью pandas.
3. Вывести на экран первые 5 строк.
4. Посмотреть на описание признаков и на их содержание.
```
*1.1 Создать новый признак Cpu_Company, который будет содержать только название фирмы, которая произвела CPU.* <br>
*1.2 Создать новый признак Memory_Amount, который будет содержать только количество Gb памяти без указания типа носителя.* <br>
*1.3 Создать новый признак Memory_Type, который будет содержать только тип носителя (HDD/SDD/др.).* <br>
*1.4 Удалите признаки Memory и ScreenResolution.*

**Задача 2.** <br>
*2.1 Создайте признак SSD, который изначально равен 0.* <br>
*2.2 Поставьте в признаке SSD 1, если ноутбук действительно с типом носителя SSD.* <br>
*2.3 Уберите в признаке Weight значения 'kg' и поменяйте его тип данных на вещественный.* <br>

**Задача 3.** <br>
*Создайте датафрейм с клиентами:*

```
clients = pd.DataFrame({
 'client_id': [45, 32, 67, 33, 43],
 'laptop_id': [506, 398, 710, 120, 1999]
})
```
*!!!laptop_id - это индексы датафрейма с ноутбуками!!!* <br>
*3.1 Присоедините к таблице clients данные по ноутбукам через метод join.* <br>
*3.2 Присоедините к таблице clients данные по ноутбукам через метод merge.* <br>
Это нужно, чтобы понимать, какие ноутбуки покупались клиентами!

**Задача 4.** <br>
*Составьте несколько сводных таблиц.*
*4.1 Найдите среднюю стоимость ноутбуков в зависимости от компании производителя Отсортируйте от меньшей стоимости к большей.* <br>
*4.2 Найдите минимальную, среднюю и максимальную стоимости ноутбуков в зависимости от производителя процессора.* <br>
*4.3 Постройте таблицу с подсчетом количества ноутбуков в данных в зависимости от производителя CPU и ОЗУ.* <br>
*4.4 Постройте таблицу с подсчетом средней стоимости ноутбуков в данных в зависимости от операционной системы и GB памяти.* <br>

**Задача 5.** <br>
*Ответьте на несколько вопросов*
*5.1 Ноутбуков каких компаний и с каким процессором больше?* <br>
*5.2 С каким типом памяти и с каким объемом памяти больше ноутбуков?* <br>

# Семинар 4. Визуальный анализ данных. <br>
**Задача 1.** <br>
```
1. Скачать данные по ссылке https://drive.google.com/file/d/1MpAdHAl727fO3oW32NO4FpSRhUBUfjfS.
2. Считать данные с помощью pandas.
3. Вывести на экран первые 5 строк.
```

*1.1 Изучите количество памяти с помощью matplotlib.* <br>
```
1. Постройте график.
2. Назовите график.
3. Сделайте именование оси x и оси y.
4. Сделайте выводы.
```

*1.2 Изучите стоимость ноутбуков с помощью matplotlib.* <br>
```
1. Постройте график.
2. Назовите график.
3. Сделайте именование оси x и оси y.
4. Сделайте выводы.
```
*1.3 Изучите вес ноутбуков с помощью matplotlib.* <br>
```
1. Постройте график.
2. Назовите график.
3. Сделайте именование оси x и оси y.
4. Сделайте выводы.
```


**Задача 2.** <br>
*2.1 Создайте признак SSD, который изначально равен 0.* <br>
```
1. Постройте график.
2. Сделайте выводы.
```
*2.2 Изучите распределение компаний производителей.* <br>
```
1. Постройте график.
2. Сделайте выводы.
```
*2.3 Изучите распределение операционной системы.* <br>
```
1. Постройте график.
2. Сделайте выводы.
```
*2.4 Изучите распределение компаний производителей CPU.* <br>
```
1. Постройте график.
2. Сделайте выводы.
```

**Задача 3.** <br>
Изучите взаимосвязь компаний производителей ноутбуков и компаний производителей процессоров, используя сложенную или многорядовую столбчатую диаграмму. <br> *!!!Процессоры от Samsung не изучайте!!!*
*3.1 Постройте график в абсолютных величинах.* <br>
*3.2 Постройте график в относительных величинах.* <br>

**Задача 4.** <br>
*4.1 Изучите взаимосвязь стоимости ноутбука и компании производителя процессора.* <br>
```
1. Постройте график.
2. Назовите график.
3. Сделайте именование оси x и оси y.
4. Сделайте выводы.
```
*4.2 Изучите взаимосвязь стоимости ноутбука и типа носителя памяти.* <br>
```
1. Постройте график.
2. Назовите график.
3. Сделайте именование оси x и оси y.
4. Сделайте выводы.
```

*4.3 Изучите взаимосвязь стоимости ноутбука и кол-ва оперативной памяти.* <br>
```
1. Постройте график.
2. Назовите график.
3. Сделайте именование оси x и оси y.
4. Сделайте выводы.
```

*4.4 Изучите взаимосвязь стоимости ноутбука и компании производителя.* <br>
```
1. Постройте график.
2. Назовите график.
3. Сделайте именование оси x и оси y.
4. Сделайте выводы.
```

**Задача 5.** <br>
Постройте матрицу корреляций для таблицы.

**Задача 6.** <br>
Визуализируйте геоданные.