# $response.xml

Method `$response.xml()` sets HTTP response code and returns data as XML. Also it sets **Content-Type** HTTP header to **'application/xml'**.

## Syntax

```
$response.xml(code, data)
```

## Parameters

### code
HTTP response code (int)

### data
Response data (string). You need to serialize date manually.

## Examples

```
$response.xml(200, '<data></data>')
```
