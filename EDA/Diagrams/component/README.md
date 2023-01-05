# Diagram komponent

![Component diagram](/resources/diagrams/component.png)

## Popis diagramu
Diagram komponent se skládá z dvou hlavní komponent - frontendu a AWS, přičemž ke komunikaci dochází přes API rozhraní.

### Frontendová část
Na frontendové části se poté nacházejí dvě single page aplikace - jedna pro inzerenty a druhá pro kupující.

### AWS
V Amazon Web Services se poté nachází několi subsystémů - prvním z nich je Elastic Load Balancer, který automaticky příchozí provoz distribuuje mezi skupinu backendových serverů způsobem, který zvyšuje rychlost a výkon řešení a pomáhá se škálovatelností. Ten je dále navázán na AWS Lambdu, což je výpočetní služba, která umožňuje spouštět kód tzv. serverless, a zajišťuje automatické škálování.

Další subsystémem je serverless aplikace, která obsahuje několik dalších komponent. Mezi ně patří uživatelská služba zajišťující autentizaci a autorizaci uživatelů, dále služba pro správu fronty (v případě přetížení budou uživatelé zařazeni do fronty pro nákup vstupenek), dále platební brána (obsahující konkrétní integrace) a služba pro správu akcí, díky které mohou inzerenti spravovat konkrétní události.

Je tu také služba kontrolující obsazenost míst, která bude v reálném čase ověřovat celkovou kapacitu, stejně jako obsazenost konkrétních míst. Poslední součástí, kterou lze jmenovat je služba pro generování lístků, která slouží pro vygenerování unikátních lístků včetně příslušného QR kódu vstupenky.

Subsystém serverless aplikace pak pomocí AWS SDK komunikuje s DynamoDb, což je NoSQL databázová služba. Další komunikace také probíhá s Amazon S3, což je úložiště objektů. 