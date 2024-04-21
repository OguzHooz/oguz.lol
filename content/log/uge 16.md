---
title: "Uge 16"
summary: "Log for uge 16"
ShowReadingTime: false
ShowWordCount: false
ShowRssButtonInSectionTermList: false
weight: 100
---

## Mandag 15/04

Jeg var til ERFA-møde i webudvikling, for vi havde besøg af Morten fra webudvikling top-up uddannelsen,
hvor han snakkede generelt om webudvikling og den erfaring, han har fået fra reelle use cases samt informerede om top-up uddannelsen.

Efter det tog jeg hjem og arbejdede videre på [csdm API'en](https://github.com/OguzHooz/csdmAPI), så JSON-dataen nu bliver gemt i databasen, og det er også muligt at tilgå dataen via endpoints.
Der er ikke blevet kigget på Flutter i dag.

## Tirsdag 16/04

Vi mødtes i projektgruppen, og jeg arbejdede videre med [csdm API'en](https://github.com/OguzHooz/csdmAPI), så det nu er muligt at tilgå data fra en specifik spiller,
så man ikke får andres data med eller generelle data om selve kampen, der ikke er nødvendige for den specifikke spiller, og hvordan andre klarer sig.

## Onsdag 17/04

Jeg begyndte på et helt andet kursus end det, jeg oprindeligt havde planlagt til Laravel.
Jeg følger følgende [YouTube tutorial](https://www.youtube.com/watch?v=VrQRa-afCAk) og er cirka halvvejs igennem den, og mit arbejde kan ses på følgende [GitHub repo](https://github.com/OguzHooz/laravel-pm-spa).
Produktet ender med at blive en projekt styrings webapplikation, hvor man kan se forskellige opgaver knyttet til projekter.

## Torsdag 18/04

Var til procesvejledning, hvor vi snakkede om vores langsigtet læringmål.
Blandt andet snakkede vi om forskellen på viden, færdigheder og kompetencer og hvordan de opsættes. Mine nuværende langsigtet læringmål kan ses [her](/plan/langsigtet).

Efterfølgende var jeg i projektgruppen, hvor jeg arbejdede på at få hostet [csdm API'en](https://github.com/OguzHooz/csdmAPI).
Kom dog ikke i mål, da jeg løb ind i problemer med databaseopsætningen. Da api'en skal køre på production, kan den ikke bruge en lokal database, men i stedet den fulde SQL Server,
hvilket også var et problem, da jeg prøvede at få den op på min egen Linux-server, så den kan tilgås fra andre enheder.

## Fredag 19/04

Det meste af dagen blev brugt på at få databasen op og kørende. Dog var der stadig nogle problemer med at få API'en til at forbinde sig til databasen.