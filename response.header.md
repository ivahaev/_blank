# $response.header

Method `$response.header()` sets HTTP header

## Syntax

```
$response.header(name, value)
```

## Parameters

### name
Header name (string)

### value
Header value (string)

## Example

```
$response.header('Content-Disposition', 'attachment; filename="sample.txt"')
```