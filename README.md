*Ce fichier peut servir à noter nos questions ou réflexions ainsi que nos avancées d'ici la fin du projet.*  

# Rôles :

## Partie Python
Florine : affichage des bobs des autres joueurs  
Yoann : envoie des infos aux autres  
Julian : Reception  
Célestine : Notion de propriété  

## Partie Reseau
Titouan : python - C & C - python  
Delong : C - C  

# Consignes
Chaque joueur à une copie locale du jeu pour visualiser la simulation et placer ses bobs/sa nourriture  
Les modifications locale des joueurs sont envoyées aux autre joueur pour qu'il mettent a jour leur copie locale  
Il est acceptable qu'un joueur voit les mouvements d'un autre avec un peu de retard  
Un joueur a acces aux caractéristiques des entitées des autres joueurs
Les entitées (bobs et nourriture) ont une propriété metier, les objets du jeu (case, bobs et nourriture) ont une propriété réseau
-Propriété métier : a qui ça appartient
-Propriete réseau : qui y a acces temporairement
Concurence sur les objets : plusieur bob ont acces aux mêmes nourriture mais attention ils ne peuvent pas manger deux fois la même nourriture

# Notes :
## Célestine
Je met "Add" en commentaire à coté des lignes de code que je modifie pour pouvoir les retrouver facilement en Ctrl F  
La vérification que le bob nous appartient bien pour lui faire faire une action se fait vers la ligne 250 de gameControl.py (dans la boucle de jeu, au moment de faire faire une action à un bob) et pas dans chaque fonctions des bobs  
Modification faite : on ne peut faire faire une action qu'à ses bob, les bobs ne mangent pas les copains et ne font des bébés que entre bobs du même propriétaire  

## Florine 
J'ai créé une fonction `initiateOtherBobs` dans le fichier GameControl.py. Cette fonction servira à afficher les Bobs de l'autre joueur en modifiant l'attribut : `self.isMine`. Cela permet donc de changer la couleur des Bobs : *bleu* quand ils nous appartiennent, *vert* sinon. 
