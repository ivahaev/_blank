# objectLifeCycle.didRemove

Optional property `didRemove` contains **Javascript** scenario that will executed after object was removed from store.  

Scenario has access to this object in `Object` property of [$db](./db.html) module. It's good chance to [notifying users](./db.notify.html), performing related changes in [$db](./db.html), sending [email](./email.html) or performing [http request](./js.http.html). 
