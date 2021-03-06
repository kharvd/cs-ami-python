# Семинар 5 (19.09.2018)
## Строки
В стандартной библитеке есть много методов для манипуляций со строками: https://docs.python.org/3/library/string.html

Также список можно посмотреть в интерпретаторе с помощью команды `help`:
```python
>>> help(str)
```

## (Псевдо-)случайные числа
* https://docs.python.org/3/library/random.html
* https://ru.wikipedia.org/wiki/%D0%93%D0%B5%D0%BD%D0%B5%D1%80%D0%B0%D1%82%D0%BE%D1%80_%D0%BF%D1%81%D0%B5%D0%B2%D0%B4%D0%BE%D1%81%D0%BB%D1%83%D1%87%D0%B0%D0%B9%D0%BD%D1%8B%D1%85_%D1%87%D0%B8%D1%81%D0%B5%D0%BB

```python
>>> import random
>>> random.randint(1, 10)  # Случайное целое число от 1 до 10 (включительно)
6
>>> random.random()  # Случайное вещественное число от 0 до 1
0.21869684306305814
>>> random.seed(1)  # Задать начальное состояние генератора — от него полностью зависит, какие числа будут генерироваться
>>> random.randint(1, 10)
3
>>> random.randint(1, 10)
10
>>> random.randint(1, 10)
2
>>> random.seed(1)  # Инициализируем генератор тем же числом и получаем точно такую же "случайную" последовательность
>>> random.randint(1, 10)
3
>>> random.randint(1, 10)
10
>>> random.randint(1, 10)
2
```

## Дата и время
* https://docs.python.org/3/library/time.html
* https://docs.python.org/3/library/datetime.html
* https://docs.python.org/3/library/calendar.html

## Файловый ввод-вывод
* https://docs.python.org/3/tutorial/inputoutput.html

## Сторонние библиотеки
* https://pypi.org/project/pip/
### `requests`
* http://docs.python-requests.org/en/master/
* https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol
