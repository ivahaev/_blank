# i18n.get

Метод `i18n.get()` возвращает соответствующую фразу.  

## Синтаксис  

```
i18n.get(path[, locale])
```  

## Параметры

### path
Путь к фразе (строка) в точечной нотации. Первым сегментом следует указывать название хранилища. Для фразы из хранилища `_commonSettings`, следует использовать `$settings`  

### locale    
Идентификатор локали (строка, опционально). Если параметр опущен, будет использована заданная локаль по умолчанию.  

## Возвращаемое значение

Строка, в случае успешного выполнения, или `undefined`, если строка не найдена.  
