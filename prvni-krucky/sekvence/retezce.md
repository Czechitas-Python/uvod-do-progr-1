Do této chvíle jsme uměli do nějaké proměnné uložit pouze jednu hodnotu,
například číslo nebo řetězec. Počítače ale často potřebují pracovat v mnohem
větším objemem dat, než je několik čísel nebo řetězců.

## Řetězce

Sekvence nám umožňují do jedné proměnné uložit více hodnot. Hodnoty uvnitř
sekvencí sídlí na takzvaných _indexech_ , které se vždy počítají od nuly. To
je takový zvláštní programátorský úzus, že se většinou začíná počítat od nuly
a ne od jedničky. Má to svoje důvody, které tady ovšem nebudeme rozvádět.
Raději si rovnou ukážeme jedna z nejjednodušší sekvencí, a to je řetězec. Díky
tomu, že řetězec je sekvence, je možné přistupovat k jednotlivým jeho prvkům,
v tomto případě písmenům.

```python
jmeno = 'hubert'
print(jmeno[0])  # 'h'
print(jmeno[4])  # 'r'
```
