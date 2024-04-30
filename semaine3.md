## Compte rendu de la semaine 3

On a dû rechercher d'autres commandes et des videos pour mieux comprendre comment se servir de jupyter.

A la fin de notres recherches, on trouver une façon de convertir une image directement en matrice:

![Screenshot 2024-04-30 182253](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231182/ab2ee9cd-9684-473e-8c9d-826715d79dc6)

On a utilisé cette image de labyrinthe qu'on a crée sur paint;

![Screenshot 2024-04-30 182651](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231182/232d6747-b1b3-489a-999b-8992ed0b1d7a)

Qui donne à la fin une matrice de ce genre;

![Screenshot 2024-04-30 182829](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231182/58f55960-1e18-417b-9c6f-6babc10ab161)


Mais comme vous pouvez le constater, il est facile de se perdre parmis tous ces arrays donc on a normaliser la matrice.

Nous utilisons le codage de couleur dans l'espace RVB afin de créer la nouvelle matrice.

Chaque couleur représente des paramètres différents :
- Noir (0,0,0) -  matrice 3 - Les murs du labyrinthe
- Blanc (255,255,255) - matrice 0 - Les déplacements possibles du blob
- Jaune (255,255,0) - matrice 1 - Une cellule du slime
- Bleu (0,0,255) - matrice 2 - La source de nourriture

![Screenshot 2024-04-30 183117](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231182/b09d6ea5-a4ff-4f44-9920-e26f9aa12287)

En l'occurence comme vous le voyez dans l'image ci dessus, on n'a que des 3 (mur) et des 0 (case vides) mais ni de 1 ou 2 malgré qu'on n'a du bleu et jaune dans l'image.

Cela est dû au fait que le bleu et jaune dans l'image n'ont pas le même représentation en RVB. 

On a ainsi ajouté ce problème à une liste de touts les erreurs ou conditions qu'on peut résoudre plus tard ou au quelles on doit faire attention.


Suivant: [Semaine 4](https://are-dynamic-2024-g4.github.io/croissance-du-blob/semaine4)

