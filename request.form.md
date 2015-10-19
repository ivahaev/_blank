# $request.Form

`$request.Form` contains POST form. Available for HTTP POST hooks.

From data kept in `$request.Form.Value` object as array of strings. For example, to get form field value **siteId** need to do following:

```
var siteId = $request.Form.Value['siteId'];
if (siteId != null) {
    console.log(siteId[0])
}
```