# http.get

Метод `http.get()` выполняет GET запрос на указанный URL.

## Синтаксис

```
email.send(message)
```

## Параметры

### message
Объект с необходимыми данными для отправки письма

```
{
    from: "name@domain.com",
    to:"name@domain.com",
    cc:"name@domain.com",
    bcc:"name@domain.com",
    subject: "Hi there",
    body: "This is the very important email!"
}
```

Если не указано поле `from`, будет использовано значение из настроек.  

## Возвращаемые значения

null или описание ошибки в виде строки.