
## 1. Qu'est ce que lE GIl

Le GIL est un sytème qui empèche plusieurs threads python de s'éxecuter en même temps. Il a été ajouté dans les premiers jours de python pour permettre aux bibliothèques de mieux fonctionner. 

En effet à l'époque les OS géraient mal le multithreading et ça causait problème avec un grand nombre de bibliothèque en particulier celles écrit en C. 

## 2. Temps pris avec et sans le gil 

Avec le gil l'exercice prends 5.359347105026245 s

Sans le gil l'exercice prends 4.41986608505249 s

L'exécution est beaucoup plus rapide sans le gil, d'autant que le travail n'est vraiment pas complexe donc la différence devrait augmenter rapidement avec la complexité.

## 3. applications dans la vie réelle avec accès à une même variable

Dans la vraie vie deux threads peuvent avoir besoin d'accèder à la même variable par exemple dans un word, il y a un thread qui s'occupe de vérifier l'orthographe et un thread qui s'occupe de l'affichage sur l'écran. 