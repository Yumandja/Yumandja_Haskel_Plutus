TACHE 2

🟩 Tâche 2 : Fonction pure circleArea
🎯 Objectif :
Créer une fonction pure qui calcule l'aire d’un cercle à partir du rayon.

✅ Rappel : Qu’est-ce qu’une fonction pure ?
Une fonction est pure si :

Elle dépend uniquement de ses arguments (pas de variables externes).

Elle ne modifie rien à l’extérieur (pas d’effets de bord).

Pour un même argument, elle renvoie toujours le même résultat.

📐 Formule de l’aire d’un cercle :
Aire=π×r2
 
Où r est le rayon.



-- Déclaration de la fonction avec son type :
-- Elle prend un Float et retourne un Float (l'aire du cercle)
circleArea :: Float -> Float
circleArea rayon = pi * rayon * rayon

-- Fonction principale pour tester la fonction circleArea
main :: IO ()
main = do
    let rayon = 5
    let aire = circleArea rayon
    putStrLn ("L'aire du cercle de rayon " ++ show rayon ++ " est " ++ show aire)


     Explication :
circleArea est le nom de la fonction.

Float -> Float signifie : la fonction prend un Float (le rayon) et retourne un Float (l’aire).

pi est une constante prédéfinie dans Haskell (≈ 3.14159).

rayon * rayon c’est le carré du rayon.

📚 Explication rapide de main :
let rayon = 5 → on choisit un rayon de 5.

let aire = circleArea rayon → on calcule l’aire avec la fonction pure.

putStrLn → affiche une phrase à l’écran.

show → transforme un nombre en texte pour pouvoir l'afficher.

