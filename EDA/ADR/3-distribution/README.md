# Rozhodnutí o kanálu distribuce aplikace

## Status
Schválený

## Context
Aplikace musí být někde dostupná pro klienty (těmi jsou inzerenti nebo kupující) k používání.

## Decision
Aplikace bude běžet jako SPA aplikace ve webovém prohlížeči.

## Consequences
Díky využití webové aplikace bude možné k ni přistoupit z širokého množství zařízení. SPA dovolí použít i nějaké funkcionality offline, např. pro zobrazení QR kódu v prohlížeči, pokud na události nebude signál. Dále odpadne nutnost udržovat vícero aplikací aktuálních, kdy by byla potřeba aplikace pro počítače, mobilní zařízení využívající OS Android a iOS. Frontend bude tvořen dvěmi SPA, kdy dojde k jasnému GUI rozdělení části pro inzerenty a kupující, oboje dostupné na jiné adrese (pro inzerenty řešeno subdoménou.)