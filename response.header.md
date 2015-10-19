# $response.Header

Method `$response.Header` sets HTTP header

## Syntax

```
$response.Header(name, value)
```

## Parameters

### name
Header name (string)

### value
Header value (string)

## Example

```
$response.Header('Content-Disposition', 'attachment; filename="sample.txt"')
```