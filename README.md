# Labo-4-onderzoeksrapport-iot-thomdela2
## Inleiding
Het AMQP, ofwel Advanced Message Queuing Protocol, is een toepassingslaagprotocol voor berichtgevende middleware. 
Een toepassingslaag is een abstractielaag die gedeelde communicatieprotocollen en interfacemethoden specificeert die door hosts in een communicatienetwerk worden gebruikt.
De toepassingslaag is de laatste laag binnen het OSI-model (Open System Interconnection-model).
Voorbeelden van toepassingslagen zijn http en https.
Met berichtgevende middleware (message-oriented middlewere - MOM) bedoelen we de software- of hardware-infrastructuur die het verzenden en ontvangen van berichten tussen gedistribueerde systemen ondersteunt.
API's die zich uitstrekken over verschillende platformen en netwerken worden meestal geleverd door MOM.
Bepalende kenmerken van AMQP zijn MOM, queuing, **routing** (met point-to-point en publish-and-subscribe), reliability en security.
### Routing
Routing is het proces waarbij een pad wordt geselecteerd voor verkeer in een netwerk of tussen meerdere netwerken.
In grote lijnen wordt routing uitgevoerd in vele soorten netwerken zoals computernetwerken en internet.
Routing is een besluitvorming die netwerkpaketten van bron naar de bestemming leidt langs verscheidene netwerkknooppunten. Het pakket doorsturen is de overdracht van netwerkpaketten van netwerkinterface A naar netwerkinterface B. De netwerkknooppunten zijn doorgaans netwerkhardwareapparaten zoals routers, gateways, firewalls of switches.
Routing, in de nauwkeurigere zin van het woord, verwijst vaak naar IP-routing en staat in contrast met bridging.
Ip-routing is het veld van routeringsmethoden van Internet Protocol (IP) - paketten binnen en over IP-netwerken.
#### Point-to-point
Binnen de telecommunicatie verwijst point-to-point verbinding naar een communicatieverbinding tussen twee communicatieknooppunten. 
Een voorbeeld van point-to-point communicatie is een telefoongesprek. Er zijn 2 dezelfde communicatieknooppunten, in dit geval de telefonen, en er ontstaat communicatie door een verbinding, wat de een zegt kan de ander horen. Point-to-point wordt vaak ook afgekort door P2P, niet te verwarren met peer-to-peer. Beiden worden afgekort met P2P, al wordt peer-to-peer enkel gebruikt in context van netwerken voor het delen van bestanden.
#### Publish-and-subscribe
Publish-and-subscribe is een berichtenpatroon waarbij afzenders van berichten (uitgevers) de berichten niet programmeren om rechtstreeks naar specifieke ontvangers (abonnees) te sturen, maar in plaats daarvan de gepubliceerde berichten in klassen indelen zonder kennis van welke abonnees er kunnen zijn.
Het publish-and-subscribe patroon is een broer of zus van het **berichtwachtrijparadigma** en maakt deel uit van het MOM.
##### Berichtwachtrijparadigma
In de informatica worden deze paradigma's beschouwd als software engineering componenten voor de communicatie tussen processen (IPC) of inter- thread communicatie binnen hetzelfde proces.
Ze maken gebruik van een wachtrij voor de berichten, een wachtrij voor het doorgeven van de controle van berichten of van de inhoud van de berichten.
Dit paradigma is een broer of zus van het patroon van de uitgever of abonnee en is logischerwijs onderdeel van een nog groter MOM.
## Overzicht
AMQP is een protocol voor applicatielagen, ontworpen om efficiënt een breed scala aan berichtapplicaties te ondersteunen. Er zijn 4 mogelijke soorten binnen berichtgeoriënteerde communicatie met berichtbezorgingsgaranties.
1. **Maximaal één keer**, elk bericht één keer of nooit wordt afgeleverd
2. **Ten minste één keer**, elk bericht zeker wordt afgeleverd, maar kan dit herhaaldelijk doen
3. **Precies één keer**, elk bericht komt zeker toe, en doet dit slechts één keer
4. Authenticatie en/of versleuteling op basis van **SASL** en/of **TLS**
### SASL
Simple Authentication and Security Layer, is een framework voor de authenticatie en beveiling van gegevens in Internetprotocollen. 
### TLS
Transport Layer Security, vernieuwde versie van de Secure Sockets Layer (SSL), zijn protocollen die ontworpen zijn om communicatiebeveiliging te bieden via een computernetwerk.
Diverse versies van deze protocollen worden op grote schaal gebruikt in toepassingen zoals surfen op het web, e-mail, instant messaging en meer.
## Lagen
De AMQP-specificatie is gedefinieerd in verschillende lagen:
1. Een type systeem
2. Een symmetrisch, asynchroon protocol, voor overdracht van berichten van proces A naar proces B
3. Een standaard, uitbreidbaar berichtformaat
4. een set gestandaardiseerde, uitbreidbare 'messaging-possibilities'
## Beschrijving van AMQP 1.0
### type-system
AMQP wordt gedefinieerd als een zelfsbeschrijvend coderingsschema dat weergave van een groot aanal veelgebruikten typen mogelijk maakt, en om getypte gegevens te annoteren met een extra betekenis.
Met annoteren bedoelen we extra informatie toevoegen aan een bepaald punt of stuk informatie.
In ons geval kan een bepaalde tekenreeks geannoteerd worden zodat deze kan worden begrepen als een URL (Uniform Resource Locator).
Het type-system gebruikt men om een berichtformaat te definiëren waarmee standaard- en uitgebreide metadata kunnen worden uitgedrukt én begrepen worden door de verwerkingsidentiteiten.
### Performatieven en het linkprotocol

## Bronnen
[Advanced Message Queuing Protocol - Wikipedia](https://en.wikipedia.org/wiki/Advanced_Message_Queuing_Protocol "Wikipedia - Advanced Message Queuing Protocol")

[Application layer - Wikipedia](https://en.wikipedia.org/wiki/Application_layer "Wikipedia - Application layer")

[OSI-model - Wikipedia](https://en.wikipedia.org/wiki/OSI_model "Wikipedia - OSI-model")

[Routing - Wikipedia](https://en.wikipedia.org/wiki/Routing "Wikipedia - Routing")

[IP-routing - Wikipedia](https://en.wikipedia.org/wiki/IP_routing "Wikipedia - IP-routing")

[Point-to-point - Wikipedia](https://en.wikipedia.org/wiki/Point-to-point_(telecommunications) "Wikipedia - Point-to-point")

[Publish-and-subscribe - Wikipedia](https://en.wikipedia.org/wiki/Publish%E2%80%93subscribe_pattern "Wikipedia - Publish-and-subscribe")

[Message queu - Wikipedia](https://en.wikipedia.org/wiki/Message_queue "Wikipedia - Message queu")

[Simple Authentication and Security Layer - Wikipedia](https://en.wikipedia.org/wiki/Simple_Authentication_and_Security_Layer "Wikipedia - Simple Authentication and Security Layer")

[Transport Layer Security - Wikipedia](https://en.wikipedia.org/wiki/Transport_Layer_Security "Wikipedia - Transport Layer Security")