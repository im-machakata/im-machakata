```php
$aboutMe       = new Bio();
$smartUser     = new User();
$hiringManager = new User();

// smart users
$smartUser
    ->reads($aboutMe)
    ->on('https://isaac.co.zw/');

// hiring managers
$hiringManager
    ->reads($aboutMe)
    ->on('https://isaac.co.zw/')
    ->browsesProjects()
    ->emails('hie@isaac.co.zw')
    ->withJobOffer();
```
