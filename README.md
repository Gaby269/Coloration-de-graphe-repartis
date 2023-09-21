# Projet de Coloration de graphe HADDAD Gatien, POINTEAU Gabrielle

L'idée de ce projet était de pouvoir colorier un graphe où les noeuds sont des clients reliés entre eux par des sockets. Nous devions les colorer de telle façon à ce qu'un noeud soit d'une couleur différente par rapport à ses voisins.

Pour cela, nous avons mis en place la connexion entre les clients à l'aide d'un serveur et puis nous les avons connectés entre eux pour qu'il soit autonome et trouve leur couleur.

Vous verrez donc dans le dossier [code](https://github.com/Gaby269/Coloration-de-graphe-repartis/tree/main/Code) les différents fichiers que nous utilisons.

## Liste des fichiers :

- [***graphes :***](https://github.com/Gaby269/Coloration-de-graphe-repartis/tree/main/Code/graphes) dossier contenant les différents fichiers de graphes que nous utilisons pour tester le programe, ces fichiers sont issues du site : [http://cedric.cnam.fr/~porumbed/graphs/](http://cedric.cnam.fr/~porumbed/graphs/). Il y a également les deux photos utilisées pour illustrer nos exemples dans le rapport.
- [***bin***](https://github.com/Gaby269/Coloration-de-graphe-repartis/tree/main/Code/bin) et [***obj***](https://github.com/Gaby269/Coloration-de-graphe-repartis/tree/main/Code/obj) : dossiers de compilation et d'éxécution des scripts.
- [***script***](https://github.com/Gaby269/Coloration-de-graphe-repartis/tree/main/Code/scripts) : dossiers des programmes utilisé pour réaliser le projet
  - [*cleaner.py*](https://github.com/Gaby269/Coloration-de-graphe-repartis/blob/main/Code/scripts/cleaner.py) : fichier permettant de supprimer les processus en cours d'éxécution lancé depuis *bin/noeud* et *bin/serveur* mais qui sont inutils
  - [*fonction.c*](https://github.com/Gaby269/Coloration-de-graphe-repartis/blob/main/Code/scripts/fonctions.c) : fichier qui regroupe toutes les fonctions pour la mise en place d'une connection entre deux noeuds (clients, serveur) avec le protocole TCP, et les focntions de coloration de noeud util pour le projet
  - [*noeud.c*](https://github.com/Gaby269/Coloration-de-graphe-repartis/blob/main/Code/scripts/noeuds.c) : fichier pour montrer le déroulé de ce que fait un noeud pour se connecter à tous les autres noeuds et se colorer en fonction de ses voisins
  - [*parser.c*](https://github.com/Gaby269/Coloration-de-graphe-repartis/blob/main/Code/scripts/parseur.c) : parser des fichiers de graphe pour pouvoir les utiliser dans notre code
  - [*serveur.c*](https://github.com/Gaby269/Coloration-de-graphe-repartis/blob/main/Code/scripts/serveur.c) : fichier pour montrer le déroulé de ce que fait le serveur pour mettre en place la connection de tous les noeuds entre eux
  - [*structures.c*](https://github.com/Gaby269/Coloration-de-graphe-repartis/blob/main/Code/scripts/structures.c) : fichier de toutes les structures utilisés dans le code
  
