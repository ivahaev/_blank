# $response.HTML

Method `$response.HTML()` sets HTTP response code and returns data as HTML. Also it sets **Content-Type** HTTP header to **'text/html'**.

## Syntax

```
$response.HTML(code, data)
```

## Parameters

### code
HTTP response code (int)

### data
Response data (string).

## Example

```
$response.HTML(200, '<html><body><h1>Hi there!</h1></body></html>')
```
