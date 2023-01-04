# Rozhodnutí o způsobu fungování klientské aplikace

## Status
Schválený

## Context
Je nutné vytvořit aplikaci s uživatelským rozhraním, aby měli uživatelé možnost aplikaci používat.

## Decision
Frontend bude tvořen dvěmi SPA, jedna pro inzerenty a druhá pro kupující uživatele.

## Consequences
SPA dovolí použít i vybranou funkcionalitu offline, např. pro zobrazení QR kódu v prohlížeči, pokud na události nebude signál. Použití webové aplikace také dovolí využít klasických HTML5 elementů pro získání fotografie z kamery zařízení nebo nahrání souboru (dokumenty uživatele atd.). Dále odpadne nutnost udržovat vícero aplikací aktuálních, kdy by byla potřeba aplikace pro počítače, mobilní zařízení využívající OS Android a iOS. Frontend bude tvořen dvěmi SPA, kdy dojde k jasnému GUI rozdělení části pro inzerenty a kupující, oboje dostupné na jiné adrese (pro inzerenty řešeno subdoménou.)