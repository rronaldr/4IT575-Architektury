# Diagram nasazení

![Deployment diagram](/resources/diagrams/deployment.png)

## Popis diagramu nasazení
Diagram nasazení se skládá z hlavních komponent Client a Amazon AWS. Klient bude tedy pomocí svého zařízení obsahující webový prohlížeč přistupovat k softwarovému webovému serveru (Nginx) pomocí protokolu HTTP/HTTPS, přičemž nezáleží na tom, zda se jedná o prodejce a kupujícího - pro obě aplikace bude platit totožný rámec pro přístup.

Pomocí relace na Amazon AWS bude pak zpřístupnění probíhat pomocí aplikačního serveru obsahující API rozhraní pro zajištění komunikace pomocí CRUD operací a databázového serveru, na kterém bude běžet databáze Amazon DynamoDB, což je proprietární NoSQL databázová služba.