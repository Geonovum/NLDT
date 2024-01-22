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

Note: als data op het web ter beschkking wordt gestelt, dan moet die data [uniek identificeerbaar](https://www.geonovum.nl/uploads/documents/20210716%20Geonovum%20Ontwerp%20UOI%20v081%20definitief.pdf) zijn op het web.

### Metadata

We gebruiken [DCAT](https://www.forumstandaardisatie.nl/open-standaarden/dcat), een welgekend metadata formaat dat gebruikt wordt op verschillende niveaus in Nederland en de ons omringende landen. Denk maar aan [data.overheid.nl](data.overheid.nl) of [data.rotterdam.nl](data.rotterdam.nl) of de [EU data portal](https://data.europa.eu/en).

#### DCAT
(bron: https://www.forumstandaardisatie.nl/open-standaarden/dcat)

Beschrijven van datasets van op het internet gepubliceerde gegevenscatalogi ten behoeve van presentatie en gericht zoeken.

Door met DCAT datasets te beschrijven in data catalogi, wordt de vindbaarheid vergroot en wordt het eenvoudiger voor applicaties om metadata van meerdere catalogi te gebruiken. DCAT beschrijft dus waar data gevonden kan worden. Doordat DCAT is gebaseerd op het veel gebruikte standaardmodel voor gegevensuitwisseling RDF onderschrijft deze relatie de toegevoegde waarde van de standaard aan interoperabiliteit.

Data Catalog Vocabulary (DCAT) is een metadatastandaard en is ontworpen om interoperabiliteit tussen gegevenscatalogi, gepubliceerd op het internet, te vergemakkelijken. DCAT maakt decentrale publicaties en ontsluiting van catalogi mogelijk (federated search van datasets over meerdere catalogi). Door datasets te beschrijven volgens DCAT, oftewel met metadata, zijn datasets overzichtelijker te presenteren en is er gerichter te zoeken naar datasets. Door de beschrijving volgens DCAT zijn datasets toegankelijker en wordt het tot open data gemaakt. DCAT wordt gebruikt in CKAN (Open source software voor datacatalogi) dat in veel dataportalen wordt gebruikt, zoals data.overheid.nl. DCAT is op RDF gebaseerd.

Belangrijk bij de Metedata is dat we verwijzen *waar* we de data kunnen vinden (namelijk het end-point van de service die de data gaat serveren via het web).

### Catalogus

De catalogus speelt een belangrijke rol in het geheel. De Catalogus is de beheerder/verzamelaar van de metadata en laat toe dat er in de metadata wordt gezocht.

![Screenshot 2024-01-22 134850](https://github.com/Geonovum/DTaaS/assets/4082369/8ed8ad7c-e2fa-4681-bc99-51a3e8feb33b)

![Screenshot 2024-01-22 135242](https://github.com/Geonovum/DTaaS/assets/4082369/ff27afa1-6a25-4b68-85fa-1bc2d3079a54)

## Mensen en Organisatie

De bovengenoemde concepten (Metadata, Catalogus, WebService) moet binnen de organisatie landen. En ook het personeel (1) moet begrijpen wat ze zijn, hoe ze ingezet worden, wat ze kunnen, hoe je ze onderhoudt. Dit is geen simpele opgave. In vele gevallen is het er 'een werk erbij', waarvoor en amper beloning bestaat. Dat laatste moet omgekeerd worden.

(1) Alle mensen binnen de gemeente en provicnie, van ICTers, gebruikers, data makers, etc moeten doordrongen worden met deze gedachten. Zodat iedereen begrijpt waarom we het doen.

De organisatie moet doordrongen zijn waarom we data willen delen, waarom we het goed moeten doen - en - wat het vooral niet is (een pdf via email sturen is niet data delen).

## Processen en Mensen

De huidige processen zullen waarschijnlijk moeten aangepast worden om 'data te laten stromen via het web'. 
We kijken eerst zoals het nu gaat, nemen 2 a 3 voorbeeld datasets en gaan die als verander voorbeeld nemen. 

Formele processen worden in de deze fase niet aangepast, maar we markeren wel veranderingen in de processen voor de toekomst. We kijken ook naar nieuwe rollen binnen de organisatie (bv datastewart - iemand die enthousist is om data op order te houden, de kwaliteit ervan te begrijpen en te willen verhogen, de metadata bijhoudt,... - en waardering krijgt binnen de organisatie)

Let op: eerst begrijpen alvorens begrepen te worden.

# Digilab

In het Digilab (een digitale speeltuin) gaan we bovenstaande infrastructuur testen. Dus in het DigiLab draait een Catalogus en wat webservices. Minimale metedata is beschikbaar voor de voorbeelden.
De minimale set werkt onmiddellijk en staat klaar op het DigiLab.

## Wat is DigiLab

Een Clowdomgeving (Kubesnetes en Docker) waarop software kan gedeployed worden (denk aan de CKAN Catalogus, Docket container met webseervice).
DigiLab is een niet operationele omgeving en kan op elke moment geresetted worden. Het is een omgeving om te leren en concepten te beproevem.

## Wie kan erbij?
We kunnen iedereen op digilab uitnodignen die we willen (incl leveranciers)
