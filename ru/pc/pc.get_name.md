# pc.get_name()
Функция **pc.get_name** сообщает имя игрока, вызвавшего функцию.

## Возвращаемые значения
### player_name
Тип *string*. Имя игрока.

## Примечания
Функция **не** может быть вызвана анонимно.

Если в имени игрока присутствуют квадратные скобки, например `[GM]terron`, то при вызове функции в функции [say](../global/say.md)() (и любой другой, основанной на этой функции) содержимое квадратных скобок будет вырезано, то есть останется лишь `terron`.