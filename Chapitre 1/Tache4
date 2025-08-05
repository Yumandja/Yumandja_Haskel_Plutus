TACHE4

✅ Tâche 4 – Composer une fonction pour traiter des données de joueurs
🔢 Code Haskell :
# ✅ Tâche 4 – Composer une fonction pour traiter des données de joueurs


## 🔢 Code Haskell :
```haskell
import Data.List (sortBy)

-- Trie la liste des joueurs par score décroissant
sortByScore :: [(String, Int)] -> [(String, Int)]
sortByScore = reverse . sortBy (\(_, s1) (_, s2) -> compare s1 s2)

-- Extrait les noms des joueurs (la 1ère valeur de chaque tuple)
extractPlayers :: [(String, Int)] -> [String]
extractPlayers = map fst

-- Prend les 3 premiers éléments d'une liste
topThree :: [a] -> [a]
topThree = take 3

-- Compose les fonctions : trie → extrait les noms → garde les 3 premiers
getTopThreePlayers :: [(String, Int)] -> [String]
getTopThreePlayers = topThree . extractPlayers . sortByScore

-- Fonction principale pour tester
main :: IO ()
main = do
    let joueurs = [("Alice", 42), ("Bob", 55), ("Charlie", 28), ("Diana", 70), ("Eve", 61)]
    let topJoueurs = getTopThreePlayers joueurs
    putStrLn "Top 3 des joueurs :"
    mapM_ putStrLn topJoueurs
```



📚 Explications :
sortByScore trie la liste des tuples (nom, score) selon le score décroissant.

compare s1 s2 → trie croissant.

reverse → on inverse pour avoir décroissant.

extractPlayers applique map fst pour extraire les noms des tuples.

topThree garde les 3 premiers éléments avec take 3.

getTopThreePlayers compose tout ça : trie → extrait les noms → prend les 3 premiers.

main crée une liste de joueurs, applique getTopThreePlayers, puis les affiche.





