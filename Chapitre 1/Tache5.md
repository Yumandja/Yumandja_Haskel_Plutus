TACHE 5

✅ Tâche 5 – Générer une liste infinie de nombres (paresse en Haskell)
🧩 Objectif :
Créer une fonction infiniteNumbers qui génère une liste infinie de nombres (par exemple : 1, 2, 3, 4…).

Puis, extraire seulement les n premiers éléments de cette liste (paresse / "laziness").

```
-- Génère une liste infinie de nombres entiers à partir de 1
infiniteNumbers :: [Int]
infiniteNumbers = [1..]

-- Fonction principale pour tester
main :: IO ()
main = do
    let n = 10
    let premiers = take n infiniteNumbers
    putStrLn ("Les " ++ show n ++ " premiers nombres :")
    print premiers

```
📚 Explications :
[1..] crée une liste infinie paresseuse de tous les entiers à partir de 1.

En Haskell, grâce à la paresse (lazy evaluation), cette liste n’est pas calculée tant qu’on ne la demande pas.

take n infiniteNumbers extrait seulement les n premiers éléments de cette liste infinie, donc pas de crash ou de boucle infinie.

Dans main, on affiche les 10 premiers nombres de la liste.

✅ Résultat attendu :
csharp
Copy
Edit
Les 10 premiers nombres :
[1,2,3,4,5,6,7,8,9,10]
