# Filters

```
"filters": {
    "filterName1": {
        // filter1 description
    },
    "filterName2": {
        // filter2 description
    }
    ...
}
```

## Filter description structure:

```
{
    "label": "Label for using in browser form",
    "display": "Type of display such in props. Allowed: textInput, searchBox, select, masked, dateRange",
    "placeholder": "Placeholder for display==textInput",
    "conditions": "Array of conditions to compare with",
    "searchBy": "Only for display==searchBox. Array of props for search in store",
    "store": "Only for display==searchBox. Store for search",
    "filterBy": "WTF???",
    "values": "Only for display==select. Values with labels for select",
    "mask": "Only for display==masked"
}
```

## Conditions

```
{
    "property": "Property to compare with search string",
    "operator": "Operator for comparing"
}
```

### Condition operators

`=` means equals exactly. For strings used no case sensitivity comparison.  
`!=` means no equals exactly. For strings used no case sensitivity comparison.  
`contains` means that search string included in prop's value. For strings used no case sensitivity comparison.  
`>`, `>=`, `<`, `<=` as in Javascript.  

## Example

```
"filters": {
    "textFilter": {
        "label": "Search",
        "display": "textInput",
        "conditions": [
            {
                "property": "name",
                "operator": "contains"
            },
            {
                "property": "address",
                "operator": "contains"
            }
        ]
    },
    "textFilter": {
        "label": "City",
        "display": "searchBox",
        "store": "cities",
        "searchBy": ["name", "fullName"],
        "conditions": [
            {
                "property": "cityId",
                "operator": "="
            }
        ]
    },
    "createdAt": {
        "label": "Created",
        "display": "dateRange",
        "conditions": [
            {
                "property": "createdAt",
                "operator": "contains"
            }
        ]
    }
}
```