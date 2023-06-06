## Moduly

Python sice obsahuje mnoho užitečných funkcí, ale vzhledem k množství problémů, které chceme pomocí Pythonu řešit, je to pořád málo a různých funkcí potřebujeme opravdu hodně. Abychom se v tom všem vyznali, třídíme funkce do takzvaných modulů.

Jeden z užitečných modulů nese název `math`, a obsahuje mnoho standardních matematických funkcí. Mimo jiné obsahuje funkce pro zaokrouhlování nahoru a dolů. Pokud chceme modul `math` použít, musíme jej nejdříve importovat příkazem

```py
import math
```

Příkazy `import` pro přehlednost zapisujeme na začátek programu. Poté, co tento příkaz zadáme Pythonu, můžeme volat všechny funkce z tohoto modulu tak, že vždy před název funkce pomocí tečky připojíme název modulu, ze kterého funkce pochází. Například

```py
zaokrouhlene_cislo = math.ceil(3.14)
print(zaokrouhlene_cislo)
```

Dalším užitečným modulem je modul `random`, který obsahuje funkce pro generování náhodných čísel. Jedna z takových funkcí se jmenuje `randint()`. Umí generovat náhodná celá čísla v zadaném rozmezí. Můžeme tak například simulovat házení kostkou.

```py
import random
nahodne_cislo = random.randint(1, 6)
print(nahodne_cislo)
nahodne_cislo = random.randint(1, 6)
print(nahodne_cislo)
```
