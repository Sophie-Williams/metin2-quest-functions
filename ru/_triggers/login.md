# login
Триггер **login** срабатывает, когда игрок входит в игру или телепортируется.

## Примечания
Утверждение &laquo;срабатывает при входе в игру&raquo; не совсем корректно. На самом деле, триггер срабатывает по завершении окна загрузки персонажа, будь то телепортация или первый вход в игру.

При вызове функции [say](../global/say.md)() с помощью данного триггера использовать функцию [wait](../selfmade/wait.md)() не получится &mdash; она не сработает. Чтобы добиться желаемого функционала, надо в данном триггере вызвать функцию [timer](../global/timer.md)() со вторым параметром, равным `1`, а затем уже вызывать квестовое окно через триггер [timer](../_triggers/timer.md).