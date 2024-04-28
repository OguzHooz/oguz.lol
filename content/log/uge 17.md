---
title: "Uge 17"
summary: "Log for uge 17"
ShowReadingTime: false
ShowWordCount: false
ShowRssButtonInSectionTermList: false
weight: 100
---

## Mandag 22/04

Jeg arbejder med Flutter-kurset[^1], som ender med en udgiftsregistreringsapp, hvor man kan indtaste sine udgifter med pris, dato og forskellige kategorier.
Her er et udsnit af Dart-kode, som viser opsætningen af en widget for en enkelt udgift:
```Dart
import 'package:expense_tracker/model/expense.dart';
import 'package:flutter/material.dart';

class ExpenseItem extends StatelessWidget {
    const ExpenseItem(this.expense, {super.key});

    final Expanse expense;

    @override
    Widget build(BuildContext context) {
        return Card(
            child: Padding(
                padding: const EdgeInsets.symmetric(
                    horizontal: 20,
                    vertical: 16,
                ),
                child: Column(
                    children: [
                        Text(expense.title),
                        const SizedBox(height: 4),
                        Row(
                            children: [
                                Text('\$${expense.amount.toStringAsFixed(2)}'),
                                const Spacer(),
                                Row(
                                    children: [
                                        Icon(categoryIcons[expense.category]),
                                        const SizedBox(width: 8),
                                        Text(expense.formattedDate),
                                    ],
                                ),
                            ],
                        ),
                    ],
                ),
            ),
        );
    }
}
```

## Tirsdag 23/04

Fortsatte med projektarbejdet og kiggede videre på at få hostet [csdm API'en](https://github.com/OguzHooz/csdmAPI).
Jeg har fået databasen op og kørende, og API'en forbinder korrekt til databasen. Dog er der nogle problemer med at tilgå endpointsne gennem nginx-proxyen på serveren.

## Onsdag 24/04

Fortsatte med [YouTube tutorial](https://www.youtube.com/watch?v=VrQRa-afCAk), og det meste af tiden er gået med at fikse bugs.
Jeg fik også kigget lidt videre på hosting af [csdm API'en](https://github.com/OguzHooz/csdmAPI) denne gang på Azure, men det lod ikke til at virke,
da jeg løb ind i problemer med at få den publiceret.

## Torsdag 25/04

Fortsatte med at kigge på, hvordan jeg kunne få hostet [csdm API'en](https://github.com/OguzHooz/csdmAPI).
Problemet er, at API'en prøver at redirecte til https, men fejler, selvom den indgående anmodning er i https bag en nginx-proxy.
Jeg fik også kigget lidt på praktiksøgning.

{{< inTextImg url="/project/project-1.png" height=40 alt="" >}}

## Fredag 26/04

Dagen blev primært brugt til at færdiggøre Flutter-kurset[^1], som kan ses på følgende [GitHub repo](https://github.com/OguzHooz/Expense-Tracker).

[^1]: [*Flutter & Dart - The Complete Guide*](https://www.udemy.com/course/learn-flutter-dart-to-build-ios-android-apps/)