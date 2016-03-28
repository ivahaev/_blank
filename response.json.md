# $response.json

Method `$response.json()` sets HTTP response code and returns data as JSON. Also it sets **Content-Type** HTTP header to **'application/json'**.

## Syntax

```
$response.json(code, data)
```

## Parameters

### code
HTTP response code (int)

### data
Response data (object|array|string). Data will serialized automatically.

## Examples

```
$response.json(200, {result: 'SUCCESS'})
```
```
$response.json(404, 'not found')
```
