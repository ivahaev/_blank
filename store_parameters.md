# Store Description

Introduction to store parameters must be here.

## Total list of parameters
* [type](#type)
* [access](#access)
* menuGroup
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
## type
Describes type of store (string). Takes one of the following values:  
`directory` means that store is a simple directory.  
`process` means that store's objects can have one of the states described in `states` parameter.  
`workspace` used for describing interfaces work spaces.  
`map` contains useful settings.

### Example

```
    "type": "directory"
```

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