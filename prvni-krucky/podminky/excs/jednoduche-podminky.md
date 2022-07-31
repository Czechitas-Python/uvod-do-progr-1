---
title: Jednoduché podmínky
demand: 2
---

1. Založte si program `prihlaseni.py`. V tomto nechte uživatele zadat svoje uživatelské jméno a poté heslo. Pokud se heslo shoduje s heslem **simsalabim** vypište na výstup

```
Správné heslo
```

Program spusťte na konzoli a vyzkoušejte, že dělá co má.

2. Upravte tento program tak, aby vypsal

```
Vstup nepovolen
```

pokud uživatel zadá špatné heslo.

3. K vypsání textu `Vstup nepovolen` nyní použijte funkci `exit()` namísto funkce `print()`. Funkci `exit()` můžete použít stejně jako funkci `print()`, tj. text k výpisu zadejte do závorek jako vstup. Funkce `exit()` ale spolu s výpisem zprávy program ukončí a zajistí, že uživatel bez správného hesla nebude moci v aplikaci provádět žádné další akce. 

4. Na konec programu vložte příkaz, který se uživatele zeptá na jeho věk. Pokud je uživateli 18 let či více, vypiš mu zprávu

```
Smíš vstoupit
```

Pokud je mladší, vypiš zprávu

```
Vstup je možný až od 18 let
```
