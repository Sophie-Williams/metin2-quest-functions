# d.get_kill_stone_count()
Функция **d.get_kill_stone_count** сообщает количество разрушенных игроками камней метина за всё время нахождения в подземелье.

## Параметры функции
### empty_parameter1
Тип *number*. **Обязательный параметр**. Параметр, который ни на что не влияет (возможно, это баг).

### empty_parameter2
Тип *number*. **Обязательный параметр**. Параметр, который ни на что не влияет (возможно, это баг).

## Возвращаемые значения
### kill_count
Тип *number*. Количество разрушенных камней метина. Если параметры [empty_parameter1](#empty_parameter1) и [empty_parameter2](#empty_parameter2) не определены, не являются числами или если функция вызвана вне подземелья, то возвращается `0`.

## Примечания
Функция может быть вызвана анонимно.

В качестве параметров необходимо указать совершенно любые числа, например `d.get_kill_stone_count(1, 1)`. Эти параметры ни на что не повлияют, но если их не указать, то функция вернет `0`. Это баг.

Эта функция работает только в подземельях.