# Blog 

# Semaine 1 : Premières recherches

Lors de notre première séance, nous avons commencé à effectuer des recherches en surface, pour l'instant nous cherchons principalement des pistes et des moyens de s'aiguiller efficacement.
Quels modèles existent déjà ? Dans ces modèles, lequel correspondrait le mieux à notre sujet ? Quels seraient les facteurs importants ? 

Il nous faut donc effectuer des recherches sur plusieurs sites sérieux, tels que wikipédia, primo bsu, github, des thèses et autres. 

Ces recherches sont laborieuses et prennent un temps considérable.

# Semaine 2 : Suite des recherches

Plus concrétement, nous avons continué le travail de recherche plus approfondi et avons pour objectif de commencer l'écriture du code. 

On a maintenant une idée plus claire de comment réaliser le labyrinthe en terme de matrice et nous avons déterminé les règles de la modélisation.

# Semaine 3 : Commencement du codage

Codage des fonctions les plus simples du modèle, pour créer la matrice, placer le blob, placer la nourriture (donc son objectif) et enfin l'implémentation de la fonction d'affichage de la matrice.

Voici ce que ça donne pour l'instant:

![Capture d’écran du 2024-03-29 11-49-03](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231182/b733a601-a910-41ff-a09b-f628b94e0902)

Jaune - BLob

Bleu - Nourriture

# Semaine 4 : Appronfondisement des Parametres

Nous commençons à refléchir à comment le blob va bouger dans la matrice et à coder cela.

Nous avons décidé de créer un labyrinthe dans paint et de l'implémenter dans un notebook jupyter.

![Capture d’écran du 2024-04-05 11-06-26](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231182/594f70bd-a9bb-491f-a64b-bec33065355f)

Nous utilisons le codage de couleur dans l'espace RVB afin de créer une matrice.

Chaque couleur représente des paramètres différents :
- Noir (0,0,0) -  matrice 3 - Les murs du labyrinthe
- Blanc (255,255,255) - matrice 0 - Les déplacements possibles du blob
- Jaune (255,255,0) - matrice 1 - Une cellule du slime
- Bleu (0,0,255) - matrice 2 - La source de nourriture


Voici ce qu'affiche la matrice d'après le labyrinthe qu'on a dessiné:

![Capture d’écran du 2024-04-05 11-17-04](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231182/29440698-00af-4562-88b2-d78776f7ae18)


# Semaine 5 : Déplacements du Blob

Pendant les vacances, on a grandement avancé sur le code.

Pour bouger dans le labyrinthe qu'on a crée, on l'a implementé en terme de matrice:

![Capture d’écran du 2024-04-26 11-36-05](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231182/be429b4c-0a4f-41a0-8a2e-5a72682c0b10)

Le slime et la source de nourriture peuvent maintenant s'étendre dans le labyrinthe. 

L'odeur de la source de nourriture s'étend dans le labyrinthe grace à cette équation qu'on a implémenté dans un notebook jupyter:

![image](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231024/85b62c1b-2fe1-4aef-8765-f37b6cc16590)

Et le slime celui-là:

![image](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231024/277587b6-4d2d-4237-8acb-b9c51e32c733)

Les deux vont ainsi s'étendre jusqu'à ce qu'ils se rencontrent et le slime suivra l'odeur de la nourriture.

# Semaine 6 : Animation Tkinter

[Semaine 6](https://are-dynamic-2024-g4.github.io/croissance-du-blob/semaine6)
