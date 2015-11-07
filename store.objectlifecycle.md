# objectLifeCycle

Optional property `objectLifeCycle` describes hooks executed when events fired on object life cycle.   
Events are:  
* [willCreate](./store.objectlifecycle.willcreate.html)
* [didCreate](./store.objectlifecycle.didcreate.html)
* [willSave](./store.objectlifecycle.willsave.html)
* [didSave](./store.objectlifecycle.didsave.html)
* [willRemove](./store.objectlifecycle.willremove.html)
* [didRemove](./store.objectlifecycle.didremove.html)
* [didRead](./store.objectlifecycle.didread.html)

## Syntax  

```
    "objectLifeCycle": {
        "willCreate": {},
        "didCreate": {},
        "willSave": {},
        "didSave": {},
        "willRemove": {},
        "didRemove": {},
        "didRead": {}
    }
```  

## Params

### _id   

Идентификатор объекта (строка)  

### store  

Идентификатор хранилища (строка, опционально). По умолчанию используется текущее хранилище. 

## Return value  

`null` или описание ошибки в виде строки.
