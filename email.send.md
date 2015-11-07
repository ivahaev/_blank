# email.send

Метод `email.send()` отправляет письмо.

## Синтаксис

```
email.send(message[, callback])
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

### callback
Функция, выполняемая после отправки письма. Функция принимает первым аргументом ошибку в виде строки.

## Возвращаемые значения

`null`, в случае успешного выполнения, или описание ошибки в виде строки.