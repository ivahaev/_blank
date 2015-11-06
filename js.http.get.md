# http.get

Метод `http.get()` выполняет GET запрос на указанный URL.

## Синтаксис

```
http.get(uri[, params])
```

## Параметры

### uri
Адрес запроса (строка). Слэши следует экранировать.

### params
Объект с необходимыми данными для выполнения запроса. Если в `uri` уже будет закодирован один из параметров в `params`, он будет перезаписан.

```
{
    param: "value"
}
```

## Возвращаемые значения

Объект вида:

```
{
    header: {
        header1: ['value'],
        header2: ['value2', 'value3']
    },
    statusCode: 200,
    body: 'RESULT'
}
```

## Пример  

```
var params = {
    param: 'yaya.ru',
    param2: 'neya.ru'
};
http.get('http:\/\/yandex.ru?param=ya.ru', params);
```

Будет выполнен запрос на `http://yandex.ru?param=yaya.ru&param2=neya.ru`  
