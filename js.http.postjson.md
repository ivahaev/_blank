# http.postJSON

Метод `http.postJSON()` выполняет POST запрос на указанный URL, отправляя переданный JSON объект.

## Синтаксис

```
http.postJSON(uri, params)
```

## Параметры

### uri
Адрес запроса (строка). Слэши следует экранировать.

### params
Данные для выполнения запроса. 

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

Если во время выполнения запроса произошла ошибка, её значение будет прописано в результирующем объекте в параметре `error`.

## Пример  

```
var params = {
    param: 'yaya.ru',
    param2: 'neya.ru'
};
http.postJSON('http:\/\/yandex.ru', params);
```

