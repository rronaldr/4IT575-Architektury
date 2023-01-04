# Event Driver ADR

## Status

Navrhnuta architektura řízená událostmi. 

## Context

Potřebujeme vhodnou architekturu, které splňuje požadavky na aplikace ze zadání naši seminární práce – důležitá je především škálovatelnost, výkon a odolnost vůči chybám. Uživatelů muže být v jeden moment velké množství, pokud se budou prodávat lístky na populární koncert, a nesmí se stát, že by na jedno místo měli nárok dva uživatelé. Z toho důvod je důležitý i výkon, abychom mohli rychle obsloužit velké množství zákazníků. 

## Decision

Navrhujeme využít událostmi řízenou architektury pro řešení aplikace ze zadání naší seminární práce z důvodu vysoké škálovatelnosti a výkonu aplikace spolu s o vysokou ochranou vůči chybám, což jsou charakteristiky zvolené architektury, které jsou vysoce žádané v řešené aplikaci. 

## Consequences

Důsledkem bude využití moderní distribuované architektury pro řešení aplikace, která z velké míry splňuje požadavky aplikace. 