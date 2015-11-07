# objectLifeCycle.didCreate

Optional property `didCreate` contains **Javascript** scenario that will executed after fresh object was saved.  

Scenario has access to this object in `Object` property of [$db](./db.html) module. It's good chance to notifying users, performing related changes in db, sending email or performing http request. 

You can return `false` or string describe of the error to break creating object.  

After execution will perform additional validating of created object.  