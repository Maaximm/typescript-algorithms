# Бинарный поиск

В информатике бинарный поиск, также известный как полуинтервальный поиск, логарифмический поиск или двоичное дробление - это алгоритм 
поиска который находит позицию целевого значения в отсортированном массиве. Двоичный поиск сравнивает целевое значение со средним
элементом массива; если они неравны, половина, в которой цель не может лежать устранена, и поиск продолжается на оставшейся половине. 
Если поиск заканчивается тем, что оставшаяся половина остается пустой, цель не в массиве.

![Binary Search](https://upload.wikimedia.org/wikipedia/commons/8/83/Binary_Search_Depiction.svg)

## Сложность

**Временная сложность**: `O (log (n))` - поскольку мы разделяем область поиска на два для каждой
следующей итерации.

## Ссылкт

- [Wikipedia](https://en.wikipedia.org/wiki/Binary_search_algorithm)
- [YouTube](https://www.youtube.com/watch?v=P3YID7liBug&index=29&list=PLLXdhg_r2hKA7DPDsunoDZ-Z769jWn4R8)