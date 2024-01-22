# Plateau 3

## Rekenmodellen

Het [Nelen en schuurman](https://nelen-schuurmans.nl/en/home/) opnemen in DigiLab en de datafeeds doen via API's (dus machines en geen mensen), alsook het antwoorden. Dus meer en meer gaan integreren.

In Plateau 4 willen we modellen aan elkaar te knopen.

## Asyncroniteit

Asyncroniteit

![Screenshot 2024-01-22 153224](https://github.com/Geonovum/DTaaS/assets/4082369/98531ed2-106c-41be-8d68-a2bd57cba036)

(bron: Dreamworks Animation Shrek 2, 2004)

Niet meer 'Are we there yet' (100x en dan 'plop' :-) ), maar "we have arrived"

De meeste 'event' in een Digitale Tweeling komen onaangekondigd - net zoals in het echte leven. (en liefst op het slechtste moment).

Daarom het is het noodzakelijk om een Asyncroneous event afhandler te hebben in onze omgeveing - aka een Pub-Sub systeem. Pub-Sub?

## Publish en Subscribe

In softwarearchitectuur is publiceren-abonneren (Publish en Subscribe - aka PubSub) een berichtenpatroon waarbij uitgevers berichten categoriseren in klassen die door abonnees worden ontvangen. Dit staat in contrast met het typische berichtenpatroonmodel waarbij uitgevers berichten rechtstreeks naar abonnees sturen.

## Request en Response

Bij een request/response wordt een request gedaan voor data. Deze vraag komt aan bij de data owner, die op zoek gaat naar de data die gevraagd werd. Dit zou in praktijk kunnen betekenen dat de data owner een vraag van een gebruiker die door middel van een API tot bij hem kwam, via een query opvraagt in zijn database.

Eens de data owner zijn data gevonden heeft, stuurt hij deze terug. Dit is de response.

