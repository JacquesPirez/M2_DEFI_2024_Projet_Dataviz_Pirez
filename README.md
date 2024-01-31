# Qualité de l'air à Paris : où en est-ton ?

## Sommaire

- [Présentation du sujet](#presentation-du-sujet)
- [Collecte des données](#collecte-des-données)
- [Nettoyage des données](#nettoyage-des-données)
- [Conclusion](#conclusion)

# Présentation du sujet

C'est un problème qui existe depuis des années, il s'agit de la pollution de l'air aussi bien à l'extérieur que dans les milieux souterrains, notamment dans les stations de métro ou de RER. Concernant la pollution de l'air dans les stations souterraines du métro, la RATP a été plusieurs fois pointée du doigt par la mairie de Paris, et mène en parallèle plusieurs expérimentations pour lutter contre ce problème. Où en est-on aujourd'hui avec les différentes mesures ? Nous allons tenter d'y répondre à travers plusieurs jeux de données.

# Collecte des données
Concernant la collecte des données,j'ai commencé par des jeux de données réalisés par la RATP au format CSV, station par station. Avant d'analyser ces tableaux, il est nécessaire de faire un point sur les différents cigles mis en avant (les informations viennent de la notice explicative de la RATP, datant de 2017) :

| Indicateurs | Description de chaque indicateur                                                                                             |
|-------------|------------------------------------------------------------------------------------------------------------------------------|
| DATE        | Date et heure de la mesure exprimé en Temps Universel L’heure réelle peut être TU+1 ou TU+2 suivant l’heure d’été ou d’hiver |
| HEURE       | Heure de la mesure                                                                                                           |
| NO          | Concentration moyenne en NO en µg/m3                                                                                         |
| NO2         | Concentration moyenne en NO2 en µg/m3                                                                                        |
| PM10        | Concentration moyenne en PM10 en µg/m3                                                                                       |
| PM25        | Concentration moyenne en PM2,5 en µg/m3 uniquement pour la station AUBER                                                     |
| CO2         | Concentration moyenne en CO2 en ppm                                                                                          |
| TEMP        | Température ambiante en °C                                                                                                   |
| HUMI        | Humidité relative en %   

Informations de la RATP, tableau généré par Tables Generator.

Deux autres informations importantes selon la RATP :

- "La qualité de l'air en station varie en fonction de différents paramètres tels que l'affluence, la profondeur de la station, le type de matériel roulant, la fréquence du trafic, les travaux d'entretien et de génie civil, l'air extérieur...
- La nuit, en dehors des heures d'exploitation, les pics de concentrations en particules et en dioxyde d'azote sont dus essentiellement à la présence de chantiers de rénovation (renouvellement des voies, ajout de façades de quai etc...)".

# Nettoyage des données

Qualité de l'air à la station Châtelet (source : https://data.ratp.fr/explore/dataset/qualite-de-lair-mesuree-dans-la-station-chatelet/information/) :

<div class="flourish-embed flourish-chart" data-src="visualisation/16631062"><script src="https://public.flourish.studio/resources/embed.js"></script></div>


Qualité de l'air à la station Châtelet (côté RER) (source : [RATP](https://dataratp.opendatasoft.com/explore/dataset/qualite-de-lair-mesuree-dans-la-station-chatelet-rer-a0/information/?sort=-dateheure)) : 

<div class="flourish-embed flourish-chart" data-src="visualisation/16639741"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

Qualité de l'air à la station Auber (source : https://data.ratp.fr/explore/dataset/qualite-de-lair-mesuree-dans-la-station-auber/information/?sort=-dateheure) : 

<div class="flourish-embed flourish-chart" data-src="visualisation/16641032"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

Qualité de l'air à la station Nation (côté RER A) (source : https://data.ratp.fr/explore/dataset/qualite-de-lair-mesuree-dans-la-station-nation-rer-a0/information/) :

<div class="flourish-embed flourish-chart" data-src="visualisation/16641606"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

Concernant les différents jeux de données de la RATP que j'ai utilisé, je me suis limité aux mesures prises à partir de janvier 2022, pour raison de lisibilité des graphiques.

Pour compléter mon analyse, j'ai décidé de me rendre sur la plateforme OpenData de la Mairie de Paris. Pour mesurer la qualité de l'air extérieure, la Mairie de Paris utilise l'indice ATMO, qui a été révisé par le Ministère de la Transition Ecologique le 1er janvier 2021. Selon  la Mairie de Paris, cet indice "intègre les principaux polluants atmosphériques réglementés, traceurs des activités de transport, urbaines et industrielles PM10, PM2.5, dioxyde d'asote, ozone, dioxyde de souffre. Il se décline en six qualificatifs définis selon différentes classes pour ces cinq polluants : "bon", "moyen", "dégradé", "mauvais", "très mauvais", "extrêmement mauvais"". 
Voici une visualisation dynamique qui couvre la qualité de l'air en 2021 ainsi qu'en 2022 (source : https://opendata.paris.fr/explore/dataset/qualite-de-l-air-indice-atmo/information/) :

<div class="flourish-embed flourish-chart" data-src="visualisation/16641296"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

# Conclusion

Pour conclure, grâce à cette enquête, nous venions d'apprendre que la qualité de l'air à Paris, que ce soit à l'extérieur, dans le métro ou le RER, dépend de plusieurs facteurs, et que la Mairie de Paris et la RATP utilisent quasiment les mêmes indicateurs pour lutter contre ce problème. Il s'agit d'un sujet sérieux contre lequel il faut lutter pour éviter d'amplifier ce phénomène de pollution.
