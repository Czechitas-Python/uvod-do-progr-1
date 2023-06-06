Zatím jsme vše, co naše programy dělaly, museli naprogramovat sami. Nyní si ukážeme používání funkcí, což nám umožňuje využívat kód, který už napsal někdo před námi. Tím ušetříme spoustu času a budeme se moci věnovat věcem, které jsou unikátní pro náš program.

Jednu funkci už známe, a tou je `print()`. Nyní si ukážeme nějaké další a řekneme si více o tom, jaké možnosti funkce nabízejí.

## Funkce

Funkce je nějaký komplikovanější výpočet nebo malý program zabalený do jakési krabičky. Této krabičce dáme nějaké jméno, abychom jej mohli používat na různých místech v našem programu. Funkci si můžeme představit jako topinkovač. Topinkovač pro nás dělá nějakou užitečnou činnost (opéká topinky), která by byla otravná a zdlouhavá, kdybychom ji chtěli dělat sami, například smažit topinky na oleji na pánvičce. Každá funkce má svoje jméno a obvykle má nějaký vstup (čerstvý chleba) a výstup (opečená topinka). Funkci spustíme tak, že ji takzvaně **zavoláme**.

Dobrým příkladem v jazyce Python je funkce `round()`, která pro nás dělá zaokrouhlování. Můžeme tedy psát

```py
zaokrouhlene_cislo = round(3.141592)
print(zaokrouhlene_cislo)
```

Tomuto zápisu se říká *volání funkce*. Funkce se vždy volá tak, že napíšeme její jméno a do kulatých závorek za něj její vstupy (odborně se vstupům říká *argumenty*). V našem případě funkci předáváme jeden argument (vstup), a to číslo 3.141592. Když funkci zavoláme s nějakým argumentem, funkce takzvaně *vrátí* výsledek. Výsledek můžeme uložit do proměnné pomocí znaku `=`. Při volání funkce můžeme používat i proměnné.

```py
cislo = 3.141592
zaokrouhlene_cislo = round(cislo)
print(zaokrouhlene_cislo)
```

Kromě funkce `round()` Python obsahuje mnoho dalších užitečných funkcí a mnoho z nich uvidíme v pozdějších částech tohoto kurzu. Nyní můžeme kromě funkce `round()` zmínit například funkci `len()`, která vrací počet znaků uvnitř nějakého řetězce. Například:

```py
jmeno = 'Theodor Holohlávek'
delka_jmena = len(jmeno)
print(delka_jmena)
```
