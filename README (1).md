
# algorithmie-grafikart

J'ai pris mon temps pour faire les exercices d'algorithmie et de comprendre leur fonctionnement.

chapitre 1 - Les variables
***
Exercice 1 : *modèle de calcul*
```
    DEBUT
        A = 12
        B = 2
        C = A * B (il multiplie les deux variable C = 24)
    FIN
```
Exercice 2 : *modèle d'inversion*
```
    DEBUT
        A = 12
        B = 2
   
        C = A (C = 12)
        A = B (A = 2)
        B = A (B = 12)
    FIN
```
Exercice 3 : *modèle de calcul*
```
    DEBUT
        A = "123"
        B = "12"
        C = A + B ("12312")
    FIN
```
chapitre 2 - Lecture et écriture
***
Exercice 1 : *modèle pour calculer un prix*
```
    DEBUT
        ECRIRE "entrez le prix de votre objet"
        LIRE PRIXHT (l'utilisateur rentre le prix de son objet HT)
        PRIXTTC = PRIXHT * 1.196 (le prix HT est calculer * 1.196 et on a le prix TTC)
        ECRIRE " PRIX HT" , PRIXHT (lui montre le prix HT)
        ECRIRE " PRIX TTC" , PRIXTTC (lui montre le prix TTC)
    FIN
```
Exercice 2 : *intégrer le .mot. dans une phrase*
```
    DEBUT
        ECRIRE "entre ton Prenom"
        LIRE prenom (l'utilisateur entre son prénom)
        ECRIRE "entre ton Nom"
        LIRE nom (l'utilisateur entre son nom)
        ECRIRE "Bonjour" , prenom, "votre nom est" , nom (la phrase est afficher avec le       
        prénom et nom de l'utilisateur)
    FIN

        (attention! aux erreurs de syntaxe lorsque l'on écrit une phrase il ne faut pas oublier
        le point au début et/ou à la fin selon comment vous intégrer votre mot)
```
chapitre 3 - Les test
***
Exercice 1 : *entrer deux nombre et voir si le résultat est positif ou négatif*
```
    DEBUT
        ECRIRE "entrez votre nombre :"
        LIRE A (l'utilisateur rentre le premier nombre)
        LIRE B (l'utilisateur rentre le deuxième nombre)
        RESULTAT = A * B (les deux nombres sont calculer et donne le resultat)
        SI RESULTAT > 10 ALORS (si le resultat est superieur au nombre c'est positif sinon si c'est inférieur c'est négatif)
        ECRIRE "C'est positif"
        SINON
        ECRIRE "c'est négatif" 
        FINSI
    FIN
```
Exercice 2 : *confirmation de l'âge*
```
    DEBUT
        ECRIRE "Ton age"
        LIRE age (l'utisateur rentre l'âge)

        SI age < 13 ALORS (l'âge est inférieur alor)
        ECRIRE "tu peux allez voir action man"
        SINON SI age >= 13 ET age <= 18 ALORS (si l'âge est supérieur ou égal - inférieur ou égal alor)
        ECRIRE "tu peux allez voir matrix"
        SINON (si il est supérieur alor)
        ECRIRE "tu peux allez voir EVIL DEAD"
        FINSI
    FIN
```
chapitre 4 - Les boucles
***
Exercice 1 : *compter les nombre 0 jusqu'a 10*
```
    DEBUT
        ECRIRE "entrez votre chiffre"
        LIRE chiffre (entrer un chiffre)
        TANTQUE chiffre <= 10 FAIRE (tant que le chiffre est inferieur il continue - si le chiffre est égal alor il arrête)
        ECRIRE chiffre , " " (il affiche le chiffre)
        chiffre = chiffre + 1 (il rajoute 1 tant que le chiffre est inférieur)
        FINTANTQUE
    FIN
```
Exercice 2 : *compter les nombre 10 jusqu'a 0*
```
    DEBUT
        ECRIRE "entrez votre chiffre"
        LIRE chiffre (entrer un chiffre)
        TANTQUE chiffre >= 0 FAIRE (tant que le chiffre est superieur tu continue - si le chiffre est egal alor tu arrête)
        ECRIRE chiffre , " " (il affiche le chiffre)
        chiffre = chiffre - 1 (il retire 1 tant que le chiffre est supérieur)
        FINTANTQUE
    FIN
```
Exercice 3 : *faire deviner un chiffre*
```
    DEBUT
        aDeviner = 12 (chiffre de départ)
        ECRIRE "devine un chiffre"
        LIRE rep (l'utisateur rentre sa reponse)
        TANTQUE rep <> 12 FAIRE (tant que le chiffre est supérieur ou inférieur a la reponse il continue)
        ECRIRE "mauvaise reponse continuer"
        LIRE rep (l'utilisateur continue a rentrer sa réponse)
        FINTANTQUE
        SI rep = 12 ALORS (si l'utilisateur a trouvé la reponse alor)
        ECRIRE "gg"(il lui marque un mot de victoire)
        FINSI
    FIN
```
chapitre 5 - les boucles FOR
***
Exercice 1 : *la boucle pour compter les point*
```
    DEBUT
        POUR point = 0 JUSQU'À 30 FAIRE (La boucle compte jusque 30 et s'arrête quand elle quand elle arrive a 30)
        ECRIRE "voici la liste des point" , point (un texte est rajouter plus la valeur pour l'afficher)  
        FINPOUR
    FIN
```
Exercice 2 : *calculer les valeur en boucle*
```
    DÉBUT
        POUR valeur = 0 JUSQU'À 49 FAIRE (la boucle compte de 0 a 49)
        ECRIRE "calculer" , valeur + 1 (et pour arrivée a 50 on additionne la valeur + 1)
        FINPOUR
        SI valeur <= 50 ALORS (si la valeur est inférieur a tu continue)
        SINON (et si elle est egal alor elle arrête)
        ECRIRE "terminer"
        FINSI
    FIN
```
chapitre 6 - les tableaux
***
exercice 1 : *calcul la valeur total du tableau*
```
    DEBUT
        chiffre = [10,15,20,15,14,8] (le programme calcul le tableau)
        valeur = 0 (la valeur pour chaque element du tableau)
        POUR i = 1 JUSQU'À 6 FAIRE (compte les elemen du tableau)
        valeur = valeur + chiffre[i](la chiffre est ajouter a la valeur)
        FINPOUR
        ECRIRE "la valeur", valeur(affichage de la valeur total)
    FIN
```
Exercice 2 : *donne la note du nombre d'élèves*
```
    DEBUT
        ECRIRE "entrez le nombre d'élève"
        LIRE nombres (le nombre d'élève est rentré)
        ECRIRE "entrez les notes"
        POUR i = 1 JUSQU'À nombres FAIRE 
        LIRE note[i] (chaque note est rentrer pour chaque élève)
        FINPOUR
    FIN
```
Exercice 3 : *si la moyenne est supérieur ou égal des élèves*
```
    DEBUT
        ECRIRE "entrez le nombre d'élève"
        LIRE nombres (le nombre d'élève est rentrer)
        top = 0 (le nombre d'élève qui a la moyenne sera noté)
        ECRIRE "entrez les notes"
        POUR i = 1 JUSQU'À nombres FAIRE (la boucle répête l'opération pour chaque élève)
        LIRE note[i] (on rentre une note)
        SI note[i] >= 10 ALORS (si chaque note rentrée est supérieur ou égal 10 alor)
        top = top + 1 (reprend chaque note entrée)
        FINSI
        FINPOUR
        ECRIRE "votre moyenne est bonne", top (affiche le nombre d'élève qui a la moeynne)
    FIN
```
chapitre 7 - Les tableaux multidimensionnel
***
Exercice 1 : *le programme va chercher la valeur le plus grande du premier tableau dans le second tableau*
```
    DEBUT
        valeur = [[0, 18], [1, 45], [45, 48], [-3, 2]] (les différent valeur du tableau)
        TOP = 0 (chaque valeur sera ajouté)
        POUR i = 1 JUSQU'À 4 FAIRE (calcul les 4 element)
        POUR j = 1 JUSQU'À 2 FAIRE (la boucle va comparé chaque nombre du tableau et voir qu'elle est la plus grande valeur)
        SI valeur[i][j] > top  ALORS (si la valeur est supéreiur alor)
        TOP = valeur[i][j] (il enregistre la valeur)
        FINSI
        FINPOUR
        FINPOUR
        ECRIRE "la plus grande valeur" , TOP (affiche la plus grande valeur)
    FIN
```
chapitre 8 - Les fonction

