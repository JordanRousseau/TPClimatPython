# TPClimatPython
Nous avons tout d'abord traiter le fichier climat mois par mois. Dans le but d'avoir 12 courbes pour chaque mois. Cela nous permet d'avoir une vision global de nos donnés ainsi que les bornes des températures cela nous sera utile pour la suite.

![alt text](https://cdn.discordapp.com/attachments/382081589234106389/806093813515812874/unknown.png)

Ensuite nous avons réalisé le graphique pour assembler afin d'avoir toutes les températures de l'année. Nous avons retiré les valeurs NaN pour éviter d'avoir des trous dans notre graphique. Nous obtenons la courbe suivante :

![alt text](https://cdn.discordapp.com/attachments/382081589234106389/806095497944236032/unknown.png)

Nous avions également un deuxième fichier qui comprennait des erreurs nous devions les isoler puis les corriger, à l'aide d'une expression regex verifiant que les données sont strictement des températures, nous cherchons les valeurs qui ne sont pas numérique dans le but de les supprimer et de les remplacer à l'aide de la fonction Interpolate. Ce qui nous donne le graphique suivant :

![alt_text](https://cdn.discordapp.com/attachments/382081589234106389/806099964756230155/unknown.png)

Nous pouvons remarquer que certaines valeurs sont trop disparates par rapport au reste du graphique nous cherchons donc à corriger ses valeurs incohérentes.
Ces valeurs "extrêmes" sont supprimées pour être une fois de plus remplacé grâce à la fonction Interpolate.
Pour cela nous comparons avec des valeurs proches de la saisie erronée dans le but de d'avoir des données se rapprochant de la réalité.

![alt_text](https://cdn.discordapp.com/attachments/382081589234106389/806100030326046730/unknown.png)

Ensuite nous avons compararé notre graphique avec la station météo de Savukoski et nous arrivons avec 2 courbes qui possèdent la même allure nous pouvons donc conclure que notre ficher mystère est une ville d'Europe du Nord.

![alt_text](https://cdn.discordapp.com/attachments/382081589234106389/806100279091003402/unknown.png)

Nous avons donc récupéré les données météo de 4 villes : Prague, Oslo, Helsinki et Moscou
Suite à cela nous avons employé 3 méthodes pour trouver quel serait le meilleur candidat possible.

Dans un premier temps nous avons calculer les moyennes de chaque mois cela nous permet de trouver quelle ville à la plus de similitude avec les données de la ville "inconnue".
Dans ce cas de figure, la ville de Moscou ressort en majorité.

![alt_text](https://cdn.discordapp.com/attachments/382081589234106389/806175487432327178/unknown.png)

Dans un deuxième temps nous avons calculer les différents écart-types de chaque mois pour  pour vérifier notre prédiction ; grâce à cette méthode nous trouvons cette fois la ville d'Oslo, nous avons donc 2 candidats possible nous allons devoir les départager.

![alt_text](https://cdn.discordapp.com/attachments/382081589234106389/806175327248318524/unknown.png)

Pour cela nous avons utilisé la méthode du dynamic time wraping qui nous permet de calculer la distance entre deux courbes en fonction du temps ; plus la valeur est basse, plus la courbe est proche, donc plus les données sont proches de manière générale 
Une nouvelle fois, la ville de Moscou est la plus proche

![alt_text](https://cdn.discordapp.com/attachments/382081589234106389/806175593732505630/unknown.png)

Pour conclure d'après les méthodes que nous avons utilisés la ville de Moscou semble être le meilleur candidat.
