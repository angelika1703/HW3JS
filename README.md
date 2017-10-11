# Типы данных в Javascript

## Число «number»

```
var n = 123;
n = 12.345;
```
Единый тип *число* используется как для целых, так и для дробных чисел.

Существуют специальные числовые значения `Infinity` (бесконечность) и `NaN` (ошибка вычислений).

Например, бесконечность `Infinity` получается при делении на ноль:

```
alert( 1 / 0 ); // Infinity
```

Эти значения формально принадлежат типу «число», хотя, конечно, числами в их обычном понимании не являются.

Особенности работы с числами в JavaScript разобраны в главе [Числа](https://learn.javascript.ru/number).

## Строка «string»

```
var str = "Мама мыла раму";
str = 'Одинарные кавычки тоже подойдут';
```

**В JavaScript одинарные и двойные кавычки равноправны.** Можно использовать или те или другие.

**Тип *символ* не существует, есть только *строка*.**

В некоторых языках программирования есть специальный тип данных для одного символа. Например, в языке С это `char`. В JavaScript есть   только тип «строка» `string`. Что, надо сказать, вполне удобно.

Более подробно со строками мы познакомимся в главе [Строки](https://learn.javascript.ru/string).

## Булевый (логический) тип «boolean»

У него всего два значения: `true` (истина) и `false` (ложь).

Как правило, такой тип используется для хранения значения типа да/нет, например:

```
var checked = true; // поле формы помечено галочкой
checked = false;    // поле формы не содержит галочки
```

О нём мы поговорим более подробно, когда будем обсуждать логические вычисления и условные операторы.

## Специальное значение «null»

Значение `null` не относится ни к одному из типов выше, а образует свой отдельный тип, состоящий из единственного значения `null`:

```
var age = null;
```

В JavaScript `null` не является «ссылкой на несуществующий объект» или «нулевым указателем», как в некоторых других языках. Это просто специальное значение, которое имеет смысл «ничего» или «значение неизвестно».

В частности, код выше говорит о том, что возраст `age` неизвестен.

## Специальное значение «undefined»

Значение `undefined`, как и `null`, образует свой собственный тип, состоящий из одного этого значения. Оно имеет смысл «значение не присвоено».

Если переменная объявлена, но в неё ничего не записано, то её значение как раз и есть `undefined`:

```
var x;
alert( x ); // выведет "undefined"
```

Можно присвоить `undefined` и в явном виде, хотя это делается редко:

```
var x = 123;
x = undefined;

alert( x ); // "undefined"
```

В явном виде `undefined` обычно не присваивают, так как это противоречит его смыслу. Для записи в переменную «пустого» или «неизвестного» значения используется `null`.

## Объекты «object»

Первые 5 типов называют *«примитивными»*.

Особняком стоит шестой тип: *«объекты»*.

Он используется для коллекций данных и для объявления более сложных сущностей.

Объявляются объекты при помощи фигурных скобок `{...}`, например:

```
var user = { name: "Вася" };
```





