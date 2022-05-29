## První program

Vytvořme si ve Visual Studiu program s názvem `program.py` a do něj vložme
následující řádky

```python
kurz = 25
cena = 12 * kurz
print(cena)
```

Toto je jednoduchý program, který nám spočítá cenu lístku v korunách podle
kurzy 25 korun za euro. Takovýto program pak spustíme příkazem

```shell
$ python program.py
```

Pozor na znak dolaru na začátku tohoto příkazu. Tento znak nepíšeme! Znak
dolaru pouze naznačuje, že tento příkaz musíme zadat do terminálu operačního
systému, nikoliv do Python konzole. Pokud tedy váš příkazový řádek stále
začíná třemi zobáčky (`>>>`), jste ještě pořád uvnitř Python konzole a musíte z ní
vyskočit pomocí funkce `exit()`.
