# Plateau 2

Het Plateau 1 werkt: alle elementen uit POPIT zijn er bekend mee en weten hoe het werkt.
Tijd om er wat extra *excitement* in te brengen:

## 3D Data  
In het DigiLab gaan we (eenvoudige) 3D data zetten en die met OGC web services ter beschikking stellen aan de Catalogus (en Metadata).
Mijn voorstel om een bekende 3D dataset te nemen (neem geen dataset die je nog moet gaan ver'tile'n - dat is te moeilijk op dit moment)

## 3D Viewer
Nu we een 3D dataset hebben, willen we visualiseren in een 3D omgeveing.
Kies een 3D omgeveing waar je ervaring mee hebt en [die je kent](https://www.imagem.nl/digital-twin/3d-city/)  - ken je er geen, dan is [Unreal](https://www.unrealengine.com/en-US) of [Cesium](https://cesium.com/) of [Unity](https://unity.com/) startpunten.

(Het tijdriezen in de 3D viewer gaan we nog niet invullen). We kijken naar het 'hier en nu'.

## Sensor data

Tot nu hebben we 'trage' data omsloten via het web. Nu gaan we ook 'snelle' data via het web gaan ontsluiten - sensor data! Die sensordata kunnen we dan gaan binnenpakken in het 3D model.
Voorstel is om het [OGC SensorThings API](https://www.ogc.org/standard/sensorthings/) te gebruiken als standaard en een open source implementatie te gebruiken van [Fraunhofer FROST](https://github.com/FraunhoferIOSB/FROST-Server) (er zijn er ook anderen).

Ook hier zoals in Plateau 1: laat ook de organisatie deelnemen en de comcepten omarmen.

Niets zo slecht als een techno-demo! Laten we daarom zoeken naar een doel voor het gebruik van sensoren - liefst in context van het DMI project. (Dat kan bv waterval zijn, voor de hoosbui use case - maar ook iets met bomen....).

Ook hier weer: we gaan geen 10000 sensoren gaan uitrollen, maar eerder max een tiental - een nummer dat beheersbaar is. Om van te leren en te begrjipen.
