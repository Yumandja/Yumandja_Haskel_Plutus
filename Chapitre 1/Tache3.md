# ✅ Tâche 3 – Vérifier si un nombre est supérieur à 18

## 🧩 Objectif :
Créer une fonction `greaterThan18` qui vérifie si un nombre entier est strictement supérieur à 18.

---

## 🔢 Code Haskell :
```haskell
-- Déclaration de la fonction avec son type :
-- Elle prend un entier et retourne un booléen (True ou False)
greaterThan18 :: Int -> Bool
greaterThan18 nombre = nombre > 18

-- Fonction principale pour tester
main :: IO ()
main = do
    let n = 20
    let resultat = greaterThan18 n
    putStrLn ("Le nombre " ++ show n ++ " est-il supérieur à 18 ? " ++ show resultat)
```

---

## 📚 Explications :

- `greaterThan18` prend un entier (`Int`) et retourne un booléen (`Bool`) : `True` si le nombre est strictement supérieur à 18, `False` sinon.
- `nombre > 18` : comparaison simple.
- Dans `main`, on teste avec `n = 20`, ce qui doit afficher `True`.

---

## ✅ Résultat attendu :
```
Le nombre 20 est-il supérieur à 18 ? True
```

---


