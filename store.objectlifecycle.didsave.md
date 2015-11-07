# objectLifeCycle.didSave

Optional property `didSave` contains **Javascript** scenario that will executed after object was saved.  

Scenario has access to this object in `Object` property of [$db](./db.html) module. It's good chance to [notify users](./db.notify.html), perform related changes in [$db](./db.html), send [email](./email.html) or make [http request](./js.http.html). 
 
