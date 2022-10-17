Při komplikovanějších výpočtech se nám často stane, že si potřebujeme nějaký
mezivýpočet uložit pro pozdější použití. K tomu nám slouží takzvané
_proměnné_.

Proměnná je jakási pojmenovaná krabička nebo šuplík, do kterého si můžeme
uložit nějakou hodnotu, abychom ji neztratili a mohli ji používat v dalších
výpočtech.

Můžeme například v rámci dietního programu spočítat kolik vanilkových věnečků
denně jsme spořádali za posledních 5 dní.

```pycon
>>> celkem = 1 + 2 + 4 + 1 + 6
>>> prumer = celkem / 5
```

## Jména proměnných

Už do úplných začátků s programováním je dobré učit se dobrým návykům, které
budou později usnadňovat programátorský život nejen vám ale hlavně lidem kolem
vás. Jedním z takových návyků je správné pojmenovávání proměnných.

* Název proměnné by neměl začínat velkým písmenem, např. `Pocet`. Takové názvy jsou rezervované pro speciální typy proměnných, ke kterým se v tomto kurzu nedostaneme.
* Název proměnné by neměl obsahovat diakritiku, např. `počet`. Programovací jazyky vznikaly v anglofonním prostředí, kde se diakritika nepoužívá, takže si ní většina jazyků neporadí.
* Víceslovné proměnné nesmí obsahovat mezeru, např. `pocet hodin`. To by si Python myslel, že to jsou dvě proměnné za sebou a nevěděl by co s tím. Pokud chcete proměnnou s více slovy, použíjte takzvanou velbloudí notaci `pocetHodin` nebo hadí notaci `pocet_hodin`.
* Vždy proměnnou pojmenujte tak, aby její název jasně napovídal, co se uvnitř ní nachází. Například proměnná `pocet_hodin` jasně říká, že v ní bude asi nějaký počet hodin. Můžeme podlehnout touze název proměnné zkrátit například na `pcthd` aby se nám lépe psala. Až ovšem někdo další bude takový program číst, bude mlátit hlavout do stolu cože proboha znamená zkratka `pcthdn`.
* Naposledy je dobré si uvědomit, že programy i programátoři se téměř vždy pohybují v mezinárodním prostředí. Takže je vždycky lepší pojmenovávat proměnné anglicky. V tomto kurzu ještě tohle pravidlo trošku rozvolníme, ale i tak si můžete začít zvykat na proměnné s názvem `number_of_hours`.
