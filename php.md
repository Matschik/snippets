# PHP

## Convert "JSON string without double quotes" to "JSON string with double quotes"
```php
$jsonStringWithDoubleQuotes = preg_replace('/("(.*?)"|(\w+))(\s*:\s*)\+?(0+(?=\d))?(".*?"|.)/s', '"$2$3"$4$6', $jsonStringWithoutDoubleQuotes);
```
