# Exercices sur les bases

Ces exercices ont pour objectifs :

- l'évaluation d'expressions
- écriture d'algorithmes simples avec entrées / sorties et variables

## Exercices 1 - Opérations booléennes

Avec les données initiales :

- ```booléen x = vrai```
- ```booléen y = faux```
- ```booléen z = vrai```

Évaluez les expressions suivantes :

1. ```x et y```
2. ```y ou x```
3. ```x  ou z ou y```
4. ```y ou (x et z)```
5. ```y ou non x```
6. ```non x et y```
7. ```(non y et non x) ou x```

## Exercices 2 - Évaluations plus complexes

Avec les données initiales :

- ```entier x = 10```
- ```entier y = 5```
- ```entier z = 1```

Évaluez les expressions suivantes :

1. ```(X > Y) ou (Z > 1)```
2. ```(X/2 >= Y) et (Y == 5)```
3. ```non(X > 10) ou (Z > 1)```
4. ```(3*Z*Y == X+Y) et (X*5  == Y*10)```
5. ```non( (10*X-Y == 95) et (X-Y == Z*5) )```
6. ```(X % 3 == Y % 2) et (Z % 2 == 2)```
7. ```(X / 3 > 3) ou (Y / 3 > 1)```

## Exercices 3 - Salutations

Écrivez un algorithme qui lit le nom de l’utilisateur et qui lui affiche le texte "Bonjour " suivi du nom.

## Exercices 4 - Dé

Écrivez un algorithme qui affiche à l’utilisateur un nombre tiré au hasard compris entre 1 et 6.

## Exercices 5 - Divisions

Écrivez un algorithme qui lit deux nombres entiers et qui affiche le quotient et le reste de la division entière.

## Exercice 6 – Algorithme mystère

Soit l’algorithme suivant :

```csharp
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

## Exercice 8 – Algorithme mystère 2

Soit l’algorithme suivant :

```csharp
entier nombreX = 0;
entier nombreY = 10;
entier resultat = 0;
nombreX = lire();
resultat = nombreX / ( nombreX - nombreY);

écrire(resultat);
````

Qu’arrive-t-il si le programme lit le nombre ```10``` au clavier? Pourquoi?

## Exercice 9 – Échanges

Écrivez un algorithme qui lit 2 réels dans les variables ```reel1``` et ```reel2```. Cet algorithme doit être capable d’échanger les valeurs contenues dans ```reel1``` et ```reel2```. À la fin de l’algorithme, affichez le résultat de ces deux variables.

<script>
  var url = encodeURIComponent(window.location.origin);
  url = "https://try.dot.net/?fromGist=df44833326fcc575e8169fccb9d41fc7&hostOrigin=" + url;
  document.getElementById("myIFrame").contentWindow.document.location.href=url;
</script>

<iframe id="myIFrame" src="about:blank" width="1000" height="450" >
</iframe>
