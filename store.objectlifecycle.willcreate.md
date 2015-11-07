# objectLifeCycle.willCreate

Optional property `willCreate` contains **Javascript** scenario that will executed right before fresh object will be saved.  

Scenario has access to this object in `Object` property of `$db` module. It's good chance to modify and validate created object before saving. 

You can return `false` or string describe of the error to break creating object.  

After execution will perform additional validating of created object.  
