## Compte rendu de la semaine 6

Enfin pour cette dernière semaine, on s'est intéressé à l'animation de notre projet sur Tkinter et les métriques qu'on a décidé de modifier.

On a d'abord dû faire des recherches sur comment utilser Tkinter qui nous ont pris plus de temps qu'on ne le souhaitait, mais on a finalement pû le comprendre et l'implémenter.

Ce qui à la fin nous a donné cette animation.

![Screenshot 2024-05-02 164050](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231182/b9d07973-d6cb-4be5-8e80-2d935aeda069)


Comme dit précedemment, le jaune est le blob, et le bleu la source de nourriture.


https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231182/b18a66e4-95c1-472c-8230-b311c0c32e40


Comme vue dans la video, le slime s'est propagé dans le labyrinthe en entier jusqu'à la source de nourriture.

En violet est le chemin finale trouvé par le slime, et les cases en vert sont des cellules avec les concentrations de slime restantes, inférieure à 100.

A la fin de la video, la source de nourriture qui était bleu au début est devenue jaune car la case avait désormais 100% de concentration de slime. En d'autres termes, le slime a mangé la nourriture.

# Autres Simulations

**Test**

https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231182/4305edf1-104a-4e82-ad4e-d79290dd29da



# Métriques
![image](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231024/b5eb5e80-e782-481c-8d88-5d562122e0ba)

![image](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231024/646a4496-1b43-42a5-9b64-88ca7ad5c947)

 Les paramètres de diffusion influent avec des poids différents. Le plus intéressant à regarder est PMP1.
 Ces deux courbes ont été réalisés sur la map5.png, qui représente le labyrinthe comme présenté en laboratoire.
 En-dessous de 0.02, la masse de slime en fin de simulation est assez faible et croît lentement, ce qui peut indiquer une diffusion plutôt mauvaise en dessous de ce seuil.
 Egalement, on voit que notre algorithme aura besoin de plus d'itérations avec un PMP1 plus faible, m^me dans une configuration pourtant assez simple.
 On peut donc viser un PMP1 assez elevé pour avoir une bonne diffusion et également un algorithme assez rapide.


[Semaine 5](https://are-dynamic-2024-g4.github.io/croissance-du-blob/semaine5) <- Précedent
