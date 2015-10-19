# $request.Params

`$request.Params` used to return URL parameters configured in HTTP hook.

## Example

```
"httpHooks": {
    "example/:id": {
        "method": "GET",
        "script": "console.log($request.Params['id'])"
    }
}
```