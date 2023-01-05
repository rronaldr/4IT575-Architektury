# Sekvenční diagram rezervace

![Sequence diagram](/resources/diagrams/sequence.png)

## Popis sekvenčního diagramu rezervace
Sekvenční diagram rezervace se skládá z webového prohližeče kupce, systému aplikace a platební brány třetí strany.

Webový prohlížeč zahajuje proces rezervace tím, že systému pošle požadavek na zobrazení všech koncertů podle volitelných parametrů, jako je například žánr.
Systém následně na základě požadavku nechá prohlížeči zobrazit si všechny koncerty, které splňují nastavené parametry.
Webový prohlížeč si následně vybere jeden koncert a systém mu pošle detaily o koncertu, jako je například cena nebo počet volných míst.
Na stránce s detaily koncertu si webový prohlížeč dále může vybrat místo na koncertu, a odeslat požadavek na jeho zarezerovávní.
Systém zkontroluje, že místo na koncertu je volné a pokud ano, umožní prohlížeči, aby za něj zaplatil skrze platební bránu třetí strany.
V momentě, kdy platební brána platbu zpracuje, pošle potvrzení o platbě systému, který tím dokončí rezervaci místa na koncert a potvrdí to prohlížeči.