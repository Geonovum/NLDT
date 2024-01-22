# Plateau 1

## Introduction
Het opzetten van de basis componenten voor het vinden en delen van data - het fundament waarop je kan bouwen.

Het delen van data is momenteel een verzameling van 'knippen en plakken', 'tussenkomst van medewerkers met handwerk', 'niet tracebaar', 'kwetsbaar' en 'moeilijk reproduceerbaar'. In dit plateau gaan we zaken samenbrengen om het (duur) ad-hoc werk te minimalisarem, processen te optimaliseren, reproduceerbaarheid te verhogen. Mensen enthousiast maken om met data (en data kwaliteit) te werken.

Enkele uitspraken:
- Het web is het operating systeem (toegang tot gegeves gaat via http)
- We gebruiken webservices om de data via het web te beschikking te stellen
- Elke dataset heeft een uniek identifier
- De data blijft bij de bron - principe
- Vindbaarheid en Toegangkelijkheid in een gefedereerde omgeving
- We gebruiken welgekende Open Internationale Standaarden en de Nederlandse Standaarden van Forum Standardisatie
- Stapje voor Stapje - niet alles op hetzeelfde moment. Al doende leert men.
- Samen met onze partners!

## Informatie en Technologie

Short: Maak Metadata van 2 a 3 welgekende, eenvoudige datasets (die iedereen mag zien, geen persoonsgerelateerde informatie) en klein. De oorsprong van de data is gekend en in het process ingebed. Die Metadata maken we op in DCAT2 (wetende dat die nog niet geheel klaar is)

### WebServices en Open API's
De data wordt ontsloten vai een webservice, die luistert naar HTTP en ingericht is volgende de [Nederlandse OpenAPI Design Rules](https://gitdocumentatie.logius.nl/publicatie/api/adr/).

De Geo wereld heeft reeds bestaande (en welgekende) API's voor het delen van Geo informatie - dit is een kanshebber om eerste mee te gaan. Denk aan WMS, WMTS of WFS.

Maar ook niet-Geo data (een Xls sheet) is prima informatie om via een API te delen (nogmaals: geen gevoelige data, neem die data die reeds open is).

### Metadata

We gebruiken [DCAT](https://www.forumstandaardisatie.nl/open-standaarden/dcat), een welgekend metadata formaat dat gebruikt wordt op verschillende niveaus in Nederland en de ons omringende landen. Denk maar aan [data.overheid.nl](data.overheid.nl) of [data.rotterdam.nl](data.rotterdam.nl) of de [EU data portal](https://data.europa.eu/en).

#### DCAT
(bron: https://www.forumstandaardisatie.nl/open-standaarden/dcat)

Beschrijven van datasets van op het internet gepubliceerde gegevenscatalogi ten behoeve van presentatie en gericht zoeken.

Door met DCAT datasets te beschrijven in data catalogi, wordt de vindbaarheid vergroot en wordt het eenvoudiger voor applicaties om metadata van meerdere catalogi te gebruiken. DCAT beschrijft dus waar data gevonden kan worden. Doordat DCAT is gebaseerd op het veel gebruikte standaardmodel voor gegevensuitwisseling RDF onderschrijft deze relatie de toegevoegde waarde van de standaard aan interoperabiliteit.

Data Catalog Vocabulary (DCAT) is een metadatastandaard en is ontworpen om interoperabiliteit tussen gegevenscatalogi, gepubliceerd op het internet, te vergemakkelijken. DCAT maakt decentrale publicaties en ontsluiting van catalogi mogelijk (federated search van datasets over meerdere catalogi). Door datasets te beschrijven volgens DCAT, oftewel met metadata, zijn datasets overzichtelijker te presenteren en is er gerichter te zoeken naar datasets. Door de beschrijving volgens DCAT zijn datasets toegankelijker en wordt het tot open data gemaakt. DCAT wordt gebruikt in CKAN (Open source software voor datacatalogi) dat in veel dataportalen wordt gebruikt, zoals data.overheid.nl. DCAT is op RDF gebaseerd.

Belangrijk bij de Metedata is dat we verwijzen *waar* we de data kunnen vinden (namelijk het end-point van de service die de data gaat serveren via het web).

### Catalogus

De catalogus speelt een belangrijke rol in het geheel. De Catalogus is de beheerder van de metadata

## Mensen en Organisatie

## Processen
