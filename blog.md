# Blog 

# Semaine 1 : Premières recherches

Lors de notre première séance, nous avons commencé à effectuer des recherches en surface, pour l'instant nous cherchons principalement des pistes et des moyens de s'aiguiller efficacement.
Quels modèles existent déjà ? Dans ces modèles, lequel correspondrait le mieux à notre sujet ? Quels seraient les facteurs importants ? 

Il nous faut donc effectuer des recherches sur plusieurs sites sérieux, tels que wikipédia, primo bsu, github, des thèses et autres. 

Ces recherches sont laborieuses et prennent un temps considérable.

# Semaine 2 : Suite des recherches

Plus concrétement, nous avons continué le travail de recherches plus approfondis et avons pour objectif de commencer l'écriture du code. 

On a maintenant une idée plus claire de comment réaliser le labyrinth en terme de matrice et nous avons déterminé les règles de la modélisation.

# Semaine 3 : Commencement du codage

Codage des fonctions les plus simples du modèle, pour créer la matrice, placer le blob, placer la nourriture (donc son objectif) et enfin l'implémentation de la fonction d'affichage de la matrice.

Voici ce que ça donne pour l'instant:

![Capture d’écran du 2024-03-29 11-49-03](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231182/b733a601-a910-41ff-a09b-f628b94e0902)

Jaune - BLob

Bleu - Nourriture

# Semaine 4 : Appronfondisement des Parametres

Nous commençon à refléchir et coder comment le blob vas bouger dans la matrice.

Nous avons décider de creer un labyrinthe dans paint et l'implementer en jupyter

![Capture d’écran du 2024-04-05 11-06-26](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231182/594f70bd-a9bb-491f-a64b-bec33065355f)

Nous utilisons le codage de couleur dans l'espace RVB afin de creer une matrice.

Chaque couleur represente des differentes parametres:
- Noir (0,0,0) -  matrice 3 - Les murs du labyrinthe
- Blanc (255,255,255) - matrice 0 - Les deplacements possibles du blob
- Jaune (255,255,0) - matrice 1 - une cellule du slime
- Bleu (0,0,255) - matrice 2 - La source de nourriture


Voici cec qu'affiche la matrice d'après le labyrithe qu'on a dessin:

![Capture d’écran du 2024-04-05 11-17-04](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231182/29440698-00af-4562-88b2-d78776f7ae18)


# Semaine 5 : Deplacements du Blob

Pendant les vacances, on a grandement avancé sur le code.

Pour bouger dans le labyrinthe qu'on a creé, on l'a implementé en terme de matrice:

![Capture d’écran du 2024-04-26 11-36-05](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231182/be429b4c-0a4f-41a0-8a2e-5a72682c0b10)


Le slime et la source de nourriture peuvent maintenat s'étendre dans le labyrinthe. 

Le slime utilise cette equation que nous avons implementer en jupyter:

![Capture d’écran du 2024-04-26 11-37-27](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231182/12d1005a-41d2-406f-bb67-68df6a9183d9)

![Capture d’écran du 2024-04-26 11-37-42](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231182/cef01be5-3dbe-49e1-96e8-3a8becd0ce7c)


Nous avons décider de les étendre tous les deux ainsi, des qu'ils se rencontrent, le slime suivra "l'odeur" de la nourriture jusqu'à ce qu'il le trouve.
