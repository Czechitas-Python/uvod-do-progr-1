S čísly a řetězci jsme zatím byli schopní pracovat pouze pomocí aritmetických
operátorů. To nám ale brzy nebude stačit a budeme potřebovat složitější
operace, kterým říkáme *funkce*.

## Funkce

Funkce je nějaký komplikovanější výpočet nebo malý program zabalený do jakési
krabičky. Této krabičce dáme nějaké jméno, abychom jej mohli používat na
různých místech v našem programu. Funkci si můžeme představit jako topinkovač.
Topinkovač pro nás dělá nějakou užitečnou činnost (opéká topinky), která by
byla otravná a zdlouhavá, kdybychom ji chtěli dělat sami, například smažit
topinky na oleji na pánvičce. Každá funkce má svoje jméno a obvykle má nějaký
vstup (čerstvý chleba) a výstup (opečená topinka). Funkci spustíme tak, že ji
takzvaně **zavoláme**.

Dobrým příkladem v jazyce Python je funkce `round()`, která pro nás dělá
zaokrouhlování. Můžeme tedy psát

```pycon
>>> round(3.141592)
3
```

Tomuto zápisu se říká *volání funkce*. Funkce se vždy volá tak, že napíšeme
její jméno a do kulatých závorek za něj její vstupy (odborně se vstupům říká
*argumenty*). V našem případě funkci předáváme jeden argument (vstup), číslo
3.141592. Když funkci zavoláme s nějakým argumentem, funkce takzvaně *vrátí*
výsledek.

Kromě funkce `round()` Python obsahuje mnoho dalších užitečných funkcí a mnoho
z nich uvidíme v pozdějších částech tohoto kurzu. Nyní můžeme kromě funkce
`round()` zmínit například funkci `len()`, která vrací počet znaků uvnitř
nějakého řetězce. Například:

```pycon
>>> jmeno = 'Theodor Holohlávek'
>>> len(jmeno)
18
```
