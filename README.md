# TPClimatPython
Nous avons tout d'abord traiter le fichier climat mois par mois. Dans le but d'avoir 12 courbes pour chaque mois. Cela nous permet d'avoir une vision global de nos donnés ainsi que les bornes des températures cela nous sera utile pour la suite.

![alt text](https://cdn.discordapp.com/attachments/382081589234106389/806093813515812874/unknown.png)

Ensuite nous avons réalisé le graphique pour assembler afin d'avoir toutes les températures de l'année. Nous avons retiré les valeurs nulles pour éviter d'avoir des trous dans notre graphique. Nous obtenons la courbe suivante :

![alt text](https://cdn.discordapp.com/attachments/382081589234106389/806095497944236032/unknown.png)

Nous avions également un deuxième fichier qui comprennait des erreurs nous devions les isoler puis les corriger, à l'aide d'une expression regex, nous cherchons les valeurs qui ne sont pas numérique dans le but de les supprimer et de les remplacer à l'aide de la fonction Interpolate. Ce qui nous donne le graphique suivant :

![alt_text](https://cdn.discordapp.com/attachments/382081589234106389/806099964756230155/unknown.png)

Nous pouvons remarquer que certaines valeurs sont trop disparates par rapport au reste du graphique nous cherchons donc à corriger ses valeurs incohérentes. Pour cela nous comparont avec des valeurs proches de la saisie eroné dans le but de d'avoir des données se raprochant de la réalité 

![alt_text](https://cdn.discordapp.com/attachments/382081589234106389/806100030326046730/unknown.png)

Ensuite nous avons compararé notre graphique avec la station météo de Savukoski et nous arrivons avec 2 courbes qui possède la même allure nous pouvons donc conclure que notre ficher mystère est une ville d'Europe du Nord. 

![alt_text](https://cdn.discordapp.com/attachments/382081589234106389/806100279091003402/unknown.png)
