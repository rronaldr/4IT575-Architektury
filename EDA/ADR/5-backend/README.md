# Backend aplikace pro prodej vstupenek

## Status

Accepted.

## Context

Aplikace pro prodej vstupenek bude spravovat databázi vstupenek a umožňovat souběžné nákupy vstupenek. Potřebujeme navrhnout backend aplikace, která bude schopna zpracovávat velké množství požadavků současně a zajistit, že žádné místo nebude prodáno více než jednou.

## Decision

Pro backend aplikace pro prodej vstupenek použijeme Apache Kafka pro řízení stavu a PostgreSQL pro ukládání informací.

## Consequences

- Použití Apache Kafka umožní asynchronní zpracování požadavků a schopnost zpracovávat velké množství požadavků současně.
- Použití PostgreSQL s podporou transakcí umožní spojit více operací s daty do jedné logické jednotky a zajistit, že žádné místo nebude prodáno více než jednou.
- Obě technologie jsou široce používané a dobře dokumentované, což by mělo usnadnit vývoj a údržbu aplikace.