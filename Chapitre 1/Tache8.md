TACHE 8

✅ Tâche 8 – Créer une fonction applyTwice
🧩 Objectif :
Créer une fonction d’ordre supérieur qui prend une fonction et une valeur, et applique cette fonction deux fois à la valeur.

```
-- Déclare applyTwice : prend une fonction (a -> a) et une valeur a, renvoie a
applyTwice :: (a -> a) -> a -> a
applyTwice f x = f (f x)

-- Fonction principale pour tester
main :: IO ()
main = do
    print (applyTwice (+1) 3)      -- 5
    print (applyTwice (*2) 4)      -- 16
    print (applyTwice reverse "abc")  -- "abc"

```
📚 Explications :
applyTwice prend en paramètre :

une fonction f qui transforme un type a en lui-même (a -> a)

une valeur x de type a

Elle applique f deux fois : f (f x)

Quelques exemples :

applyTwice (+1) 3 → (+1) ((+1) 3) → 4 → 5

applyTwice (*2) 4 → (*2) ((*2) 4) → 8 → 16

applyTwice reverse "abc" → "cba" → "abc"


