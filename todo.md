## Déroulement du jeu


## Options
[ ] Personnalisation taille gris

[ ] Personnalisation nombre bateaux (a partir de presets)

[ ] Tirs normaux ou tirs par salves

[ ] Options afin d'empêcher de placer des bateaux cotes a cotes

## Jouabilité
[ ] Placement des bateaux à la souris

[ ]

## Boucle de gameplay

## régles du jeu

### régle

2 joueur

#### objectif 

couler tout les bateaux du joueur adverse.

#### placement

la partie commence avec une phase de placement, les deux joueur aurons devant eux une grille de taille definit dans les parametres. Il aurons des bateaux (definit par les parametres) a placé sur leur grille (les régles de placement varie selon les paramètres), une fois tout les bateaux placé la partie demarre.

#### déroulement (partie normal)

le joueur actif a une grille devant lui avec les cases ou il a déjà tiré et les case encore inconnu, le joueur voit aussi les cases ou il a touché quelque chose.
Le joueur choisi l'emplacement de sa prochaine salves sur la grille (sur une case encore inconnu) et valide son choix.
le jeu dis si le joueur a touché, a coulé ou a tiré dans l'eau

la partie continue avec le prochain joueur.

#### variante salves

si l'option tire par salve est activé le joueur pourra tiré autant de salve que de bateaux qui lui reste, cependant il ne saura pas ou il a touché selement ou il a déjà tiré et au moment de l'annonce du touché il aura en plus le nombre de salve qui on touché.

#### fin de partie

une fois qu'un des deux joueur a touché toute les cases contenant un bateau adverse le jeu se termine, le vaiqueur est celui qui a encore des bateaux non coulé.

### source

https://methodeheuristique.com/wp-content/uploads/2018/05/bataille-navale-2.pdf

https://fr.wikipedia.org/wiki/Bataille_navale_(jeu)

https://www.joueclub.fr/contenu/la-bataille-navale-un-jeu-simple-et-toujours-amusant.html


### Gameplay loop
- ecran titre
- Demander aux joueurs les paramètres
- Confirmer les paramètres (pas qu'il y a des paramètres incompatibles)
- Demander aux joueurs de placer les bateaux (pour tous les joueurs:)
	- Placer les bateaux (click sur un bateau = selectionner, click sur la grille le place, molette pour tourner + preview)
	- Retirer des bateaux si besoin si l'on clique dessus
	- Confirmer
	- Afficher un écran de confirmation (noir sans info) pour passer les controles au joueur 2
- Boucle de gameplay
	- Pour chaque joueur:
		- Afficher écran "joueur pret", avec demande confirmation
		- Afficher les grille du joueur
		- le joueur place ses salves
		- Autoriser le joueur a tirer (une ou plusieurs fois)
		- Afficher le nombre de bateau detruit
- Fin du jeu
	- Afficher écran victoire
	- Affichers options:
		- Rejouer
		- Modifier les règles
		- Quitter le jeu
		- (ou retour a l'écran titre dans le cas ou il est ajouté)
