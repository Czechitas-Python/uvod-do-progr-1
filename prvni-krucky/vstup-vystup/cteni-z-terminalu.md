## Čtení z terminálu

Uvažujme, že vytváříme program pro směnárnu, který by měl umět převést libovolnou částku dle přání zákazníka. Náš program by se tedy měl na začátku zeptat uživatele, jaká částka má být převedena. K tomu slouží funkce `input()`. Jako vstup zadáme zprávu, která se má zobrazit uživateli, aby věděl, jakou informaci program očekává.

Důležité je, že funkce `input()` vždy vrací hodnotu vloženou uživatelem jako typ **řetězec**, a to i v případě, že uživatel zadal pouze čísla. Na číslo musíme hodnotu **převést**. K tomu využijeme funkci `int()`, která nemění hodnotu vstupu, ale **mění typ hodnoty**, v tomto případě převádí řetězec na celé číslo.

```python
kurz = 25
euro = input("Zadej počet euro: ")
euro = int(euro)
cena = euro * kurz
```

### Formátovaný výpis

Předchozí program sice výsledek spočítá, ale nevypíše. K vypsání můžeme použít funkci `print()`, kterou již známe. Ve výpisu potřebujeme zkombinovat vysvětlující text a peněžní částku.

Od verze 3.6 přibyl v Pythonu nový způsob, jak pracovat s řetězci, a to jsou :term{cs="formátované řetězce" en="f-strings"}. Ty umožňují kombinovat vepsaný text s proměnnými bez nutnosti přetypovávání vkládaných proměnných.

Formátovaný řetězec musíme od běžného řetězce odlišit písmenem `f`, které
vkládáme před první uvozovku (nebo apostrof). Tím Pythonu říkáme, že daný
řetězec je formátovaný řetězce a je nutné věnovat pozornost **složeným
závorkám** uvnitř něj. Následně můžeme dovnitř uvozovek do složených závorek
vkládat proměnné (obecně kusy Python kódu), a to i v případě, že jsou jiného
typu než řetězec. Proměnná je automaticky převedena na řetězec a až poté
vložena k ostatním částem řetězce.

```python
print(f"Cena je {cena} Kč.")
```
