# pc.warp_local()
Функция **pc.warp_local** телепортирует игрока на определенные локальные координаты.

## Параметры функции
### local_x
Тип *number*. **Обязательный параметр**. Локальная координата по оси X с двумя нулями на конце.

### local_y
Тип *number*. **Обязательный параметр**. Локальная координата по оси Y с двумя нулями на конце.

### map_index
Тип *number*. **Обязательный параметр**. Индекс локации, куда будет сделана телепортация.

## Примечания
Функция **не** может быть вызвана анонимно.

Телепортация во время торга невозможна. Перед вызовом этой функции используйте функцию [pc.can_warp](../pc/pc.can_warp.md)() для проверки того, может ли игрок сделать телепортацию.