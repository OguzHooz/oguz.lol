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


## Onsdag 24/04


## Torsdag 25/04


## Fredag 26/04


[^1]: [*Flutter & Dart - The Complete Guide*](https://www.udemy.com/course/learn-flutter-dart-to-build-ios-android-apps/)