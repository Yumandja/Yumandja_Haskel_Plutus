HC1T1 - Tâche 1 : Composition de fonctions

🔧 Objectif :
Créer une fonction qui double un nombre , puis ajoute 1 , en utilisant la composition de fonctions .

✅ Code Haskell minimal avec explication :
Haskell

Copie

Modifier
-- Double un nombre
double x = x * 2

-- Incrémente un nombre
increment x = x + 1

-- Applique double, puis increment (composition de fonctions)
doubleThenIncrement = increment . double

-- Affiche le résultat pour le nombre 3
main = print (doubleThenIncrement 3)
🔍 Explication :
double x = x * 2→ Multiplier xpar 2.

increment x = x + 1→ Ajout 1 à x.

doubleThenIncrement = increment . double→ Fait double puis increment .

main→ Afficher le résultat de doubleThenIncrement 3.
