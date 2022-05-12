Cílem tohoto kurzu není z vás udělat programátory, protože to je běh na mnohem
delší trať než na jakou máme během jediného dne čas. Co ale za jeden den
stihneme, je nahlédnout pod pokličku toho, jak vypadá každodenní práce
programátora nebo vývojáře a ochutnat jaké problémy se v programátorské praxi
řeší.

Programování z velké části sestává z psaní kódu v nějakém programovacím
jazyce. Než ale vůbec můžeme začít něco takzvaně kódit, musíme si dobře
rozmyslet, jak zadaný problém vlastně budeme řešit. Je to podobné jako když
spisovatel nejdříve vymyslí zápletku příběhu a až poté může sednout k počítači
a začít ťukat obsah knihy.

## Problém spolubydlení

Psát kód zatím ještě neumíme, ale programátorský způsob přemýšlení nad
problémy si můžeme vyzkoušet už nyní.

Představte si šest spolubydlících: Libora, Zuzku, Patra, Pavlu, Ondru a Míšu.
Žijí v jednom bytě a dělí se o náklady na společně používané věci jako je
toaletní papír, mýdlo, prací prášek apod. Postupně svoje útraty zapisují do
tabulky, která může vypadat například takto:

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

Dejme tomu, že uplynulo například půl roku a spolubydlící se chtějí navzájem
finančně vyrovnat. Vaším úkolem je vymyslet přesný postup, který mají
následovat, aby došlo k celkovému vyrovnání všech lidí. Důležité je, že tento
postup musíme vymyslet tak, abychom jej později dokázali sdělit počítači, což
znamená, že náš postup musí být opravdu detailní. Nelze přikazovat věci typu
"rozpočítej útratu mezi všechny účastníky". Takové příkazy počítač nezná.
Budeme muset pracovat s určitými omezeními.

### Počítač za nás nebude přemýšlet

Počítač si můžeme představit jako naprosto hloupého úředníka s tužkou, papírem
a kalkulačkou. Naprosto nerozumí pojmům jako účastník, částka, rozpočítat
apod., vůbec neumí samostatně přemýšlet. Všechno mu musíme vysvětlit
polopaticky a nevynechat žádný detail, na kterém by se mohl zaseknout. On umí
pouze základní početní operace na kalkulačce, umí si něco poznamenat na papír
a to je tak všechno.

### Počítač nekouká doleva ani doprava

Pokud se podíváte na naši tabulku výdajů, možná budete mít nutkání ji vyřešit
tak říkajíc šmahem: prostě kouknu a vidím, nějak to tady přičtu, tady odečtu a
hotovo. To se může celkem povést pro tabulku o šesti lidech. Těžko ale takový
postup uplatníme například pro menší  švýcarskou vesnici, která má 375 obyvatel
a v tabulce výdajů je 8 822 záznamů. Pro vaši představu, taková data zaberou
oboustranně 197 listů A4 a těžko je můžeme zpracovat šmahem.
