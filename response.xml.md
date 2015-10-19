# $response.XML

Method `$response.XML` sets HTTP response code and returns data as XML.

## Syntax

```
$response.XML(code, data)
```

## Parameters

### code
HTTP response code (int)

### data
Response data (string). You need to serialize date manually.

## Examples

```
$response.XML(200, '<data></data>')
```
