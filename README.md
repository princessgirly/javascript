# JAVASCRIPT
Cours sur javascript

Grammaire
=
Des éléments de la grammaire française traduits en JS :

+ ponctuation <pre><code>, ; ( ) { }</pre></code>

+ logique et conjonctions de subordination ~ contrôle <pre><code>if else switch while for</pre></code>

+ nom : données/valeurs <pre><code>1 "un" [1] { prop: 1} function() {}</pre></code>

+ pronom (prend la place d'un nom) <pre><code>var</pre></code>

+ il y a des mots "invariables" <pre><code>true false</pre></code>

+ verbes : opérateurs, fonctions et méthodes  

Champ lexical
=
Si on admet l'analogie "nom en français" <=> "données en JS", on peut comparer le champ lexical au type de données :

données de type primitif :
+ booléens <code>true false</code> (espace de valeurs invariable)
+ nombres 1 1.1 1e4
+ chaînes de caractères <code>"aujourd'hui" ou 'aujourd\'hui'</code>
+ symbols
+ valeur <code>nulle null</code>
+ valeur <code>non définie undefined</code>
+ les objets
+ objet générique <code>{ propriété: "valeur", autre: 2 }</code>
+ tableaux [1, 2, 3]
+ plus tous les types qu'on veut créer, ceux d'ES6 (Map, Set)...
+ les fonctions (et oui un verbe peut servir de nom "tricher n'est pas jouer")
+ TODO portée des variables

Les verbes en actions
=
// operator

var result = x + y;

// invocation de fonction

result = add(x, y);

// invocation de méthode

result = x.add(y);

Quelques opérateurs . typeof = + - ! * / % > < <= >= !== === && || ? : ++ -- new += return ? :

Orthographe JS
=
+ un nom de variable est une lettre optionnellement suivie par une ou plusieurs lettres, chiffres et _
+ il existe des mots réservés par le langage, et donc interdits dans le noms de variables <code>if function else var...</code>
+ les valeurs littérales :
 - pour un nombre <code>10 2.5 3.1e2</code>
 - une chaîne de caractère
- un tableau <code>(array) [1, 2, 3]</code>
 - un objet
 - une fonction <code>function myFunction(arguments) { "body"; }</code>
 - une expression régulière <code>/ab+c/</code>

Conjugaison JS
=
Les différentes manières d'enclencher les actions/verbes (invocation, apply, call)

Vocabulaire JS
=
Mots du langage, et API, à savoir objets et fonctions déjà présents, par exemple :

* Indentation : décaler certaines parties du code de manière à le rendre plus lisible.
* parseInt : convertir en un nombre entier
* parseFloat : convertir en un nombre décimal
* isNaN : Not a number ce n'est pas un nombre
* true
* window dans un navigateur
* console
* JSON.parse()

Quelques exemples vous montrant la souplesse de ces fonctions :

* parseInt("12.9 Euros") vaudra 12 (on convertit en entiers, les chiffres après la virgule sont ignorés)
* parseInt(" 12 Frs ") vaudra également 12 (l'espace en début de chaîne est ignoré)
* parseInt("J'ai 12 Euros") vaudra Nan (la chaîne commence par une lettre)
* parseFloat(" 12.9 Frs ") vaudra 12.9
* parseFloat("3,14") vaudra... 3 : il faut utiliser le point et non la virgule. La conversion va donc s'arrêter après le "3".

Priorités de calcul
-
1. de gauche à droite
2. multiplications (*), division (/) et modulo (%)
3. addition (+) et soustraction (-).

Autres opérateurs
-
resultat += X;   
resultat = resultat + X;
***
Ces deux lignes sont strictement équivalentes, idem pour :
***
resultat -= X;   
resultat = resultat - X;

resultat *= X;   
resultat = resultat * X;

resultat %= X;   
resultat = resultat % X;

variable += X;
variable = variable + X;

variable -= X;
variable = variable - X;

Incrémentation / décrémentation
-
Pour augmenter de 1 la valeur d'une variable (= incrémenter) **variable++**

Pour diminuer de 1 la valeur d'une variable (= décrémenter) **variable--**

variable++; 
variable += 1; 
variable = variable + 1;


variable--; 
variable -= 1; 
variable = variable - 1;

Exemples de fonction :
-
triple(x) qui renvoie le triple de l'argument : **function triple(x) { return 3*x; }**

carre(x) qui renvoie le carré de l'argument (x²) :  **function carre(x) { return x*x; }**

cube(x) qui renvoie le cube de l'argument: **function cube(x) { return x*x*x; }**






