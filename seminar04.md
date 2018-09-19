# Семинар 4 (14.09.2018)
## Библиотека `math`
* https://docs.python.org/3/library/math.html

Библиотека содержит функции для математических вычислений с целыми и действительными числами.

Пример:
```python
>>> import math
>>> math.exp(1)
2.718281828459045
>>> math.factorial(100)
93326215443944152681699238856266700490715968264381621468592963895217599993229915608941463976156518286253697920827223758251185210916864000000000000000000000000
```

## Рациональные числа (`fractions`)
* https://docs.python.org/3/library/fractions.html

```python
>>> from fractions import Fraction
>>> a = Fraction('1/3')  # Обратите внимание, что передаём строку
>>> b = Fraction(5, 7)  # Но можно и отдельно числитель и знаменатель
>>> a + b  # Можно производить привычные действия
Fraction(22, 21)
>>> c = Fraction('1')
>>> c / 3  # Операции с дробями осуществляются точно
Fraction(1, 3)
>>> a.numerator  # Числитель
1
>>> a.denominator  # Знаменатель
3
>>> d = Fraction('4/2')  # Дроби автоматически сокращаются
>>> d
Fraction(2, 1)
```


## Работа с комплексными числами
* https://en.wikipedia.org/wiki/Complex_number
* https://python-reference.readthedocs.io/en/latest/docs/complex/

```python
>>> 1j  # Мнимая единица
1j
>>> 1j ** 2  # В квадрате даёт -1
(-1+0j)
>>> x = 2.5 - 4j
>>> x.imag  # Мнимая часть
-4.0
>>> x.real  # Действительная часть
2.5
```

Аналог библиотеки `math` для комплексных чисел — `cmath`:
```python
>>> import cmath
>>> cmath.exp(1j * cmath.pi)  # Тождество Эйлера
(-1+1.2246467991473532e-16j)
```
