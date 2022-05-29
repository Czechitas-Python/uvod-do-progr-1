Počítače a programování byly vymyšleny především proto, aby ušetřili lidem
nudnou a repetitivní práci. Proto chceme umět počítači říct, že má nějakou
činnost **opakovat mnohokrát po sobě**. K tomu nám v programování slouží takzvané
cykly.

## Cyklus FOR

Jeden z nejpoužívanějších cyklů v téměř všech programovacích jazycích ja
takzvaný cyklus FOR. Tento cyklus umí projít jakýkoliv zadaný seznam prvek po
prvku a pro každý prvek vykonat určitý blok kódu. Představme si například, že
máme seznam známek z písemek nějakého studenta a chceme tyto známky vypsat na
obrazovku, každou na nový řádek. K tomu nám stačí takovýto kousek kódu.

```python
znamky = [1, 3, 2, 1, 1, 2]
for z in znamky:
    print(z)
```

V tomto konkrétním případě tedy náš cyklus prochází seznam známek jednu po
druhé. Známka, která je právě zpracovávána, je uložena v proměnné `z`. Jméno
této proměnné jsme si zvolili tak, aby bylo čitelné, co je v proměnné uloženo,
tedy z jako známka.

Podobně jako v případě podmínek můžeme cyklu FOR předat celý blok příkazů
najednou. Mějme například seznam jmen, kdy za každé jméno chceme přidat konec
e-mailové adresy.

```python
jmena = ['petr', 'pavel', 'jitka', 'jana']
for jmeno in jmena:
    mail = jmeno + '@gmail.com'
    print(mail)
```

Takto vytiskneme na obrazovku maily jednotlivých lidí, každý na jeden řádek.

Jak už bylo napsáno výše, cyklus může obsahovat libovolný blok příkazů, takže
se můžeme opravdu rozparádit a vložit do bloku v cyklu FOR třeba podmínku.

```python
znamky = [1, 3, 2, 1, 1, 2]

pocet_jednicek = 0
for z in znamky:
    if z == 1:
        pocet_jednicek = pocet_jednicek + 1

print("Počet jedniček:", pocet_jednicek)
```

Tímto jsme vlastně vysvětlili to hlavní a zásadní co o cyklu FOR zatím
potřebujeme vědět. Možná se to na první pohled nezdá, ale přidáním cyklu do
našeho programátorského arzenálu jsme otevřeli pandořinu skříňku plnou
možností, co v našich programech můžeme dělat. Taky jsme ale otevřeli bránu do
samotného pekla, neboť už díky cyklům dokážeme řešit mnohem složitější a
komplikovanější problémy, na které ale bude často potřeba pořádně roztočit
mozkové závity.

Ukažme si například jak se pomocí cyklu spočítá součet všech čísel v seznamu.

```python
soucet = 0
for cislo in cisla:
    soucet = soucet + cislo
```

Ne, že bychom zrovna tento cyklus nutně potřebovali. Python obsahuje funkci
`sum()`, která umí dělat přesně toto. Tento příklad ale spíše ukázat, že s
cykly můžeme dělat spoustu zajímavých věci.
