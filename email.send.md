# $email.send

Метод $db.Send() отправляет письмо.

## Синтаксис

```
$db.send(message)
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

## Возвращаемые значения

null или описание ошибки в виде строки.