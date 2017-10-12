[![N|Solid](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRAhk6glux07Qv-MJHXlBmK8LQ0gKALFPp2Yc_UTMGd9AMR_gRLKg)]()
# RetroAchievements composer package

RetroAchievements composer Package is a ......................................................
# Open Source

  - RetroAchievements composer package is completely open sourced. Any [contribution](https://github.com/joestrong/retroachievements-composer/#contribute) is highly appreciated.



# Installation

RetroAchievements composer package requires [Composer](https://composer.org/) to run.

#### Install the dependencies.

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


# Development

Want to contribute? Great!



### Todos

 - Write MORE Tests
 - Add Night Mode

License
----

MIT


**Free Software, Hell Yeah!**
