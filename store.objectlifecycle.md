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
        "willCreate": "",
        "didCreate": "",
        "willSave": "",
        "didSave": "",
        "willRemove": "",
        "didRemove": "",
        "didRead": ""
    }
```  

Each hook can contains Javascript scenario that will executed when corresponding event fired.  