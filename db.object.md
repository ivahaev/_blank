# $db.Object

Свойство `$db.Object` содержит в себе текущий объект. В `willCreate` и `willSave` хуках возможно изменение объекта перед передачей в хранилище. В любом случае, будет выполнена дополнительная валидация объекта после выполнения `willCreate` или `willSave` хука.

Свойство доступно в [экшинах](./store.actions.html) и [хуках objectLifeCycle](./store.objectlifecycle.html)