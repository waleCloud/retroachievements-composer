# RetroAchievements composer package
```sh
/* RetroAchievements composer Package is a simple wrapper around the RetroAchievements.org API written in PHP
*/
```

# Open Source

  - RetroAchievements composer package is completely open sourced.



# Installation
```sh
$ composer require joestrong/retroachievements
```

# Getting Started Usage

```sh
require_once('../vendor/autoload.php');

use JoeStrong\RetroAchievements\RetroAchievements;

$ra = new RetroAchievements($username, $apiKey);
$users = $ra->getTopTenUsers();

foreach ($users as $user) {
    echo "$user->username<br>";
}
```

### Methods

```php
Auth with the API

$ra = new RetroAchievements($username, $apiKey);

Get the top 10 users

$ra->getTopTenUsers();

Get the consoles

$ra->getConsoles();

Get games for console

$ra->getGamesForConsole($consoleId);
```
