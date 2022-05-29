## Podmínky s více větvemi

Podobně jako u filmů tak i u divadelních představení bychom mohli chtít
jemnější rozdělení přístupnosti nějakého představení. Můžeme například mít
představení nevhodné vyloženě pro malé děti, zatímco teenageri jsou v pohodě.
Budeme tady potřebovat podmínku s více větvemi:

```python
if vek < 6:
    print('Předškolák')
elif vek < 15:
    print('Školák')
elif vek < 18:
    print('Mladistvý')
else:
    print('Dospělý')
```
