## Čtení na doma

Pozor na to, že zaokrouhlování v jazyce Python se chová trošku jinak než jak
jsem zvyklí ze školy. Zkuste například následující příkazy:

```py
zaokrouhlene_cislo = round(3.5)
print(zaokrouhlene_cislo)
zaokrouhlene_cislo = round(2.5)
print(zaokrouhlene_cislo)
```

Funkce `round()` totiž zaokrouhluje vždy k nejbližšímu sudému číslu, pokud se
vstup funkce nachází přesně uprostřed mezi dvěma hodnotami. Například 3.5 je
přesně mezi 3 a 4. Díky tomuto pravidlu tak Python namísto zaokrouhlování vždy
nahoru zaokrouhluje v polovině případů nahoru a v polovině dolů. Je to jakýsi
pokus být víc fér, protože tento způsob zaokrouhlování nezkreslí průměr hodnot.

## Cvičení na doma
::exc[excs>klasicke-zaokrouhlovani]

