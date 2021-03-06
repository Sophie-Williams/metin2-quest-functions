# pc.have_pos_scroll()
Функция **pc.have_pos_scroll** сообщает, имеется ли у игрока свиток местности с определенными координатами.

## Параметры функции
### x
Тип *number*. **Обязательный параметр**. Серверная координата по оси X. Неизвестно насчет двух нулей на конце.

### y
Тип *number*. **Обязательный параметр**. Серверная координата по оси Y. Неизвестно насчет двух нулей на конце.

### radius
Тип *number*. **Обязательный параметр**. Радиус поиска. Если указать этот параметр равным, допустим, `15`, функция будет искать свитки местности с координатами &plusmn; 15.

## Возвращаемые значения
### has_scroll
Тип *boolean*. Если один из параметров не является числом или если в инвентаре игрока нет определенного свитка местности, то возвращается `false`; если свиток местности присутствует, то возвращается `true`.

## Примечания
Функция **не** может быть вызвана анонимно.

Функция ищет предметы с `type` == `3`, `subtype` == `1` и `value0` == `0` или `2`, а не по vnum или каким-то другим параметрам.