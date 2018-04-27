Airbnb - Analyse des données de locations d’appartements à NY


Ce travail est un modèle basé sur une base de données d'appartements en location sur Airbnb à NY qui inclut les éléments suivant: le prix, les nombres de chambres, le type de lit, la localisation, la note. Cette base de données prend en compte la saisonnalité des données.
Les données brutes contiennent plus de 27000 données.

L’architecture de ce programme se décompose en trois dossiers :
- BDD-Airbnb :ce dossier contient le programme « Manipulation des données »
- opinion-lexique : ce dossier contient deux fichiers texte contenant des mots à connotations négatives dans le premier fichier, et positives dans le deuxième fichier
- BDD-brute : ce dossier contient trois fichiers csv « groupe_mots », « reviews » et « liste-données ». 

Le programme « Manipulation des données » contient :
- La partie data cleaning
- La partie sentiment analysis

Concernant la partie data cleaning, nous avons enlevé les valeurs incohérentes qui se trouvaient dans le fichier (NaNs) et les valeurs nulles. Le programme génère un nouveau fichier csv nettoyé. Nous avons aussi rajouté un graphe qui permet de visualiser la distribution des prix des locations Airbnb à NY.

Concernant la partie sentiment analysis, cette partie nous a permis de quantifier les commentaires laissés par les utilisateurs sur les appartements en location. Nous avons essayé de voir en quoi ces commentaires peuvent impacter les prix. Nous avons donc calculé la polarité des mots positifs et négatifs en deux méthodes, TextBlob et par méthode manuelle. On a classifié les différents segments des commentaires pour voir s’ils étaient dans l’ensemble positifs ou négatifs à partir de la liste de mots « opinion-lexique ». Les résultats obtenus sont très différents pour ces deux méthodes. Nous pensons pouvoir attribuer ces différences à la non exhaustivité des listes de mots positifs et négatifs que nous avons utilisés.
# Projet-Airbnb-DAC
