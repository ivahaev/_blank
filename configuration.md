# Configuration

Настройка платформы производится в текстовом JSON файле, в котором описывается как структура данных, так и его представление в браузере. Вся бизнес логика описывается скриптами на языке Javascript. Имеется хорошо документированное [JS API](js_api.html) как для доступа данным, так и для взаимодействия с внешним миром.   

Описание полей конфигурации одного хранилища приложения:  

```
{
    "users": {
        "type": "directory",
        "menuGroup": "config",
        "i18n": {
            "ru": {
                "singularLocal": "Пользователь",
                "singularAccusativeLocal": "Пользователя",
                "pluralLocal": "Пользователи",
                "pluralGenitiveLocal": "Пользователей"
        },
            "en": {
                "singularLocal": "User",
                "singularAccusativeLocal": "User",
                "pluralLocal": "Users",
                "pluralGenitiveLocal": "Users"
        },
        "formGroupsOrder": [
            "Права доступа",
            "Финансовая информация",
            "Личные данные"
        ],
        "access": [
            {
                "role": "00000000-0000-0000-0000-000000000000",
                "permissions": "crud"
            }
        ],
        "actions": [
            {
                "_id": "activate",
                "localName": "Включить",
                "multi": false,
                "script": "\n$db.Object.isActive = true;\n$db.Set($db.Object);",
                "conditions": [
                    {
                        "property": "isActive",
                        "value": true,
                        "operator": "!="
                    },
                    {
                        "property": "_id",
                        "value": "00000000-0000-0000-0000-000000000000",
                        "operator": "!="
                    }
                ]
            },
            {
                "_id": "deactivate",
                "localName": "Заблокировать",
                "icon": "material-icons text md-16 block",
                "multi": false,
                "script": "\n$db.Object.isActive = false;\n$db.Set($db.Object);",
                "conditions": [
                    {
                        "property": "isActive",
                        "value": true,
                        "operator": "="
                    },
                    {
                        "property": "_id",
                        "value": "00000000-0000-0000-0000-000000000000",
                        "operator": "!="
                    }
                ]
            }
        ],
        "labels": [
            {
                "text": "Активен",
                "color": "#5cb85c",
                "showInList": 1,
                "show": [
                    {
                        "property": "isActive",
                        "value": true,
                        "operator": "="
                    }
                ]
            },
            {
                "text": "Отключен",
                "color": "#b85c5c",
                "showInList": 1,
                "show": [
                    {
                        "property": "isActive",
                        "value": true,
                        "operator": "!="
                    }
                ]
            }
        ],
        "props": {
            
        }
    }
}
```