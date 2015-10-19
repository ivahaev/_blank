# $response.Redirect

Method `$response.Redirect` returns a HTTP redirect to the specific location.

## Syntax

```
$response.Redirect(code, location)
```

## Parameters

### code
HTTP code to set (int)

### location
Location to redirect (string)


## Examples

```
$response.Redirect(303, '/redirected.html')
```
