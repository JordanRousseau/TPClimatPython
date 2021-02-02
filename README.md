# TPClimatPython
Nous avons tout d'abord traiter le fichier climat mois par mois. Dans le but d'avoir 12 courbes

![alt text](https://cdn.discordapp.com/attachments/382081589234106389/806093813515812874/unknown.png)


Ensuite nous avons réalisé le graphique pour assembler pour avoir toutes les températures de l'année. Nous avons également du retirer les valeurs nulles pour éviter d'avoir des trous dans notre affichage. 

![alt text](https://cdn.discordapp.com/attachments/382081589234106389/806095497944236032/unknown.png)

Nous avions également un deuxième fichier qui comprennait des erreurs nous devions les isoler puis les corriger, à l'aide d'une expression regex, nous cherchons les valeurs qui ne sont pas numérique Pour les supprimer et les changer à l'aide de la fonction Interpolate. Ce qui nous donne le graphique suivant :

![alt_text](https://cdn.discordapp.com/attachments/382081589234106389/806099964756230155/unknown.png)

Nous pouvons remarquer que certaines valeurs sont trop disparate par rapport au reste du graphique nous cherchons donc à corriger ses valeurs incohérentes.

![alt_text](https://cdn.discordapp.com/attachments/382081589234106389/806100030326046730/unknown.png)

Ensuite nous avons compararé notre graphique avec la station météo de Savukoski et nous arrivons avec 2 courbes qui possède la même allure nous pouvons donc conclure que notre ficher mystère est une ville d'Europe du Nord. 

![alt_text](https://cdn.discordapp.com/attachments/382081589234106389/806100279091003402/unknown.png)
