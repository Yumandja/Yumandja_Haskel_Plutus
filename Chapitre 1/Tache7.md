TACHE 7

✅ Tâche 7 – Conversion Fahrenheit en Celsius
🧩 Objectif :
Créer une fonction fToC qui convertit une température en Fahrenheit vers Celsius à l'aide de la formule suivante :

𝐶 = ((𝐹-32) × 5)/ 9

```
-- Déclare la fonction : prend un Float et retourne un Float
fToC :: Float -> Float
fToC f = (f - 32) * 5 / 9

-- Fonction principale pour tester
main :: IO ()
main = do
    let tempF = 77
    let tempC = fToC tempF
    putStrLn ("La température de " ++ show tempF ++ "°F est équivalente à " ++ show tempC ++ "°C")

```

📚 Explications :
fToC :: Float -> Float : prend une température en degré Fahrenheit et retourne le résultat en degré Celsius.

La formule :

f - 32 → on ajuste l’écart de base.

* 5 / 9 → on transforme l’unité en Celsius.

main convertit 77°F, ce qui correspond à environ 25°C.
 




