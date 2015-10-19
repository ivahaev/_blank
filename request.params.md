# $request.Params

`$request.Params` used to return URL parameters configured in HTTP hook.

## Example

```
"httpHooks": [
    {
        "uri": "example/:id",
        "method": "GET",
        "script": "console.log($request.Params['id'])"
    }
]
```