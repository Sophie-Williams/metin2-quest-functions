# d.set_regen_file()
Функция **d.set_regen_file** подключает regen-файл.

## Параметры функции
### path
Тип *string*. **Обязательный параметр**. Путь до regen-файла. Можно указать как полный путь, так и относительный. Относительный путь должен указываться относительно директории, в которой лежит игровое ядро.

## Примечания
Функция может быть вызвана анонимно.

В отличие от функции [d.regen_file](../d/d.regen_file.md)(), подключенный через эту функцию regen-файл будет призывать монстров сколько угодно раз согласно настройкам внутри подключенного файла.

Эта функция работает только в подземельях.