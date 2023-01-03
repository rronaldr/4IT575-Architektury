# Title

## Status

Navrhované

## Context

Portál pro prodej vstupenek na koncerty je webová platforma, která uživatelům umožňuje nakupovat vstupenky na koncerty a další akce. Má velký počet událostí a velký objem vstupenek a potřebuje řešení, které zvládne tisíce souběžných uživatelů a nápory až 10 000 uživatelů za sekundu při prodeji vstupenek.

## Decision

Pro portál pro prodej vstupenek na koncerty použijeme architekturu mikroslužeb. Tento přístup zahrnuje rozdělení celého systému na sadu nezávislých, volně propojených služeb, které lze vyvíjet, nasazovat a škálovat nezávisle. Každá služba bude zodpovědná za určitou sadu funkcí, například za zpracování nákupu vstupenek, správu rozvrhu akcí a zobrazování volných míst.

## Consequences

Použití architektury mikroslužeb přinese portálu pro prodej vstupenek na koncerty několik výhod, například flexibilitu a škálovatelnost. Díky samostatnému vývoji a nasazení každé služby můžeme každou službu optimalizovat a škálovat podle jejích specifických potřeb. To nám umožní zvládnout velký počet událostí a vysoký objem vstupenek a umožní nám to rychle reagovat na změny a aktualizace. Tento přístup navíc usnadní aktualizaci a změny systému, protože můžeme provádět změny v jednotlivých službách, aniž by to ovlivnilo celý systém.

Použití architektury mikroslužeb má však také některé potenciální nevýhody a problémy. Například vyžaduje větší koordinaci a komunikaci mezi týmy pracujícími na různých službách, protože každou službu je třeba vyvíjet a udržovat nezávisle. Kromě toho může vyžadovat další infrastrukturu a nástroje pro správu služeb, například registr služeb a síť služeb. Tyto problémy lze zmírnit použitím správných postupů komunikace a spolupráce mezi týmy a také použitím vhodných nástrojů a technologií pro správu služeb.