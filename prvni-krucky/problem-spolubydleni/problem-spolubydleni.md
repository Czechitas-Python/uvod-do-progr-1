Možná se to nezdá, ale těch několika lekcích, kterými jste prošli, jste již
vybavení téměř všemi nezbytnými technickými dovednostmi k tomu, abyste
dokázali naprogramovat řešení našeho problému se spolubydlením ze začátku
kurzu. Pravda, po takto krátkém kurzu ještě nemáte dost zkušeností na to,
abyste si na výsledný program troufli sami. Když jej ale uvidíte už napsaný,
začnete poznávat téměř všechny věci, které jsou v programu použity - proměnné,
podmínky, seznamy, cykly a další.

## Řešení

Připomeňme si tabulku výdajů, kterou jsme viděli na začátku kurzu.

Jméno | Věc | Částka
----- | --- | ------
Petr| Prací prášek| 240 kč
Ondra| Savo| 80 kč
Pavla| Toaleťák| 65 kč
Zuzka| Mýdlo| 50 kč
Pavla| Závěs do koupelny| 350 kč
Libor| Pivka na kolaudačku| 124 kč
Petr| Pytle na odpadky| 75 kč
Míša| Utěrky na nádobí| 130 kč
Ondra| Toaleťák| 120 kč
Míša| Pečící papír| 30 kč
Zuzka| Savo| 80 kč
Petr| Tapeta na záchod| 315 kč
Ondra| Toaleťák| 64 kč

Popis řešení v lidské řeči by mohl vypadat například takto:

* Spočítej kolik každý člen utratil celkem,
* spočítej průměrnou útratu na jednoho člena,
* spočítej rozdíly jednotlivých členů proti průměru,
* všechny peníze těch, kteří zaplatili podprůměr, dej do banku,
* bank rozděl mezi ty, kteří zaplatili nad průměr.

### Python program

Jelikož už umíme v Pythonu reprezentovat data pomocí seznamů, můžeme výše
uvedenou tabulku zapsat jako seznam seznamů takto:

```python
vydaje = [
    ['Petr', 'Prací prášek', 240],
    ['Ondra', 'Savo', 80],
    ['Pavla', 'Toaleťák', 65],
    ['Zuzka', 'Mýdlo', 50],
    ['Pavla', 'Závěs do koupelny', 350],
    ['Libor', 'Pivka na kolaudačku', 124],
    ['Petr', 'Pytle na odpadky', 75],
    ['Míša', 'Utěrky na nádobí', 130],
    ['Ondra', 'Toaleťák', 120],
    ['Míša', 'Pečící papír', 30],
    ['Zuzka', 'Savo', 80],
    ['Petr', 'Tapeta na záchod', 315],
    ['Ondra', 'Toaleťák', 64]
]
```

Druhý krok je přeložit lidský popis řešení do Python kódu. Takový program by
mohl vypadat například takto:

```python
import statistics

seznam_jmen = []
utraty = []

for vydaj in vydaje:
    jmeno = vydaj[0]
    utrata = vydaj[2]

    if jmeno in seznam_jmen:
        index = seznam_jmen.index(jmeno)
        utraty[index] += utrata
    else:
        seznam_jmen.append(jmeno)
        utraty.append(utrata)

prumernaUtrata = statistics.mean(utraty)

for jmeno in seznam_jmen:
    index = seznam_jmen.index(jmeno)
    vyrovnani = round(utraty[index] - prumernaUtrata)

    if vyrovnani > 0:
        print(jmeno + ' dostane\t' + str(vyrovnani))
    else:
        print(jmeno + ' má dáti\t' + str(-vyrovnani))
```

Seznamy v proměnných `seznam_jmen` a `utraty` představují tabulku celkových útrat
pro každého jednoho člověka.