Exercice 1 : *la fonction compte le nombre de caractere dans un mot*
```
    DEBUT
        ECRIRE "entrez votre mot:"
        LIRE mot (le mot est entrez)
        top = MAX(mot) (la fonction va calculer le nombre de caractère)
        ECRIRE COMPTER (mot) (la fonction compter va faire les total des caractère du mot)
    FIN
```
Exercice 2 : *la fonction fait deviner un chiffre aléatoire*
```
    DEBUT
        aDeviner = ALEATOIRE(99) (la fonction donne un chiffre ALEATOIRE entre 1 a 10)
        ECRIRE "Deviner un nombre"
        LIRE Nombre (l'utilisateur rentre le nombre qui doit deviner)
        TANTQUE Nombre <> aDeviner FAIRE (tant que le chiffre est inférieur ou supérieur au chiffre a deviner il continue)
        SI Nombre < aDeviner ALORS (si l'utilisateur donne un chiffre inferieur alor)
        ECRIRE "plus grand" (il lui ecrit plus grand)
        SINON (si l'utilisateur donne un chiffre supérieur alor)
        ECRIRE "plus petit" (il lui ecrit plus petit)
        FINSI
        LIRE Nombre (il continue a rentrer le nombre)
        FINTANTQUE
        ECRIRE "super vous avez deviné", aDeviner
    FIN
```
chapitre 9 - Les fonction pérsonnalisé
***
Exercice 1 : *comparaison de chiffre*
```
            (module principal)
    DEBUT
        ECRIRE "entrez votre chiffre 'A'" 
        LIRE A (l'utilisateur rentre son premier chiffre)
        ECRIRE "entrez votre chiffre 'B'" 
        LIRE B (l'utilisateur rentre son second chiffre)
        ECRIRE "Le résultat :", COMPARAISON(A,B) (il affiche si c'est vrai ou faux)
    FIN
            (module de comparaison)
    ENTRER A,B (le module va comparer les chiffres )
        retour = 0 ( si c'est faux il retourne 0 )
        SI A <= B ALORS (si a est bien inférieur a b )
        retour = 1 ( si c'est vrai il retourne 1)
        FINSI
    RETOURNER retour (a la fin il retourne la reponse)
```
chapitre 10 - les tris a bulles
***
Exercice 1 : *tri du tableau dans l'ordre*
```
            (module principal)
    DÉBUT
        tab = [15,46,6,54,35,0,23] (controle les nombres du tableau)
        resultat = tab (il donne le resultat qui a dans le tableau)
        i = 1 (initialise le resultat du tableau)
        TANTQUE i < COMPTER(resultat) FAIRE (il compare les element inférieur du tableau)
        SI resultat[i] > resultat[i+1] ALORS ( il compare les elements supéreiur du tableau)
        resultat = PERMUTE(resultat, i) (prend le resultat de operation qu'il tri)
        i = 0
        FINSI
        i = i + 1
        FINTANTQUE
        ECRIRE tab 
        ECRIRE resultat
    FIN

            (module permute)
    ENTRER tab, index (chaque element du tableau sera comparer)
        tmp = tab[index]
        tab[index] = tab[index + 1]
        tab [index+1] = tmp 
    RETOURNER tab
```


