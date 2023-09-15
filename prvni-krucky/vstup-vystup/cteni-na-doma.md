## Čtení na doma

Pokud bychom z jakéhokoliv důvodu nechtěli použít f-stringy, můžeme jednotlivé informace oddělit čárkami. Funkce `print()` je spojí dohromady do jednoho textu a oddělí mezerami, ty tedy nemusíme do výpisu přidávat.

```python
print("Cena je", cena, "Kč.")
```

### Volitelné parametry funkce `print()`

Pokud by nám toto chování nevyhovovalo a chceme si o mezerách rozhodnout sami, můžeme použít vstup `sep` (od anglického slova :term{cs="oddělovač" en="separator"}). Ten musíme napsat i **se jménem** a vždy až **na konec**, aby funkce věděla, že se nejedná o další text k vypsání. Nyní již musíme mezery přidat do řetězců v uvozovkách, aby se ve výpisu objevily.

Vstup `sep` je argumentem funkce, který zapisujeme spolu se jménem. Mezi jméno argumentu a jeho hodnotu vkládáme `=`. Bez toho by Python nedokázal odlišit, co je oddělovač a co je jen další řetězec k vypsání na obrazovku.

```python
print("Cena je ", cena, " Kč.", sep="")
```

Dalším užitečným volitelným argumentem funkce `print()` je `end`, kterým se nastavuje, jak se má výpis funkcí `print()` ukončit. Ve výchozím nastavení je to znak nového řádku `end='\n'`, ale toto chování můžeme upravit, aby nám například šlo vypsat více volání funkce `print()` na jeden řádek.

```python
print("hurá", end="! ")
print("hurá", end="! ")
print("hurá", end="! ")
print()
```

Tento program vypíše vše na jeden řádek. Prázdný `print()` vypíše své výchozí ukončení, tj. nový řádek.

```shell
hurá! hurá! hurá!
```

### Převod na řetězec

Poslední možností, jak výpis provést, je použití operátorů `+` pro spojení více řetězců dohromady.
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
