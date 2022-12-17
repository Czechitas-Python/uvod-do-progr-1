## Seznamy

Ty vůbec nejpoužívanější sekvence jsou ovšem seznamy. Do nich lze uložit
jakékoliv množství hodnot jakéhokoliv typu. Dokonce můžeme mít seznamy
seznamů.

```python
znamky = [2, 3, 4, 1, 1]
teploty = [13.4, 13.5, 12.8, 11.9]
uzivatele = ['mark', 'carl', 'eve', 'ellen']
platby = ['Jan Novák', 12000, True]
body = [[140, 120], [60, 92], [34, 68]]
```

Přístupy k indexům sekvencí se dají skládat za sebe. Můžeme tak získat
například čtvrté písmenko druhého jména v seznamu `uzivatele`

```python
print(uzivatele[1][3])  # 'l'
```

nebo první číslo třetího seznamu v proměnné `body`

```python
print(body[2][0])  # 34
```
