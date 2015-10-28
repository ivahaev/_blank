# access

Contains access objects (array of access objects). Used for describe permissions for users and roles

### Example

```
    "access": [
        {
            "role": "00000000-0000-0000-0000-000000000000",
            "permissions": "crud"
        },
        {
            "role": "client",
            "permissions": "c|r"
        },
        {
            "role": "manager",
            "permissions": "r"
        }
    ]
```
