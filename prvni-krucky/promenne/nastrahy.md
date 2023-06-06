## Nástrahy

Do proměnné se jako do šuplíku ukládá pouze hodnota a nikoliv celý výpočet. Pokud tedy napíšeme například

```py
sazba = 450
cena_zakazky = 8 * sazba
print(cena_zakazky)
```

bude v proměnné `cena_zakazky` uložena hodnota 3600. Jestliže poté změníme sazbu (například započteme slevu 50 korun pro stálého zákazníka), musíme výpočet ceny zakázky přesunout až na poslední řádek. Python totiž provádí příkazy řádek po řádku a vždy pracuje s hodnotou, která je v proměnné aktuálně uložená.

```py
sazba = 450
sazba = sazba - 50
cena_zakazky = 8 * sazba
print(cena_zakazky)
```
