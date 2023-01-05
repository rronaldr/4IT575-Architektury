# Backend aplikace pro prodej vstupenek v Javě

## Status
Accepted.

## Context
Prodejní portál vstupenek potřebuje pružné řešení pro zpracování velkého počtu současných prodejů vstupenek a velkého počtu akcí. Portál bude nasazen na cloudu AWS a přístupný prostřednictvím SPA frontendu tisíci současnými uživateli, s nárazy až 10 000 uživateli za sekundu při vysoké poptávce. Aplikace musí podporovat současné nákupy vstupenek, zabraňovat opakovanému prodeji jakékoli jednotlivé vstupenky a umožňovat kupujícím zobrazovat volná místa.

## Decision
Backend pro prodejní portál vstupenek bude implementován v Javě

## Consequences
Java je oblíbený, široce používaný programovací jazyk s velkou komunitou vývojářů a komplexní dokumentací. Má dobrou podporu pro běh na cloudu a integraci s AWS službami, jako jsou S3, DynamoDB a Lambda. Má také silnou podporu pro součinnost, což je důležité pro zpracování velkého objemu požadavků v architektuře založené na událostech, a dobrou podporu pro REST API. V neposlední řadě, může existovat větší počet dostupných vývojářů se zkušenostmi v Javě, což usnadňuje hledání a najímání členů týmu s potřebnými dovednostmi.