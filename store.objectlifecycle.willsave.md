# objectLifeCycle.willSave

Optional property `willSave` contains **Javascript** scenario that will executed right before existing object will be saved.  

Scenario has access to this object in `Object` property of [$db](./db.html) module. It's good chance to modify and validate object before saving. 

You can return `false` or string describe of the error to break saving object.  

After execution will perform additional validating of object.  
