## Aritmetické operátory

Nyní už máme prostředky k tomu, abychom mohli pomocí Pythonu něco spočítat. V Python máme k dispozici běžné aritmetické operátory:

* sčítání: `+`
* odčítání: `-`
* násobení: `*`
* dělení: `/`

Díky těmto operátorům můžeme Python použít jako kalkulačku a psát *aritmetické výrazy* jako

```py
12 * 13 + 10
```

### Výpis na obrazovku

Programy automaticky neinformují o každé operaci, kterou provedou, aby nás nezahltily informacemi. Pokud například program provede nějaký výpočet a my chceme vědět jeho výsledek, můžeme využít tzv. funkci. O funkcích si řekneme později více informací, zatím budeme využívat pouze funkci `print()`, která vypíše na obrazovku výraz, který zapíšeme do kulatých závorek.

```py
print(12 * 13 + 10)
```

### Spuštění programu

Abychom výsledek viděli, musíme program spustit. Před spuštěním je potřeba soubor uložit, a to pomocí klávesové zkratky nebo pomocí menu `File` a volby `Save`. Pokud máme nainstalovaný doplněk `Python` pro Visual Studio Code, můžeme ke spuštění použít šipku, která se zobrazí vpravo nahoře. Pozor na to, že šipka se zobrazí pouze v případě, že náš soubor má v názvu příponu `.py`.

Alternativně můžeme ke spuštění programu použít terminál. Ten otevřeme pomocí menu `Terminal` a  volby `New Terminal`. V dolní části obrazovky se zobrazí terminál, což je textové rozhraní pro komunikaci s počítačem. Do terminálu napíšeme příkaz ke spuštění.

Pokud pracujeme v operačním systému Windows, napíšeme do terminálu

```
python program.py
```

Část `program.py` případně nahradíme názvem programu, který chceme spustit.

Pokud používáme operační systém MacOS nebo Linux, pouižjeme příkaz

```
python3 program.py
```

Opět platí, že část `program.py` nahradíme názvem programu, který chceme spustit.

Oba postupy spuštění vedou ke stejnému výsledku. Program se spustí a do terminálu vypíše vše, co chceme vypsat pomocí funkce `print()`. Pokud jsme použili pro spuštění programu šipku a terminál nemáme otevřený, Visual Studio Code nám ho automaticky otevře.

### Další operátory

Python ovšem nabízí ještě další užitečné operátory:

* mocnění: `**`
* celočíselné dělení: `//`
* zbytek po dělení: `%`

Pomocí mocnění můžeme umocňovat čísla, například

```py
print(2 ** 8)
```

Pomocí celočíselného dělení můžeme dělit celá čísla

```py
print(14 // 4)
```

Pokud by nás zajímal zbytek po celočíselném dělení, můžeme použít operátor pro zbytek po dělení

```py
print(14 % 4)
```

### Komentáře

K využití funkcí můžeme přidat vysvětlující poznámku, kterou označujeme jako **komentář**. Komentář je řádka programu, která má programátorům pomoci se v programu zorientovat a při samotném spuštění ji Python ignoruje. Komentář začítáme symbolem `#` a za něj můžeme napsat cokoli.

```python
# Mocnina - 2 na 8
print(2 ** 8)
# Celočíselné dělení
print(14 // 4)
# Zbytek po celočíselném dělení
print(14 % 4)
```