# $response.excel

Method `$response.excel()` renders report by provided template and writes it file into the body stream in a efficient way.

## Syntax

```
$response.excel(template, context[, reportName])
```

## Parameters

### template
Path to template `.xlsx` file (string). Example template's content:

![Sample document image](./template.png)

### context
Data to render (Javascript object)

### reportName
Filename for download (string, optional)

## Return value
`null` if success or string error if error.

## Example

```
$response.excel("./template.xlsx", {"name": "John Smith"}, "report.xlsx")
```