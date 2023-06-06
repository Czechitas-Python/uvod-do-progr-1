## Čtení z terminálu

Uvažujme, že vytváříme program pro směnárnu, který by měl umět převést libovolnou částku dle přání zákazníka. Náš program by se tedy měl na začátku zeptat uživatele, jaká částka má být převedena. K tomu slouží funkce `input()`. Jako vstup zadáme zprávu, která se má zobrazit uživateli, aby věděl, jakou informaci program očekává.

Důležité je, že funkce `input()` vždy vrací hodnotu vloženou uživatelem jako typ **řetězec**, a to i v případě, že uživatel zadal pouze čísla. Na číslo musíme hodnotu **převést**. K tomu využijeme funkci `int()`, která nemění hodnotu vstupu, ale **mění typ hodnoty**, v tomto případě převádí řetězec na celé číslo.

```python
kurz = 25
euro = input("Zadej počet euro: ")
euro = int(euro)
cena = euro * kurz
```

### Složitější výpis

Tento program sice výsledek spočítá, ale nevypíše. K vypsání můžeme použít funkci `print()`, kterou již známe. Ve výpisu potřebujeme zkombinovat vysvětlující text a peněžní částku. Jednotlivé informace oddělíme čárkami. Funkce `print()` je spojí dohromady do jednoho textu a oddělí mezerami, ty tedy nemusíme do výpisu přidávat.

```python
print("Cena je", cena, "Kč.")
```

Pokud by nám toto chování nevyhovovalo a chceme si o mezerách rozhodnout sami, můžeme použít vstup `sep` (od anglického slova :term{cs="oddělovač" en="separator"}). Ten musíme napsat i **se jménem** a vždy až **na konec**, aby funkce věděla, že se nejedná o další text k vypsání. Nyní již musíme mezery přidat do řetězců v uvozovkách, aby se ve výpisu objevily.

Vstup `sep` je agumentem funkce, který zapisujeme spolu se jménem. Mezi jméno argumentu a jeho hodnotu vkládáme `=`. Bez toho by Python nedokázal odlišit, co je oddělovač a co je jen další řetězc k vypsání na obrazovku.

```python
print("Cena je ", cena, " Kč.", sep="")
```

### Převod na řetězec

Další možností, jak výpis provést, je použití operátorů `+` pro spojení více řetězců dohromady.
Musíme ale myslet na to, že proměnná `cena` je typ číslo. Nyní tedy musíme provést 
obrácenou operaci, než jsou dělá funkce `int()`, a to je **převod čísla na řetězec**. 
K převodu slouží funkce `str()`. Jakmile máme všechny hodnoty převedené na řetězec, můžeme
je spojit dohromady pomocí `+`.

```python
cena = str(cena)
print("Cena je " + cena + " Kč.")
```

Oba řádky je možné spojit do jednoho a provést převod na řetězec uvnitř funkce `print()`.
Pokud ti ale tento zápis připadá příliš složitý, není vůbec problém nechat jej 
rozdělený na dva řádky.

```python
print("Cena je " + str(cena) + " Kč.")
```
