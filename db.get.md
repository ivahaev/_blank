# $db.get

Метод `$db.get()` возвращает объект из хранилища.

## Синтаксис

```
$db.get(_id, store)
```

## Параметры

### _id
Идентификатор объекта (строка)

### store
Идентификатор хранилища (строка). Для получения объекта из вложенного хранилища, используется следующий синтаксис: `[store].nestedStore`, где **nestedStore** - идентификатор вложенного хранилища.

### Возвращаемые значения
Запрашиваемый объект, или `null` в случае ошибки, или если объект не найден
