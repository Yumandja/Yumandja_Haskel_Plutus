TACHE 6

✅ Tâche 6 – Fonction avec signature de type : addNumbers
🧩 Objectif :
Créer une fonction addNumbers qui prend deux entiers et retourne leur somme, avec une signature de type explicite.

```
-- Déclare la fonction avec son type : deux Int → un Int
addNumbers :: Int -> Int -> Int
addNumbers x y = x + y

-- Fonction principale pour tester
main :: IO ()
main = do
    let a = 7
    let b = 5
    let resultat = addNumbers a b
    putStrLn ("La somme de " ++ show a ++ " et " ++ show b ++ " est " ++ show resultat)

```
📚 Explications :
addNumbers :: Int -> Int -> Int signifie :

prend un Int x,

puis un autre Int y,

et retourne un Int (la somme x + y).

x + y fait simplement l'addition.

main teste la fonction avec 7 et 5, et affiche le résultat.

✅ Résultat attendu :
nginx
Copy
Edit
La somme de 7 et 5 est 12


