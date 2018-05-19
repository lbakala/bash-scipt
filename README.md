# Bash-scipt
Écrire un script qui permette de copier un fichier vers un répertoire de stockage.

Syntaxe : copier fichier répertoire suffixe
##  Objectif :
Le but de ce programme est de copier le fichier donné, dans le répertoire donné, 
le fichier copié portera le nom du fichier d'origine augmenté du suffixe. 
 Exemple :

    $copier fic1 rep2 abcd
    $ ls -l rep2
    -r--------. 1 user1 user1 1217 31 oct. 11:58 fic1.abcd

## Opérations :
 - Tester la syntaxe.

> Si elle n'est pas correcte (manque un ou plusieurs paramètres) passer
> en mode interactif (~dupliquer).

 - Tester si le fichier existe, si on a le droit de lecture.

> Si ce n'est pas le cas afficher un message d'erreur (1) et demander à l'opérateur 
> de choisir un autre fichier. Au bout de trois propositions incorrectes 
> afficher un message d'erreur et abandonner le programme. (1)

- Tester si le répertoire existe.

> S'il n'existe pas demander si on doit le créer. (2) 
> Vérifier la création du répertoire, si impossibilité afficher un message 
> d'erreur et sortir du programme. (1)

 - Tester si on a le droit d'écriture dans le répertoire.

> Si pas de droit d'écriture sur le répertoire proposer de changer les droits du répertoire (2). 
> Si la réponse est négative afficher un message et sortir du programme. (1) 
> Avant d'effectuer la copie demander confirmation. (2)
>  Effectuer la copie du fichier. Modifier les droits sur le fichier sauvegardé afin que 
>  seul le propriétaire ait le droit de lecture (et rien d'autre !)

.
Afficher, au format long, les caractéristiques du fichier sauvegardé en habillant le résultat avec
commentaires et mise en forme.
## Remarques :
       (1)Les sorties sur erreur donnent lieu à un code de retour «FAUX»
       (2)Les réponses attendues sont « oui » ou «non». 
        Si la réponse est « oui » on continue.
        Si la réponse est « non » on abandonne le programme en affichant un message de politesse.
        Si la réponse est ni « oui » ni « non » redemander. Au bout de trois réponses incomprises
        avertissez l'opérateur que l'on abandonne le programme.




