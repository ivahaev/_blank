# objectLifeCycle

Optional property `objectLifeCycle` describes hooks executed when events fired on object life cycle.   
Events are:  
* willCreate
* didCreate
* willSave
* didSave
* willRemove
* didRemove
* didRead

## Syntax  

```
    "objectLifeCycle": {
        ["willCreate": {},]
        ["didCreate": {},]
        ["willSave": {},]
        ["didSave": {},]
        ["willRemove": {},]
        ["didRemove": {},]
        ["didRead": {}]
    }
```  

## Params

### _id   

Идентификатор объекта (строка)  

### store  

Идентификатор хранилища (строка, опционально). По умолчанию используется текущее хранилище. 

## Return value  

`null` или описание ошибки в виде строки.
