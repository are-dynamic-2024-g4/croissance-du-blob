## Compte rendu de la semaine 5

Nous avons continuer avec le codage.

Ainsi on se retrouve avec ses étapes pour executer le deplacement du slime et l'odeur dans le labyrinthe.

## Etape pour le deplacement

# 1. Initialiser le modèle
     Les paramètres des équations de diffusion sont défini.
     La topologie des points de départ et des sources de nourriture sont introduit grâce à un array depuis une image.

# 2. Appliquer les équations de diffusion pendant 50 itérations (t)
     Vérifier si les sources de nourritures sont couvertes avec un pourcentage prédéfini de masse du slime.
     Si au moins une source de nourriture est couverte -> Passer à l'étape 3
     Si aucune source de nourriture n'est couverte ->  Boucler l'étape 2 

# 3. Creation de tube
    Toutes les sources de nourriture couvertes avec le pourcentage prédéfini de masse du slime (thPM) sont encapsulés par le blob.
    Ils sont ensuite connectées au point de départ, SP (le point de départ du slime).
    Ces derniers se transforment ensuite en point de départ, ce qui veut dire que leur masse de slime est définie à 100.

# 4. t = 5000 itérations?
     On vérifie s'il y a eu 5000 itérations:
     * t < 5000
       - si t = 5000 -> On change les NS et SP en NS (le point de depart des sources de nourriture, intiallement égale à 100) 
                     -> On change l'avant dernier NS en SP.
       - Boucler l'étape 2

     * t > 5000
       - t < 10000 ?
          Si oui, on arrête la boucle.
          Si non, on reboucle à l'étape 2.


PM (masse de slime) vaut :

0 si la case n'est pas une case accessible.

100 si la case est un point de départ, SP.

100 si la case est une source de nourriture ET que la masse de slime sur cette case est supérieure au pourcentage de masse nécessaire prédefini, PMP.


On a ensuite fait une liste des problèmes qui pourrait apparaître lors du simulation tels que "Si le slime bouge endehors du labyrinthe", "S'il fait face a un mur", "S'il y a plusieurs sources de nourriture" ou encore "s'il y a des obstacles sur son chemin".

Ainsi on a fait plusieurs autres fonctions afin de résoudre telles problèmes.

# Ex.1
![Screenshot 2024-05-01 000437](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231182/87ef90f8-b1d7-4a87-9a9a-967fdd316205)

Vérifie que l'image implémenter et conforme au contrainte que nous avons créer.


# Ex.2
![Screenshot 2024-05-01 000844](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231182/9fe574f5-039e-43e6-bd4d-c883028792cb)

Vérifie qu'une case existe bien dans la matrice.



Suivant: [Semaine 6](https://are-dynamic-2024-g4.github.io/croissance-du-blob/semaine6)



