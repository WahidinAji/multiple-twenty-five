<p>Open to collaboration</p>
<p>Just fork and modify, then pull request😁</p>

<a href="a17wahidin@gmail.com">My Email</a>

# Code
```php
function multipleOfTwentyFive($input)
{
    $round = intval($input);
    $get_after_comma = $input - $round;
    $result = 0;
    switch ($get_after_comma) {
        case $get_after_comma == 0.00 && $get_after_comma >= 0.76:
            $result = number_format($round, 2);
            break;
        case $get_after_comma > 0.00 && $get_after_comma <= 0.25:
            $result = number_format($round + 0.25, 2);
            break;
        case $get_after_comma > 0.25 && $get_after_comma <= 0.50:
            $result = number_format($round + 0.50, 2);
            break;
        case $get_after_comma > 0.50 && $get_after_comma <= 0.75:
            $result = number_format($round + 0.75, 2);
            break;
        default:
            $result = number_format($round, 2);
            break;
    }
    return $result;
}
```

# Example to use it

```php
$convert = multipleOfTwentyFive(25.001);
echo $conver;
//output    =   25.25
```