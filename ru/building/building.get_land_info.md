# building.get_land_info()
Функция **building.get_land_info** сообщает информацию о земле гильдии.

## Параметры функции
### land_id
Тип *number*. **Обязательный параметр**. ID земли, информацию о которой необходимо получить.

## Возвращаемые значения
### price
Тип *number*. Стоимость земли.

### guild_id
Тип *number*. Владелец земли. Если землей никто не владеет, то значение будет равно `0`.

### level_limit
Тип *number*. Минимальный уровень гильдии, необходимый для покупки земли.

## Примечания
Функция может быть вызвана анонимно.

Изменять цену и минимальный уровень нужно в таблице `player.land`.

Возвращаемые значения являются опциональными для покупки земли гильдией. Это значит, что сервер не будет выдавать какой-либо ошибки, если гильдия, чей уровень ниже, чем возвращаемый параметр [level_limit](#level_limit), попытается купить землю через функцию [building.set_land_owner](../building/building.set_land_owner.md)(). Для этого надо использовать дополнительные проверки.