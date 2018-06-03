# Целые числа (int)
```python
num = 13
print(num)

num = 0
print(num)

num = -10
print(num)
```
13
0
-10

```python
num = 100_000_000
print(num)
```
100000000

## Встроенная функция **type**

```python
num = 13
print(type(num))
```
<class 'int'>

## Вещественные числа (float)

```python
num = 13.4
print(num)

num = 0.0
print(num)

num = -10.2
print(num)
```
13.4
0.0
-10.2

```python
num = 100_000.000_001
print(num)
```
100000.000001

```python
# 1.5 умножить на 10 в степени 2
num = 1.5e2
print(num)
```
150.0

## Конвертация типов:

```python
num = 150.2
print(type(num))
```
<class 'float'>

```python
num = int(num)
print(num, type(num))

num = float(num)
print(num, type(num))
```
150 <class 'int'>
150.0 <class 'float'>

## Комплексные числа (complex)
```python
num = 14 + 1j

print(type(num))
print(num.real)
print(num.imag)
```
<class 'complex'>
14.0
1.0
### Модуль **decimal** для работы с вещественными числами с фиксированной точностью

### Модуль **fractions** для работы с рациональными числами

## Основные операции с числами
### Сложение:

```python
1 + 1
```
2
```python
1 + 2.0
```
3.0

### Вычитание:

```python
10 - 1
```
9
```python
4.2 - 1
```
3.2
### Деление:
```python
10 / 2
```
5.0
### Делить на 0 нельзя:
```python
2 / 0
---------------------------------------------------------------------------
ZeroDivisionError                         Traceback (most recent call last)
<ipython-input-11-ae0c5d243292> in <module>()
----> 1 2 / 0

ZeroDivisionError: division by zero
```

### Умножение:
```python
4 * 5.25
```
21.0
### Возведение числа в степень:
```python
2 ** 4
```
16
### Целочисленное деление:
```python
10 // 3
```
3
### Остаток от деления:
```python
10 % 3
```
1
### Порядок операций в выражениях с числами:
```python
print(10 * 3 + 3)
print(10 * (3 + 3))
```
33
60
### Побитовые операции:
```python
x = 4
y = 3

print("Побитовое или:", x | y)
print("Побитовое исключающее или:", x ^ y)
print("Побитовое и:", x & y)
print("Битовый сдвиг влево:", x << 3)
print("Битовый сдвиг вправо:", x >> 1)
print("Инверсия битов:", ~x)
```
Побитовое или: 7
Побитовое исключающее или: 7
Побитовое и: 0
Битовый сдвиг влево: 32
Битовый сдвиг вправо: 2
Инверсия битов: -5

### Задача: найти расстояние между двумя точками в декартовых координатах.
distance

### Решение:
```python
x1, y1 = 0, 0
x2 = 3
y2 = 4

distance = ((x2 - x1) ** 2 + (y2 - y1) ** 2) ** 0.5
print(distance)
```
5.0
### Меняем местами значения 2-х переменных:
```python
a = 100
b = 200
print(a, b)

a, b = b, a
print(a, b)
```
100 200
200 100
### Вместо x, y = 0, 0
```python
x = y = 0
x += 1

print(x)
print(y)
```
1
0
### Но нужно помнить об отличии изменяемых (mutable) и неизменяемых (immutable) типов:
```python
x = y = []
x.append(1)
x.append(2)

print(x)
print(y)
```
[1, 2]
[1, 2]
В этом видео:

Поговорили о базовых численных типах в Python
Рассмотрели математические операции с численными типами
Узнали о конвертации типов
Затронули тему изменяемых и неизменяемых объектов в Python
 