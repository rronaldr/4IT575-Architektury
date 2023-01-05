# Dokumentace 2. architektury (Event Driven Architecture)

## Struktura dokumentace
- [ADR](/EDA/ADR/README.md)
- [Diagramy](/EDA/Diagrams/README.md)

## Přehled výhod a nevýhod zvoleného řešení

### Výhody
Mezi výhody navrženého řešení patří rozhodně to, že navržená událostmi řízená architektura splňuje důležité charakteristiky, které jsou potřebné pro splnění požadavků zadání - konkrétně se jedná o škálovatelnost, výkon a odolnost vůči chybám, díky kterým by měl být při správné implementaci řešení a volbě parametrů zajištěn souběžný a bezproblémový nákup vstupenek, při kterém nedojde k duplikování prodejů stejného místa.

K výše uvedenému také dopomůže provozování daného řešení v cloudu, a to pomocí AWS, pomocí kterého lze do značné míry zajistit elasticitu  a zlepšit škálovatelnost výkonu. Bezchybný provoz, či alespoň k včasné reakci pak může dopomoct možnost snadného monitorování provozu právě pomocí AWS.

Jako výhodu navrhovaného řešení lze uvést i rozhodnutí řešení provozovat jako webovou aplikaci - tím se zredukují náklady, a to na lidské zdroje, co se týče jejich vytíženosti při implementaci a udržování řešení (oproti nativnímu vývoji), přičemž všechny potřebné funkcionality lze realizovat i pomocí webového prohlížeče.

### Nevýhody
Co se týče provozování řešení pomocí AWS - je třeba myslet na možný zbytečný nárůst ceny při špatném nadimenzování kapacit.

Jako nevýhody řešení lze pak uvést to, že architektura je poměrně složitá a s tím souvisí i to, že v případě kritického (avšak ne příliš pravděpodobného) scénáře pádu aplikace by byl v případě nepoužití AWS komplikovaný její restart a zotavení, avšak toto riziko by se mělo použitím AWS značně redukovat.

Dále je také nevýhodou složitější testovatelnost daného řešení díky použité architektuře, avšak díky AWS od společnosti Amazon jdou i asynchronní události poměrně dobře monitorovat.
