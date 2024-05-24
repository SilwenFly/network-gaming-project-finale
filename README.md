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

# Notes :
## Célestine
Je met "Add" en commentaire à coté des lignes de code que je modifie pour pouvoir les retrouver facilement en Ctrl F  
La vérification que le bob nous appartient bien pour lui faire faire une action se fait vers la ligne 250 de gameControl.py (dans la boucle de jeu, au moment de faire faire une action à un bob) et pas dans chaque fonctions des bobs  
Modification faite : on ne peut faire faire une action qu'à ses bob, les bobs ne mangent pas les copains et ne font des bébés que entre bobs du même propriétaire  

## Florine 
J'ai créé une fonction `initiateOtherBobs` dans le fichier GameControl.py. Cette fonction servira à afficher les Bobs de l'autre joueur en modifiant l'attribut : `self.isMine`. Cela permet donc de changer la couleur des Bobs : *bleu* quand ils nous appartiennent, *vert* sinon. 
