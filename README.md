# IA-reconnaissance-de-nombre

Le dossier est composé de 3 morceaux de codes :
* setup.py -> initialiser aléatoirement les poids et les bias
* entrainement.py -> entraîner l'IA
* test.py -> tester l'IA

Ainsi que de plusieurs fichiers :
* Le dossier 'pack' contient une liste d'image de chiffre ainsi que leur valeur (pris sur le site du MNIST)
* Les fichiers txt qui sont les sauvegardes des poids et des bias
    
L'IA est codé en python avec les bibliothèques suivantes :
* numpy
* time 
* math
* tqdm
* random
    
L'IA fonctionne grâce à 45 réseaux de neuronnes indépendants comportant chacun 784 neuronnes d'entrées, 2 fois 16 neuronnes cachés, 2 neuronnes de sortie.
Chaque réseau a pour but de trouver si l'image est un chiffre ou un autre, (par exemple, le premier réseau devine si l'image est un 0 ou un 1).
À la fin, l'IA regarde parmis les 45 réseaux le chiffre qui a été le plus ressorti.
     
Pendant l'entraînement, l'IA connaît déjà la valeur de l'image, elle fait donc fonctionner que 9 réseaux différents et les améliore.
