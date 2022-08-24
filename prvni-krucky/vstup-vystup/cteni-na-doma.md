## Čtení na doma

Od verze 3.6 přibyl v Pythonu nový způsob, jak pracovat s řetězci, a to jsou **formátované řetězce**. 
Ty umožňují kombinovat vepsaný text s proměnnými bez nutnosti programování převodu vkládaných proměnných.

Formátovaný řetězec musíme od běžného řetězce odlišit písmenem `f`, které vkládáme před první uvozovku (nebo apostrof).
Tím Pythonu říkáme, že daný řetězec je formátovaný řetězce a je nutné věnovat pozornost
**složeným závorkám** uvnitř něj. 
Podle úvodního písmena f se těmto řetězcům někdy říká f-Strings. Následně můžeme
dovnitř uvozovek do složených závorek vkládat proměnné, a to i v případě, že jsou
jiného typu než řetězec. Proměnná je automaticky převedena na řetězec a až poté
vložena k ostatním částem řetězce.

Stejný výstup, jaký jsme si ukazovali již dvěma způsoby, je pak možné provést pomocí příkazu níže.

```python
print(f"Cena je {cena} Kč.")
```
