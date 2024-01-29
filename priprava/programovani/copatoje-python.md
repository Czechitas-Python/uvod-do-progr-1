## Co je to "Python"?

Jistě už tušíte, že **Python** je programovací jazyk a že ho budeme používat pro to, abychom se domluvili s počítačem a dali mu tak instrukce, co po něm budeme chtít vykonat.  
Co to ale takový programovací jazyk je?  
Zjednodušeně bychom mohli říci, že většina programovacích jazyků je tvořena:

- souborem slov a pravidel ke psaní programů - gramatikou
- způsobem jak tyto napsané programy spustit
- názvoslovím pro jednotlivé části (soubory, složky, spouštěče, překladače, ...)

V následujících lekcích se budeme učit psát programy právě v jazyce _Python_ a tyto speciální slova a pravidla si ukážeme.  

### Psaní

Nejprve je potřeba nějaký svůj první soubor (v Pythonu nazývaný `script`, nebo `modul`) vytvořit a napsat do něj příkazy tak, aby jim _Python_ rozuměl.  
U Pythonu je to velmi snadné, protože jeho soubory jsou tvořené obyčejným textem. Napíšete je tedy stejně snadno jako byste si vytvářeli například poznámku `poznamka.txt` jen místo koncovky `.txt` použijete koncovku pro python scripty `.py`. Váš první program tedy může mít například název `prvni_program.py`.
Python soubory nejsou nijak zamotané a dají se tak snadno číst, kopírovat a sdílet mezi lidmi.

Programátoři si usnadňují psaní programů tím, že k programování používají speciální editory (vývojové prostředí, IDE), které jim tvorbu souborů usnadňují, podporují chytré vyhledávání, zvýrazňování pravidel pro jednotlivé programy a také jednoduché spuštění.  
My budeme v rámci kurzu používat vývojové prostředí _Visual Studio Code_, které je velmi univerzální a rozšířené.

### Spouštění

Pokud budeme chtít aby počítač vykonal, co jsme mu připravili, budeme potřebovat takzvaný **Python interpreter**.  
To je ten "program", který jste si stáhli a nainstalovali ze stránek [python.org](https://www.python.org). 
Python interpreter je jakýsi překladač a spouštěč, který váš soubor vezme, podívá se, co je v něm napsané, a řádek po řádku bude počítači říkat (už řečí, které rozumí jen počítače) co má přesně udělat.  
My tak nemusíme umět přímo řeč počítačů, ale stačí nám jednoduchá a přehledná gramatika Pythonu. Vše ostatní zařídí právě interpreter.

Jelikož je Python oblíbený jazyk, jeho vývoj pokračuje stále dopředu a i jeho gramatika se vyvíjí (pravidelně jednou ročně v listopadu). Starší verze Pythonu (interpreteru) tak už například nerozumí slovíčkům z novějších verzí.  
Nemusíte mít ale obavy, velká změna nastala jen při přechodu mezi verzemi 2 a 3. Pokud budete používat Python verze `3.7` a vyšší, bude vše zpravidla fungovat tak, jak má.

Co když má ale někdo někde schovaný program po babičce, psaný ještě ve verzi 2? Jakým způsobem by šel spustit?  
Na počítači můžete mít v jednu chvíli nainstalováno python interpreterů kolik budete chtít, dokonce i v různých verzích.
Někdy je to dokonce i potřeba abyste si ověřili, že váš program půjde spustit i ve starší verzi, kterou má u sebe nainstalovanou kolega.  
Při spuštění vašeho programu, pokud neřeknete jinak, se vždy použije právě první interpreter, který počítač na své cestě (vnitřní seznam nainstalovaných programů) najde.

Aby to nebylo tak jednoduché, tak z interpreterů, které máte nainstalované, můžete ještě vytvářet speciální kopie pro své projekty.  
Těmto "kopiím hlavních interpreterů" se říká :term{cs="virtuální prostředí" en="virtual environment"} a často ho uvidíte pod názvem `venv` nebo `.venv`.  
Používáme to v případě, že chceme mít ve svých projektech hezky uklizeno a nechceme, aby na sobě byly jednotlivé projekty přes náš hlavní interpreter závislé.

Na obrázku níže tak vidíte příklad, kdy máme nainstalované dva intepretery (dvě verze Pythonu) ve verzích `3.7.0` a `3.6.5` a vytvořili jsme si z nich tři kopie, pro každý projekt jednu.

::fig[Notebook]{src=assets/python_envs.png}

Pokud chceme program spouštět právě přes vývojové prostředí (Visual Studio Code), je potřeba mu nastavit, který interpreter má pro náš projekt používat.
Ze začátku si s tím nemusíte příliš lámat hlavu, můžete použít ten jediný, který máte právě nainstalovaný. 

### Zajímavosti na konec  

> Jak už víme, tak Python interpreter je program, který spouští naše soubory. V jakém jazyce je ale **on sám** napsaný??
> Hlavní oficiální verze, kterou jste si stáhli je psaná v _jazyce C_. Existuje ale i několik dalších verzí (říkáme jim příchutě) napsaných například v jazyce _Java_, _Ruby_, _Rust_ a dalších.
> Více se o nich můžete dočíst [zde](https://wiki.python.org/moin/PythonImplementations).

> I přesto, že má Python dva hady jako své logo, název _Python_ není inspirován hadem.  
> _Python_ je pojmenovaný po Britské komediální skupině _Monty Python's Flying Circus_.