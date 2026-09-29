# Architecture Overview

Meralvo is a native Flutter and Dart Android application using Material 3 and Provider for lightweight state updates.

Financial records are stored in app-private local JSON files through platform document-directory storage. No remote database or service is required for core operation. Financial calculations are kept in reusable services, including budget status, protected savings, flexible daily amounts, and cashflow projections.

The cashflow planner considers locally recorded transactions, recurring obligations, expected income, and the selected month. Backup and restore operate on validated JSON documents selected by the user. The storage layer versions its schema and migrates existing V1 records to V2 while retaining historical months.

This is a high-level product overview. Implementation source and detailed internal code are maintained privately.
