# Store Description

Introduction to store parameters must be here.

## Total list of parameters
* [type](#type)
* [access](#access)
* [menuGroup](#menuGroup)
* i18n
* icon
* filters
* objectLifeCycle
* storeLifeCycle
* printTemplates ???
* formGroupsOrder
* states
* actions
* storeActions
* entries
* displayOrder
* display
* html
* labels
* tableColumns
* disableAutoSelect
* orderBy
* config
* listViewOnly
* fullWidth
* disablePartialLoad
* httpHooks
* navLinkStyle
* navLinkActiveStyle
* navLinkHoverStyle
* tasks
* props




<a name="type"></a>


<a name="access"></a>
## access
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

<a name="menuGroup"></a>
## menuGroup
Points to menu group to place store (string).

### Example

```
    "menuGroup": "Configuration"
```