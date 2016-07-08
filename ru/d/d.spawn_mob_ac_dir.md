# d.spawn_mob_ac_dir()
Функция **d.spawn_mob_ac_dir** призывает монстра или NPC в подземелье, повернутого в определенную сторону на определенное количество градусов.

## Параметры функции
### mob_vnum
Тип *number*. **Обязательный параметр**. ID монстра.

### x
Тип *number*. **Обязательный параметр**. Локальная координата по оси X без двух нулей на конце, куда будет призван монстр.

### y
Тип *number*. **Обязательный параметр**. Локальная координата по оси Y без двух нулей на конце, куда будет призван монстр.

### direction
Тип *number*. **Обязательный параметр**. Направление в градусах по часовой стрелке, куда будет смотреть монстр. Направление может быть от `0` до `359`. Если параметр равен `-1`, то направление будет задано случайно.

## Возвращаемые значения
### mob_vid
Тип *number*. VID призванного монстра. Если во время призыва произошла какая-то ошибка, то это значение не возвращается вообще.

## Примечания
Функция может быть вызвана анонимно.

Существует аналог этой функции, который позволяет задать направление в упрощенном формате &mdash; [d.spawn_mob_dir](../d/d.spawn_mob_dir.md)().

Функция может быть полезна в том случае, если необходимо призвать NPC или монстра, которые не могут двигаться, чтобы задать им направление. Например, чтобы они не стояли лицом к стене. Использование этой функции для призыва монстров и NPC, которые могут двигаться, нецелесообразно.

Эта функция работает только в подземельях.