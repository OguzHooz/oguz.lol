---
title: "Uge 10"
summary: "Log for uge 10"
ShowReadingTime: false
ShowWordCount: false
ShowRssButtonInSectionTermList: false
weight: 40
---

## Mandag 04/03

Dagen startede med et oplæg fra en tidligere studerende, som kom med nogle gode råd angående ens emner og selve projektet.
For eksempel, at man ikke behøver at være ekspert i et emne, før man begynder på sit projekt produkt, og man ikke skal være bange for at begynde for tidligt.

Der blev også kort kigget på praktiksøgning.

## Tirsdag 05/03

Vi fortsatte i gruppen med at kigge på vores API, vi kiggede blandt andet på at få opdateret databasen med data.

Jeg fik også kigget lidt på Flutter-kurset[^1].

## Onsdag 06/03

Jeg fortsatte med PHP-kurset[^2], hvor der blev kigget på superglobals og opsætning af routing med en controller.

Senere var jeg også kort til karrieredagen, hvor jeg kort fik snakket med nogle virksomheder angående praktik på 5. semester.

Her er et udsnit af en meget simpel controller, der gør brug af superglobals til at finde den efterspurgte `path` og returnere den tilsvarende side.
```php
<?php

$uri = parse_url($_SERVER['REQUEST_URI'])['path'];

$routes = [
    '/' => 'controllers/index.php',
    '/about' => 'controllers/about.php',
    '/contact' => 'controllers/contact.php',
];


function routeToController($uri, $routes)
{
    if (array_key_exists($uri, $routes)) {
        require $routes[$uri];
    } else {
        abort();
    }
}

function abort($code = 404)
{
    http_response_code($code);

    require "views/$code.php";

    die();
}

routeToController($uri, $routes);
```

## Torsdag 07/03


## Fredag 08/03


[^1]: [*Flutter & Dart - The Complete Guide*](https://www.udemy.com/course/learn-flutter-dart-to-build-ios-android-apps/)
[^2]: [*PHP For Beginners*](https://laracasts.com/series/php-for-beginners-2023-edition)