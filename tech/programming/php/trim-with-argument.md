# Trim any character from a string

Interestingly, in PHP you can actually pass in a second parameter to the `trim()` function which then will be used to trim the passed character from the beginning and end of a string.

```php
$uri = '/about/contact/';
$trimmed = trim($uri, '/');
echo $trimmed;

// about/contact
```
