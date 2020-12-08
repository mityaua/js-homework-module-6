## Задача 6-1

Массив объектов пользователей

#### map

Получи массив имен всех пользователей (свойство `name`) используя
деструктурирующее присваивание для параметра функции `({name})` без пробелов и
переносов на новую строку.

Используй только перебирающие методы массива которые не изменяют (не мутируют)
исходный массив. Т.е. нельзя использовать `for`, `splice`, `push` и т.п.
мутирующие методы.

#### Деструктурирующее присваивание для параметра функции

PS Деструктурирующее присваивание (ДП):

1.  Объект как параметр без ДП

```js
const object = { num: 2 };
function getNum(obj) {
  return obj.num;
}
console.log(getNum(object)); // 2
```

2.  ДП

```js
const object = { num: 2 };
// const num  =  object.num;
const { num } = object;
console.log(num); // 2
```

3.  Объект как параметр c ДП

```js
const object = { num: 2 };
//function getNum (obj) { return obj.num; }
function getNum({ num }) {
  return num;
}
console.log(getNum(object)); // 2
```

## Задача 6-2

Массив объектов пользователей

#### filter

Получи массив объектов пользователей, отобранный по цвету глаз (свойство
`eyeColor`), используя деструктурирующее присваивание для параметра функции
`({eyeColor})` без пробелов и переносов на новую строку.

Используй только перебирающие методы массива которые не изменяют (не мутируют)
исходный массив. Т.е. нельзя использовать `for`, `splice`, `push` и т.п.
мутирующие методы.

#### Деструктурирующее присваивание для параметра функции

PS Деструктурирующее присваивание (ДП):

1.  Объект как параметр без ДП

```js
const object = { num: 2 };
function getNum(obj) {
  return obj.num;
}
console.log(getNum(object)); // 2
```

2.  ДП

```js
const object = { num: 2 };
// const num  =  object.num;
const { num } = object;
console.log(num); // 2
```

3.  Объект как параметр c ДП

```js
const object = { num: 2 };
//function getNum (obj) { return obj.num; }
function getNum({ num }) {
  return num;
}
console.log(getNum(object)); // 2
```

## Задача 6-3

Массив объектов пользователей

#### filter, map

Получи массив имен пользователей (значение свойства `name`) по полу (значение
свойства `gender`).

Используй деструктурирующее присваивание для параметра функции `({name})` без
пробелов и переносов на новую строку.

Используй только перебирающие методы массива которые не изменяют (не мутируют)
исходный массив. Т.е. нельзя использовать `for`, `splice`, `push` и т.п.
мутирующие методы.

## Задача 6-4

Массив объектов пользователей

#### filter и оператор !

Получи массив только неактивных пользователей (отфильтруй по значению свойства
`isActive`)

Используй деструктурирующее присваивание для параметра функции `({isActive})`
без пробелов и переносов на новую строку.

Используй оператор `!`.

Используй только перебирающие методы массива которые не изменяют (не мутируют)
исходный массив. Т.е. нельзя использовать `for`, `splice`, `push` и т.п.
мутирующие методы.

## Задача 6-5

Массив объектов пользователей

#### find

Получи объект пользователя (не массив) по уникальному значению свойства `email`.

Используй деструктурирующее присваивание для параметра функции `({email})` без
пробелов и переносов на новую строку.

Используй только перебирающие методы массива которые не изменяют (не мутируют)
исходный массив. Т.е. нельзя использовать `for`, `splice`, `push` и т.п.
мутирующие методы.

## Задача 6-6

Массив объектов пользователей

#### filter, map и создание анонимных объектов

Получи массив из объектов, которые состоят только из свойств  `name`  и  `email`  тех пользователей, которые попадают в возрастную категорию от  `min`  до  `max`  лет (значение свойства  `age`).

Сравнение, пример

```js
const x = 13;

// num больше 10 ?
const larger = num > 10; // true

// num меньше 100 ?
const smaller = 100 > num; // true

// num находитя между 10 и 100 ?
const between = smaller && larger; // true

```

Создание анонимных объектов:

```js
const arr = Array(3)
  .fill('')
  .map((e,i) => ({['index']: i }));
/* [ { index: 0 }, { index: 1 }, { index: 2 } ] */

```

Используй только перебирающие методы массива которые не изменяют (не мутируют) исходный массив. Т.е. нельзя использовать  `for`,  `splice`,  `push`  и т.п. мутирующие методы.

## Задача 6-7

Массив объектов пользователей

#### reduce

Получи общую сумму баланса (сумму значений свойства  `balance`) всех пользователей.

Используй деструктурирующее присваивание для параметра функции  `{balance}`  без пробелов и переносов на новую строку

Используй только перебирающие методы массива которые не изменяют (не мутируют) исходный массив. Т.е. нельзя использовать  `for`,  `splice`,  `push`  и т.п. мутирующие методы.

## Задача 6-8

Массив объектов пользователей

#### filter, includes и map

Получи массив имен всех пользователей у которых есть друг с заданным именем.

Используй деструктурирующее присваивание для параметра функции  `{friends}`и  `({name})`  без пробелов и переносов на новую строку

Используй только перебирающие методы массива которые не изменяют (не мутируют) исходный массив. Т.е. нельзя использовать  `for`,  `splice`,  `push`  и т.п. мутирующие методы.

## Задача 6-9

Массив объектов пользователей

#### sort и map

Получи массив имен (поле  `name`) людей, отсортированных в зависимости от количества их друзей (поле  `friends`)

Избегаем мутации исходного массива: т.к. метод  `sort`  изменяет (мутирует) исходный массив, то следует сделать копию массива и сортировать уже копию, а не исходный массив.

Копирование массива:

```js
const arr = [1, 3, 5];

// 1
const first = [...arr];

// 2
const second = arr.slice();

// 3
const third = arr.concat();

```

Используй деструктурирующее присваивание для параметра функции  ({name})` без пробелов и переносов на новую строку

Используй только перебирающие методы массива которые не изменяют (не мутируют) исходный массив. Т.е. нельзя использовать  `for`,  `splice`,  `push`  и т.п. мутирующие методы.