# Module 02 - Débutons, à vos crayons !

Ces exercices ont pour objectifs :

- l'évaluation d'expressions
- écriture d'algorithmes simples avec entrées / sorties et variables

## Exercice 1 - Opérations booléennes

Avec les données initiales :

- ```booléen x = vrai```
- ```booléen y = faux```
- ```booléen z = vrai```

Évaluez les expressions suivantes :

1. ![$x \land y$](https://render.githubusercontent.com/render/math?math=%24x%20%5Cland%20y%24)
2. $y \lor x$
3. $x  \lor z \lor y$
4. $y \lor (x \land z)$
5. $y \lor \lnot x$
6. $\lnot x \land y$
7. $(\lnot y \land \lnot x) \lor x$

<details>
    <summary>Idée #1</summary>
    Remplacez les variables par leurs valeurs et effectuez le calcul.
</details>

<details>
    <summary>Idée #2</summary>
    Relisez votre cours afin de connaitre le résultat des différents opérateurs (tables de vérités).
</details>

## Exercice 2 - Évaluations plus complexes

Avec les données initiales :

- ```entier x = 10```
- ```entier y = 5```
- ```entier z = 1```

Évaluez les expressions suivantes :

1. $(X > Y) \lor (Z > 1)$
2. $(X / 2 >= Y) \land (Y == 5)$
3. $\lnot(X > 10) \lor (Z > 1)$
4. $(3 * Z * Y == X + Y) \land (X * 5 == Y * 10)$
5. $\lnot( (10 * X - Y == 95) \land (X - Y == Z * 5) )$
6. $(X \% 3 == Y \% 2) \land (Z \% 2 == 2)$
7. $(X / 3 > 3) \lor (Y / 3 > 1)$

<details>
    <summary>Idée #1</summary>
    Remplacez les variables par leurs valeurs et effectuez le calcul.
</details>

<details>
    <summary>Idée #2</summary>
    Relisez votre cours afin de connaitre le résultat des différents opérateurs. Attention au type des valeurs, ici c'est le type entier et non réel.
</details>

## Exercice 3 - Salutations

Écrivez un algorithme qui lit le nom de l’utilisateur et qui lui affiche le texte "Bonjour " suivi du nom.

<details>
    <summary>Idée #1</summary>
    Relisez le problème afin d'extraire les mots importants. Relisez ensuite votre cours afin d'extraire les instructions utiles pour le résoudre.
</details>

<details>
    <summary>Idée #2</summary>
    Avez-vous besoin d'une variable pour stocker de l'information ?
</details>

<details>
    <summary>Proposition solution</summary>

``` csharp
chaine nomUtilisateur = "";

écrire("Veuillez entrer votre nom svp : ");
nomUtilisateur = lire();

écrireNL("Bonjour " + nomUtilisateur);
```
</details>

## Exercice 4 - Dé

Écrivez un algorithme qui affiche à l’utilisateur un nombre tiré au hasard compris entre 1 et 6.

<details>
    <summary>Idée #1</summary>
    Regardez votre cours sur la génération des nombres aléatoires. Vous faut-il une variable ?
</details>

<details>
    <summary>Proposition solution</summary>

``` csharp
entier nombreTire = genererNombre(1, 7);

écrireNL("Le nombre choisi est " + nombreTire.VersChaine());
```
</details>

## Exercice 5 - Divisions

Écrivez un algorithme qui lit deux nombres entiers et qui affiche le quotient et le reste de la division entière.

<details>
    <summary>Idée #1</summary>
Posez-vous les questions suivantes : 
<ul>
 <li>comment est-ce que je ferais pour afficher le quotient et le reste de la division entière</li>
 <li>quelles sont les données dont j'ai besoin ?</li>
 <li>de quel(s) type(s) sont-elles ?</li>
</ul>
</details>

<details>
    <summary>Idée #2</summary>
Relisez la partie du cours spécifique aux opérateurs sur les entiers.
</details>

<details>
    <summary>Proposition solution</summary>

``` csharp
entier dividende = 0;
entier diviseur = 0;
entier reste = 0;
entier quotient = 0;

écrire("Entrez le dividende svp : ");
dividende = lire();
écrire("Entrez le diviseur svp : ");
diviseur = lire();

quotient = dividende / diviseur;
reste = dividende % diviseur;

écrireNL("Le quotient de la division de " + dividende.VersChaine() + " et de " + diviseur.VersChaine() + " est : " + quotient.VersChaine());
écrireNL("Le reste de la division de " + dividende.VersChaine() + " et de " + diviseur.VersChaine() + " est : " + reste.VersChaine());
```

</details>

## Exercice 6 – Algorithme mystère

Soit l’algorithme suivant :

``` csharp
entier nombreA = 5;
entier nombreB = 0;
entier resultat = 0;
nombreB = lire();
nombreB = nombreB + 1;
nombreA = nombreA + nombreB;
resultat = (nombreA * (nombreA + nombreB) % 5;

écrire(resultat);
```

Qu’est-ce que cet algorithme écrit si le nombre 2 est lu ?

## Exercice 7 – Moyenne

Écrivez un algorithme qui lit 3 réels au clavier et qui affiche à l'écran la moyenne.

<details>
    <summary>Proposition solution</summary>

``` csharp
réel valeur1 = 0.0;
réel valeur2 = 0.0;
réel valeur3 = 0.0;
réel moyenne = 0.0;

écrire("Veuillez saisir le premier nombre : ");
nombre1 = lire();

écrire("Veuillez saisir le deuxième nombre : ");
nombre2 = lire();

écrire("Veuillez saisir le troisième nombre : ");
nombre3 = lire();

moyenne = (valeur1 + valeur2 + valeur3) / 3.0;

écrireNL("La moyenne des trois valeurs est : " + moyenne.VersChaine());
```

</details>

## Exercice 8 – Algorithme mystère 2

Soit l’algorithme suivant :

```csharp
entier nombreX = 0;
entier nombreY = 10;
entier resultat = 0;
nombreX = lire();
resultat = nombreX / (nombreX - nombreY);

écrire(resultat);
````

Qu’arrive-t-il si le programme lit le nombre ```10``` au clavier ? Pourquoi ?

<details>
  <summary>Idée #1</summary>
  Quelle est la valeur de "nombreX" après la lecture ? 
</details>

<details>
  <summary>Idée #2</summary>
  Que se passe-t-il quand vous remplacer les variables par leurs valeurs dans l'expression "resultat = nombreX / (nombreX - nombreY);"
</details>

## Exercice 9 – Échanges

Écrivez un algorithme qui lit 2 réels dans les variables ```reel1``` et ```reel2```. Cet algorithme doit être capable d’échanger les valeurs contenues dans ```reel1``` et ```reel2```. À la fin de l’algorithme, affichez le résultat de ces deux variables.

<details>
  <summary>Idée #1</summary>
  Est-ce qu'une troisième variable pourrait vous servir ?  
</details>

<details>
    <summary>Proposition solution</summary>
    
```csharp
réel reel1 = 0.0;
réel reel2 = 0.0;
réel reelTemporaire = 0.0;

écrire("Entrez le premier réel : ");
reel1 = lire();

écrire("Entrez le second réel : ");
reel2 = lire();

écrireNL("reel1 vaut : " + reel1.VersChaine());
écrireNL("reel2 vaut : " + reel2.VersChaine());

reelTemporaire = reel1;
reel1 = reel2;
reel2 = reelTemporaire;

écrireNL("Après l'échange...");
écrireNL("reel1 vaut : " + reel1.VersChaine());
écrireNL("reel2 vaut : " + reel2.VersChaine());

```
</details>
