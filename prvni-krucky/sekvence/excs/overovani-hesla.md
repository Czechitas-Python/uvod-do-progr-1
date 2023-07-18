---
title: Ověřování hesla
demand: 3
---

Ověřování hesla se někdy dělá tak, že se vás systém ptá pouze na některé jeho
znaky. Napište program, který má uloženo heslo, které musí uživatel zadat. Pak
se jej postupně zeptejte například na druhý, pátý a sedmý znak hesla.
Propusťte uživatele pouze tehdy, zadá-li všechny tyto znaky správně.

Příklad použití pro heslo _czechitas_:

```shell
Zadej 2. znak hesla: z
Zadej 5. znak hesla: h
Zadej 7. znak hesla: t

Vstup povolen
```

```shell
Zadej 2. znak hesla: e
Zadej 5. znak hesla: h
Zadej 7. znak hesla: t

Vstup zamítnut
```

Bonus bonusu: Program náhodně vygeneruje na jaké tři písmena hesla se bude ptát.
