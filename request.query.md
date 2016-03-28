# $request.query

`$request.query` is used to return the url query values.

## Example

Request URL is:
`?id=1234&name=Manu`
To extract query values, do following
```
var id = $request.query['id'];
if (id != null) {
    console.log(id[0]);
}
var name = $request.query['name'];
if (name != null) {
    console.log(name[0]);
}


```