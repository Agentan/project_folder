Il y a deux fichiers : main.py et tableau.py . Après avoir téléchargé les deux fichiers, il suffira d'exécuter main.py .

Il vous sera alors indiqué de choisir entre deux cas : "première requête / renouvellement de la base de données" ou bien " requête supplémentaire sur la même base de données" .

Dans le premier cas, il vous sera demandé d'indiquer le chemin de la base de données où vous souhaitez effectuer la recherche. ATTENTION : pour des bases de données de plus de 5 MB, la création de l'index prend environ une minute. Cependant, une fois l'index construit, la recherche elle-même est toujours très rapide.

Ensuite vient le moment où vous pouvez entrer votre requête pour recherche des articles à partir de mots clés. Notre moteur de recherche est sensible à la casse des caractères. Il discrimine les articles de la base de données principalement à partir des mots qui ont, a priori, le plus d'importance dans la requête (et non pas à partir de mots très courants comme "le", "la", "de", "et", ...).

Si vous souhaitez décider vous-même de l'emplacement où seront enregistrés les index, vous pouvez écrire le chemin du dossier où vous désirez effectuer la sauvegarde à la ligne 6 à la place de 'os.getcwd()' . Par défaut, la commande 'os.getcwd' indique le chemin du dossier contenant le fichier main.py au moment de l'exécution.


