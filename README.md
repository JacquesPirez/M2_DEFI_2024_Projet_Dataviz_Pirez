# Qualité de l'air en Île-de-France : où en est-on ?
## Sommaire

- [Présentation du sujet](#presentation-du-sujet)
- [Collecte des données](#collecte-des-données)
- [Nettoyage et enrichissement des données](#nettoyage-et-enrichissement-des-données)
- [Conclusion](#conclusion)

# Présentation du sujet

C'est un problème qui existe depuis des années, il s'agit de la pollution de l'air aussi bien à l'extérieur que dans les milieux souterrains, notamment dans les stations de métro ou de RER. Concernant la pollution de l'air dans les stations souterraines du métro, la RATP a été plusieurs fois pointée du doigt par la mairie de Paris, et mène en parallèle plusieurs expérimentations pour lutter contre ce problème. Où en est-on aujourd'hui avec les différentes mesures ? Nous allons tenter d'y répondre à travers plusieurs jeux de données.

# Collecte des données
Concernant la collecte des données,j'ai commencé par des jeux de données réalisés par la RATP au format CSV, station par station. Avant d'analyser ces tableaux, il est nécessaire de faire un point sur les différents cigles mis en avant (les informations viennent de la notice explicative de la RATP, datant de 2017) :

- DATE : Date et heure de la mesure exprimé en TEmps Universel. L'heure réelle peut être TU+1 ou TU+2 suivant l'heure d'été ou d'hiver.
- HEURE : Heure de la mesure.
- NO : Concentration moyenne en NO en µg/m3.
- NO2 : Concentration moyenne en No2 en µg/m3.
- PM10 : Concentration moyenne en PM10 en µg/m3.
- PM25 : Concentration moyenne en PM2,5 en µg/m3, uniquement pour la station AUBER.
- CO2 : Concentration moyenne en CO2 en ppm.
- TEMP : Température ambiante en °C.
- HUMI : Humidité relative en %.

# Nettoyage et enrichissement des données

# Conclusion
