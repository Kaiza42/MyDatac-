# ici seras noté des therme "utilitaire" 


### range 

Pour suprimer par exemple La premiere lettre d'une string Ou la derniere lettre d'une string 

```cs

string Bonjour = "hello"
Console.WriteLine(Bonjour[1..^1]);
// dans cette exemple on surpime la premiere et la derniere lettre 
// sa peu etre utiliser dans des array et des string 

```
### parse 

dans l'idée je souhaite convertir une string en nombre 

```cs 

string mesChiffre = "125896";

int mesVraiChiffre = int.Parse(MesChiffre);
// sa peu marcher avec float double decimal 
```

### TryParse

Dans l'idée  c'est la meme choses que parse mais cette fois tu a un retour si la conversion est reussi ou non 
l'enxemple utiliser a était fait dans un exo 
```cs
int conversionSaisie;
int trouveMoi = 0;
int result = 0;

do
{
  // la saisie utilisateur Qui doit etre dans la boucle Pour continuer la saisie utilisateur 
    string saisie = Console.ReadLine();

// Tryparse permet la conversion de la saisie de  String a Int et out peut renvoyer true ou false et fait le resultat demander.
    if (int.TryParse(saisie, out conversionSaisie))
    {
      // si conversionSaisie est différent de trouveMoi Alors affiche la Console 
        if (conversionSaisie != trouveMoi)
        {
            Console.WriteLine("hey c'est pas compliquer .. un chiffre entre 0 et 9 ");

        }
        else
        {
          // Sinon bah bravo.
            Console.WriteLine("Bravo.");

        }
        // le resultat de toute les saisie utilisateur 
        result += conversionSaisie;
        Console.WriteLine("le resultat de toute tes saisie donne sa " + result);

    }
    la condition pour continuer la boucle 
} while (conversionSaisie != trouveMoi);


```
### Split 

transformer ta string en array 

```cs
string hello = "hello jpp c'est simple a comprendre";

Console.WriteLine(hello.Split(' '));

```

### Replace 

permet de remplacer un élément par un autre 

```cs
string hello = "hello";

Console.Write(hello.Replace("h", "p"));
// dans les parenthese de replace le "h" et remplacer par "p" ce qui donne "pello"
```

### string.Empty 

```cs

string vide = string.Empty;
// permet que la chainne sois vide donc le contenue est "" 

```

### ToUpper & ToLower

```cs
string name = "NAME";

//ToLower pour passer tout le texte en minuscule 
Console.WriteLine(name.ToLower());

string Name = "name";
//ToUpper pur passer tout le texte en majuscule
Console.WriteLine(Name.ToUpper());
```

### IndexOf

IndexOf va chercher le premier élément demander 
```cs
string texte = "Bonjour tout le monde";
int index = texte.IndexOf("t"); // 8 car le premier T est a la place 8
Console.WriteLine(index);

// on peut comencer l'index of apartir d'un endroit precis 
string texte = "Bonjour tout le monde";
int index = texte.IndexOf('o', 5); ici 
Console.WriteLine(index);
```


### Sort

dans cette exemple ``Sort();`` va changer l'ordre de la liste pour mettre un ordre alphabetique 
```cs
var names = new List<string> {"yes","no","myabe", "idon't know"  };
names.Sort();
foreach (var name in names)
{
  Console.WriteLine($"Hello {name}!");
}
```

### contains 
verifie si une chaine de caractère contient l'élément demander 

```cs
// je declare ma chaine de caractère 
string fruit = "amande";

ma variable verifications va vérifier grace a Contains si "a" est dans la chaine de caractère de la variable "fruit"
bool verifications = fruit.Contains("a");

Console.WriteLine(verifications);
```

### ToString
En sois ToString change une variable double pour l'exemple en chaine de caractère 

```cs
double n = 25.25; 

Console.WriteLine(n.ToString(""));
sa afficheras 25.25
//maintenant imaginons que nous ne souhaitons pas afficher la décimal
double n = 25.25; 

Console.WriteLine(n.ToString("0"));
// maintenant uniquement le premier chiffre de la virgule 
double n = 25.25; 

Console.WriteLine(n.ToString("0.0"));
// Sa afficheras 25.3 sa arrondis au supérieur 
//évidament on peut faire sa pour afficher autant de nombre en decimal qu'on veut 
double n = 25.25; 

Console.WriteLine(n.ToString("0.00"));
//sa afficheras 25.25
// ect
```

###






