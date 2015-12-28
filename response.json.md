# $response.JSON

Method `$response.JSON()` sets HTTP response code and returns data as JSON. Also it sets **Content-Type** HTTP header to **'application/json'**.

## Syntax

```
$response.JSON(code, data)
```

## Parameters

### code
HTTP response code (int)

### data
Response data (object|array|string). Data will serialized automatically.

## Examples

```
$response.JSON(200, {result: 'SUCCESS'})
```
```
$response.JSON(404, 'not found')
```
