# Rozhodnutí o výběru cloudového řešení

## Status
Schválený

## Context
Prodejní portál musí být nasazen na nějakém serveru: on-promise, hosting, cloud.

## Decision
Bylo vybráno cloudové řešení AWS od společnosti Amazon.

## Consequences
AWS nabízí komplexní řešení nejen hosting. Díky AWS bude možné využít ostatní částí jako load balancer, uložiště S3, NoSQL databázi DynamoDB, nechat aplikaci běžet serverless pomocí Lambd, které je kritické v případě využití Event Driven Architecture. Díky tomu bude aplikace velmi rychlá, k tomu nám AWS umožní škálovat výkon podle zátěže a zároveň poskytne nástroje pro monitorování výkonu.