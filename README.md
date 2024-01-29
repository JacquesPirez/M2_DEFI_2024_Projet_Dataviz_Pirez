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

% Please add the following required packages to your document preamble:
% \usepackage[table,xcdraw]{xcolor}
% Beamer presentation requires \usepackage{colortbl} instead of \usepackage[table,xcdraw]{xcolor}
\begin{table}[]
\begin{tabular}{|l|l|}
\hline
\rowcolor[HTML]{C0C0C0} 
\multicolumn{1}{|c|}{\cellcolor[HTML]{C0C0C0}\textbf{Colonne}} & \multicolumn{1}{c|}{\cellcolor[HTML]{C0C0C0}\textbf{Description}}                                                                                                                                                                                                                                                                   \\ \hline
\textbf{DATE}                                                  & \begin{tabular}[c]{@{}l@{}}Journal édité par l’Université technique Gheorghe Asachi de Iasi, se situant en Roumanie, \\ “et qui couvre un large éventail de sujets concernant l’ingénierie et la gestion de l’environnement au sens large, \\ et qui met particulièrement l’accent sur les études interdisciplinaires.\end{tabular} \\ \hline
\rowcolor[HTML]{C0C0C0} 
\textbf{HEURE}                                                 & Heure de la mesure                                                                                                                                                                                                                                                                                                                  \\ \hline
\textbf{NO}                                                    & Concentration moyenne en NO en µg/m3                                                                                                                                                                                                                                                                                                \\ \hline
\rowcolor[HTML]{C0C0C0} 
\textbf{NO2}                                                   & Concentration moyenne en NO2 en µg/m3                                                                                                                                                                                                                                                                                               \\ \hline
\textbf{PM10}                                                  & Concentration moyenne en PM10 en µg/m3                                                                                                                                                                                                                                                                                              \\ \hline
\rowcolor[HTML]{C0C0C0} 
\textbf{PM25}                                                  & Concentration moyenne en PM2,5 en µg/m3 uniquement pour la station AUBER                                                                                                                                                                                                                                                            \\ \hline
\textbf{CO2}                                                   & Concentration moyenne en CO2 en ppm                                                                                                                                                                                                                                                                                                 \\ \hline
\rowcolor[HTML]{C0C0C0} 
\textbf{TEMP}                                                  & Température ambiante en °C                                                                                                                                                                                                                                                                                                          \\ \hline
\textbf{HUMI}                                                  & Humidité relative en \%                                                                                                                                                                                                                                                                                                             \\ \hline
\end{tabular}
\end{table}

# Nettoyage et enrichissement des données

# Conclusion
