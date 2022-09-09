# Estimation des besoins de la plante par apprentissage automatique
Pour satisfaire les besoins en eau des plantes, il faut prendre en considération plusieurs facteurs à savoir le climat, les propriétés du sol et la culture. 
La partie climat est représentée par la variable évapotranspiration de référence (ET0). qui traduit la demande climatique en termes d’évaporation (quantité perdue au niveau du sol) et de transpiration des plantes . Par conséquent, les agronomes n’arriveront pas à établir leurs programmes d’irrigations sans recours à cette variable.
Malgré l’indispensabilité de cette variable pour la gestion de l’irrigation, les petits et moyens agriculteurs n’ont pas toujours l’accès à cette information cruciale. 
L’idéal pour remédier à l’ensemble des problèmes précités est de mettre à la disposition des agriculteurs l’information avec un coût raisonnable. Donc notre start-up a trouvé le meilleur compromis possible entre la précision de l’information et le coût pour y accéder. Tout d’abord, nous avons estimé l’ET0 en réduisant le nombre de paramètres de 5 à 2 avec une précision qui a atteint 80% pour une première phase. 

## Problématique
L’agriculteur ne pourra pas établir un programme d’irrigation sans avoir accès à l’ET0, ce qui explique les efforts consentis pour la mettre à sa disposition. 
L’évapotranspiration de référence (ET0) est une variable hydrologique complexe définie par diverses variables climatiques. Traditionnellement, l’ET0 est calculée par diverses méthodes empiriques basées sur des données climatiques rigoureuses. Cependant, il existe de nombreux endroits où les différentes données climatiques ne sont pas disponibles pour le calcul de l’ET0. Ceci est expliqué par un investissement lourd pour l’installation d’une station météorologique (les charges varient de 60 000 à 70 000 DH). Un tel investissement n’est pas économiquement justifiable pour les petits et moyens agriculteurs.
De plus, cette mesure nécessite l’installation de cinq capteurs au moins pour mesurer l’ensemble des paramètres météorologiques. En outre, chaque capteur exige un calibrage ainsi qu’un module de filtration des valeurs aberrantes. Sans oublier l’inadaptation de ces formules aux différentes régions climatiques du Maroc.

##  La base de Données

Pour démontrer le concept, nous avons choisi 4 stations météorologiques différentes :
    • Erreggada, Ribate El Kheir, Zaouia Bougrine et Louata situées dans la région Fès-Meknès.
Les données météorologiques quotidiennes ont été acquises pour la période allant de  janvier 2018 (4 ans) (42 mois) à partir des stations météorologiques de la Direction provinciale de l'agriculture DPA.
Les données climatiques moyennes annuelles de la station météorologique Erreggada sont présentées au tableau N°1. Cinq variables météorologiques ont été enregistrées quotidiennement, notamment l’ET0 journalière en [mm/jr] (ET0) ; la température maximale de l'air [°C] (Tmax) ; la température minimale de l'air [°C] (Tmin) ;la température moyenne de l'air [°C] (Tmoy);  l'humidité relative maximale [%] (HRmax) ;l'humidité relative minimale [%] (HRmin) ;l'humidité relative moyenne [%] (HRmoy) ; le rayonnement solaire[W/m2] (Rs) et la vitesse du vent (U2, Km/h).

Les mesures (température de l'air, humidité relative et vitesse du vent) ont été effectuées à 2 m au-dessus de la surface du sol. 
