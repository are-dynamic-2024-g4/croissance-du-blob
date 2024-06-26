## Compte rendu de la semaine 4

Nous nous intéressons maintenant aux déplacements.

On a dû relire les explications des sources plusieurs fois pour comprendre exactement ce qu'il fallait faire pour les déplacements.

Et nous avons décidé que les deux, le blob et l'odeur de la nourriture, allaient s'étendre dans le labyrinthe jusqu'à ce qu'ils se rencontrent.

Afin de bouger, le matrice sera vue comme ceci : 

![Screenshot 2024-04-30 184747](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231182/3fdeed10-906d-4ed9-ad00-89ec0a3e9f43)

Le slime ou l'odeur pourra ainsi se propager soit au nord, nord-est, est, sud-est, sud, etc...

# Les constantes qu'on a défini :

![Screenshot 2024-04-30 195104](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231182/f717d870-3554-403b-887d-f6d513ffe0b0)

PMP1, PMP2 - Diffusion du slime.

CAP1, CAP2 - Pourcentage minimum de l'odeur détecté par le slime. 

CON - Le pourcentage de nourriture absorbé par le slime.

PA - L'attraction du slime par l'odeur de la nourriture.

PAP - Constante associé à une direction. Si le slime bouge (ex. Nord), la cellule vers laquelle il se dirige est égale à PAP et la cellule adjacente (Sud) est égal à -PAP.

# Les paramètres utilisés dans les équations :

PMvNN - Contribution du voisinage de von Neumann pour la masse du slime sur cellule [i][j]. C'est-à-dire, si le slime peut bouger au nord, est, sud ou ouest.

PMeMN - Contribution du voisinage de Moore pour la masse du slime sur cellule [i][j]. C'est-à-dire, si le slime peut bouger au nord-est, sud-est, nord-ouest ou sud-ouest.

PM - Masse de slime totale à t+1 sur la case [i][j].

CHAvNN - Contribution du voisinage de von Neumann pour la diffusion de l'odeur sur la case [i][j].

CHAeMN -  Contribution du voisinage de Moore pour la diffusion de l'odeur sur la case [i][j].

CHA - L'attraction chimique (l'odeur de la nourriture) sur la case [i][j].

AA - Case vide

![Screenshot 2024-04-30 191420](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231182/10d61b25-35db-4c54-9e7d-8a1f91d2a259)


![Screenshot 2024-04-30 191435](https://github.com/are-dynamic-2024-g4/croissance-du-blob/assets/160231182/cc9548bf-edef-430c-b184-6aa84e6b4106)


[Semaine 3](https://are-dynamic-2024-g4.github.io/croissance-du-blob/semaine3) <- Précedent ... Suivant -> [Semaine 5](https://are-dynamic-2024-g4.github.io/croissance-du-blob/semaine5)

