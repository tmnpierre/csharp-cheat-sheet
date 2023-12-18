# C# Cheat Sheet

## Sommaire

- [C# Cheat Sheet](#c-cheat-sheet)
  - [Sommaire](#sommaire)
  - [Syntaxe de Base](#syntaxe-de-base)
  - [Types de Données](#types-de-données)
  - [Opérateurs](#opérateurs)
  - [Structures de Contrôle](#structures-de-contrôle)
  - [Collections](#collections)
  - [Classes et Objets](#classes-et-objets)
  - [Héritage](#héritage)
  - [Interfaces](#interfaces)
  - [Gestion des Exceptions](#gestion-des-exceptions)
  - [Lambdas et LINQ](#lambdas-et-linq)
  - [Travailler avec des Fichiers](#travailler-avec-des-fichiers)

## Syntaxe de Base

```csharp
// Commentaire en ligne
/* Commentaire
   sur plusieurs lignes */

// Déclaration de variable
int a = 5;

// Constantes
const double PI = 3.14;

// Affichage en console
Console.WriteLine("Hello, world!");
```

## Types de Données

```csharp
int    // Entier 32 bits
long   // Entier 64 bits
float  // Flottant 32 bits
double // Flottant 64 bits
bool   // Booléen (true/false)
char   // Caractère unique
string // Chaîne de caractères
```

## Opérateurs

```csharp
// Opérateurs arithmétiques : +, -, *, /, %
// Opérateurs de comparaison : ==, !=, <, >, <=, >=
// Opérateurs logiques : &&, ||, !
```

## Structures de Contrôle

```csharp
// Condition if
if (condition) {
    // code
} else if (autreCondition) {
    // autre code
} else {
    // autre code
}

// Boucle while
while (condition) {
    // code
}

// Boucle for
for (int i = 0; i < 10; i++) {
    // code
}

// Boucle foreach
foreach (var item in collection) {
    // code
}

// Switch
switch (variable) {
    case valeur1:
        // code
        break;
    case valeur2:
        // code
        break;
    default:
        // code
        break;
}
```

## Collections

```csharp
// Tableaux
int[] monTableau = new int[5];

// Listes
List<int> maListe = new List<int>();

// Dictionnaires
Dictionary<string, int> monDictionnaire = new Dictionary<string, int>();
```

## Classes et Objets

```csharp
public class MaClasse {
    // Propriétés
    public int MaPropriete { get; set; }

    // Constructeur
    public MaClasse() {
        // Initialisation
    }

    // Méthodes
    public void MaMethode() {
        // Code
    }
}
```

## Héritage

```csharp
public class ClasseBase {
    // Code de la classe de base
}

public class ClasseDerivee : ClasseBase {
    // Code de la classe dérivée
}
```

## Interfaces

```csharp
public interface MonInterface {
    void MaMethode();
}
```

## Gestion des Exceptions

```csharp
try {
    // Code pouvant générer une exception
} catch (TypeException e) {
    // Gestion de l'exception
} finally {
    // Code exécuté après le bloc try/catch
}
```

## Lambdas et LINQ

```csharp
// Expression lambda
Func<int, int> doubler = x => x * 2;

// Requête LINQ
var resultats = from element in collection
                where element.Condition
                select element;
```

## Travailler avec des Fichiers

```csharp
// Lire un fichier
string contenu = File.ReadAllText(cheminFichier);

// Écrire dans un fichier
File.WriteAllText(cheminFichier, contenu);
```
