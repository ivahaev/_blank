# objectLifeCycle.didCreate

Optional property `didCreate` contains **Javascript** scenario that will executed after fresh object was saved.  

Scenario has access to this object in `Object` property of [$db](./db.html) module. It's good chance to notifying users, performing related changes in db, sending email or performing http request. 
