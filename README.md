# Алгоритмы и структуры данных на TypeScript.

В этом репозитории содержатся базовые TypeScript-примеры многих популярных алгоритмов и структур данных. Для каждого алгоритма и 
структуры данных есть свой файл README с соответствующими пояснениями и ссылками на материалы для дальнейшего 
изучения (в том числе и ссылки на видеоролики в YouTube).

## Структуры данных

Структура данных (англ. data structure) — программная единица, позволяющая хранить и обрабатывать множество однотипных и/или логически 
связанных данных в вычислительной технике. Для добавления, поиска, изменения и удаления данных структура данных предоставляет некоторый 
набор функций, составляющих её интерфейс.

`A` - Базовый уровень, `B` - Продвинутый уровень

* `A` [Однонаправленный связный список](src/data-structures/linked-list)
* `A` [Двунаправленный связный список](src/data-structures/double-linked-list)
* `A` [Стек](src/data-structures/stack)
* `A` [Очередь](src/data-structures/queue)

## Алгоритмы

Алгоритмы - это наборы команд, способствующие эффективному программированию. Они объясняют, как сортировать записи, искать элементы, 
рассчитывать числовые значения, находить кратчайший путь между двумя точками на карте, определять максимально возможный поток 
информации по сети и т.д.

`A` - Базовый уровень, `B` - Продвинутый уровень

* **Алгоритмы поиска**
* `A` [Линейный поиск](src/algorithms/search/linear-search)
* `A` [Двоичный поиск](src/algorithms/search/binary-search) — поиск в упорядоченном массиве

* **Алгоритмы сортировки**
* `A` [Сортировка пузырьком](src/algorithms/sorting/bubble-sort)

## Асимптопатическая сложность алгоритма

**Асимптопатическая сложность (производительность)** - определяется функцией, которая указывает, насколько ухудшается работа алгоритма 
с усложнением поставленной задачи. Такую функцию записывают в круглых скобках, предваряя прописной буквой О.

![Big O Graphs](./assets/big-o-graph.png)

Ниже представлены часто используемые обозначения в нотации «О» большое, а также сравнение их производительностей на различных размерах входных данных.

| Нотация «О» большое | 10 элементов | 100 элементов | 1000 элементов |
| ------------------- | ------------ | ------------- | -------------- |
| **O(1)**            | 1            | 1             | 1              |
| **O(log N)**        | 3            | 6             | 9              |
| **O(N)**            | 10           | 100           | 1000           |
| **O(N log N)**      | 30           | 600           | 9000           |
| **O(N^2)**          | 100          | 10000         | 1000000        |
| **O(2^N)**          | 1024         | 1.26e+29      | 1.07e+301      |
| **O(N!)**           | 3628800      | 9.3e+157      | 4.02e+2567     |

### Сложности операций в структурах данных

| Структура данных           | Получение | Поиск     | Вставка   | Удаление  | Комментарии |
| -------------------------- | :-------: | :-------: | :-------: | :-------: | :---------- |
| **Массив**                 | 1         | n         | n         | n         |             |
| **Связный список**         | n         | n         | 1         | n         |             |
| **Стек**                   | n         | n         | 1         | 1         |             |
| **Очередь**                | n         | n         | 1         | 1         |             |

### Сложности алгоритмов сортировки

| Наименование               | Лучший случай | Средний случай | Худший случай | Память | Устойчивость | Комментарии |
| -------------------------- | :-----------: | :------------: | :-----------: | :----: | :----------: | :---------- |
| **Сортировка пузырьком**   | n             | n<sup>2</sup>  | n<sup>2</sup> | 1      | Да           |             |