# 1  Softwarové inženýrství

###### tags: `řsss-základ`, `swing`
> Softwarové inženýrství. Proces vývoje SW. Metodika Unified Process (UP). Agilní vývoj SW. Fáze testování a typy testů. Softwarové metriky, refaktoring kódu. Odhadování úsilí. Údržba a znovupoužitelnost. Kvalita softwaru. (PA017)

> Stranka, kde je tema spracovana o dost strucnejsie http://statnice.dqd.cz/mgr-szz:in-gra:21-gra
 
> https://docs.google.com/document/d/1JVC34-jBqK-hnyxty9YNelID_LChUsvREdgS9NaEjvI/edit#heading=h.jnc4k9d4jod3

## Softwarové inženýrství
- Softwarové inženýrství je samostatný inženýrský obor, který řeší systematický přístup k vývoji, provozování, údržbě a nahrazování software.
- Jako obor s certifikátem v USA uznáno v roce 1997.
- Chybí ucelená teorie, základní terminologie není jednotná.
- Praktici používají kolekce technik, které se zdají být funkční.

### Dobře řešený software
- **Udržovatelnost**: Měl by být umožněn vývoj SW podle měnících se potřeb zákazníka.
- **Spolehlivost**: Mezi atributy SW, na který je spolehnutí, patří spolehlivost, ochrana a bezpečnost. SW by neměl při výpadku systému způsobit fyzické, ani ekonomické škody.
- **Efektivita**: SW by neměl plýtvat prostředky systému (paměť, čas procesoru a pod.).
- **Použitelnost**: SW by měl mít přiměřené uživatelské rozhraní a odpovídající dokumentaci.

### Kritické faktory SW produktivity
- **Složitost**: Lze ji charakterizovat nepřímo, některými viditelnými atributy programu (architektura, počet proměnných).
- **Velikost**: Programování v malém vs. programování ve velkém.
- **Komunikace** Jednotlivec, malý tým, velký tým.
- **Čas, plán prací**
- **Neviditelnost SW**

### Programování v *malém*
- Ověřené techniky.
- Shora-dolů, strukturované kódování, postupné zjemňování, zdokonalování (step-wise refinement).
- Inspekce logiky a kódu.
- Nástroje - překladače, odvšivovače.

### Programování ve *velkém*
- Plánovací mechanismy - dělení práce, harmonogram, zdroje.
- Dokumentovaná specifikace.
- Strukturovaný tým.
- Formalizované soubory testů, testovací příklady.
- Formalizované inspekce.

## Proces vývoje SW
Vývoj software je proces, při němž jsou:
- **uživatelovy potřeby**
    - 🡓 transformovány na
- **požadavky na software**
    - 🡓 transformovány na
- **návrh**
    - 🡓 implementován jako
- **kód**
    - 🡓 testován, dokumentován a certifikován pro
- **operační použití**

### Základní aktivity při vývoji SW
- **Specifikace**: Je třeba definovat funkcionalitu SW a operační omezení.
- **Vývoj**: Je třeba vytvořit SW, který splňuje požadavky kladené ve specifikaci.
- **Validace**: SW musí být validován („kolaudován“), aby bylo potvrzeno, že řeší právě to, co požaduje uživatel.
- **Evoluce**: SW musí být dále rozvíjen, aby vyhověl měnícím se požadavkům zákazníka.

### Viditelné znaky výroby SW

- **Artefakty**
    - Výpisy programů
    - Dokumentace
    - Data
    - Zdrojové soubory
- **Procesy**
    - Pracovní postupy
    - Uznávaná pravidla (rules-of-thumb)
    - Interakce mezi členy týmu

### Charakteristiky výrobního procesu SW
- **Srozumitelnost**: Je proces explicitně definován a je snadné porozumět definici procesu?
- **Viditelnost**: Vyúsťují procesní aktivity ve zřetelné výsledky tak, že postup procesu je viditelný zvenčí?
- **Spolehlivost**: Je proces navržen tak, že se lze chybám procesu vyhnout, nebo je zachytit dříve, než zaviní chyby ve výrobku?
- **Přijatelnost**: Je definovaný proces přijatelný a použitelný inženýry zodpovídajícími za produkci?
- **Robustnost**: Může proces pokračovat i v po výskytu neočekávaných problémů?
- **Udržovatelnost**: Může se proces vyvíjet tak, aby odrážel měnící se organizační požadavky nebo identifikovaná zlepšení procesu?
- **Rychlost**: Jak rychle lze realizovat výrobní proces, který z dané specifikace vytvoří hotový systém předaný zákazníkovi?
- **Podporovatelnost**: Do jaké míry lze aktivity procesu podpořit nástroji CASE? (CASE nástroje primárně umožňují modelování IT systému pomocí diagramů)

### Model životního cyklu „vodopád“ 
**Manažeři tento model preferují.**
- Postupovat podle vodopádového modelu znamená přecházet od jedné fáze k následující přísně **sekvenčním** způsobem. Nejprve se například připraví specifikace požadavků, které jsou pevně dané. Teprve když jsou požadavky úplně kompletní, přejde se k návrhu. 
- Integrace systému zároveň s jeho testy
- Problémy s cenou v případě nezdaru v některé z pozdějších etap

![](https://i.imgur.com/eTysolt.jpg)

#### Problémy
- špatná reakce na změnu - **velký problém!**
- Reálné projekty nedodržují jednotlivé kroky v předepsaném pořadí.
- Uživatel nedokáže v počátečních etapách formulovat požadavky na systém zřetelně a přesně.
- Zákazník musí být trpělivý.
- Pozdní odhalení nedostatků může vážně ohrozit celý projekt.

#### Viditelnost životního cyklu „vodopád“ 


| Aktivita | Výstupní dokumenty |
| -------- | -------- |
| Analýza požadavků | Studie proveditelnosti <br/>Obrysové požadavky |
| Definice požadavků | Dokument požadavků |
| Specifikace systému | Funkční specifikace<br/>Plán testování<br/>Návrh uživatelského manuálu|
|Návrh architektury |Specifikace architektury<br/>Plán testování systému|
|Návrh rozhraní |Specifikace rozhraní<br/>Plán integračních testů|
|Podrobný návrh |Specifikace návrhu<br/>Plán testování jednotek|
|Kódování | Kód programu|
|Testování jednotek | Protokol o testování jednotek|
|Testování modulů | Protokol o testování modulů |
|Integrační testování | Protokol integračních testů<br/>Konečný uživatelský manuál|
|Testování systému | Protokol testování systému|
|Přejímací testování | Konečný systém a dokumentace|


### Model „inkrementálního“ životního cyklu

Modifikace vodopádového modelu. Finální projekt je rozdělen na dílčí verze, jednoduší části, vznikají tzv. inkrementy, na které postupně přidáváme (nabalujeme) další funkcionalitu (princip verzování). Jednotlivé verze se vyvíjejí vodopádovým modelem, ale čas na jejich realizaci je menší a můžeme sledovat vývoj systému.


![](https://i.imgur.com/9ED9wK3.png)
#### Problémy
- Obrysová specifikace vs. skutečnost
- Dokumentace programu vs. specifikace
- Údržba zvyšuje entropii

#### Vývoj podle obrysové specifikace

- **Jsou vyžadováni vysoce talentovaní pracovníci**. Průměrný tým nelze použít pro tento typ vývoje. Úspěšné produkty byly takto vytvořeny malými týmy vysoce talentovaných pracovníků.
- **Systémy jsou obvykle špatně strukturované.** Neustálé změny poškozují strukturu systému. Evoluce je obtížná a nákladná.
- **Proces není viditelný.** Manažer potřebuje pravidelné výstupy, aby mohl řídit proces. Při rychlém vývoji není efektivní produkovat dokumenty, které přesně zachycují každou verzi.

### Model životního cyklu „prototypování“ 


![](https://i.imgur.com/XEhOlf9.png)


- Tvorba prototypů probíhá za účelem získávání poznatků, **neslouží** jako předloha k vývoji
- Po specifikaci je prototyp zapomenut

### Model životního cyklu „výzkumník“ 
![](https://i.imgur.com/oPaimNn.png)
![](https://i.imgur.com/9QlvFLL.png)


#### Problémy
- Obtížné manažerské řízení
- Neexistující či neplatná dokumentace
- Nenahraditelnost řešitelů

Je to experimentování, u kterého často netušíte, jak dopadne. Metoda pokus/omyl, ve snaze zjistit od zákazníka co vlastně chce tím, že mu předkládáme hotové systémy.

### Spirálový model životního cyklu (Boehm, 1988)
Dochází zde k neustálému opakování jednotlivých stavů vývoje *navrhnu-naimplementuju-zkusím*. Mezi jednotlivé verze (inkrementy) jsou vloženy další procesy jako zhodnocení verze z pohledu finálního systému, či přidání nových požadavků zákazníka.

![](https://i.imgur.com/zAZwSxt.png)

## Metodika Unified Process (UP).
Generický proces pro UML specifikaci, který lze libovolně přizpůsobit (metodika není vázaná licencí).
Proces definuje KDO udělá CO, a KDY a JAK to udělá, aby se dosáhl nějaký cíl.
- Iterativní a inkrementální
- Řízen use casy
- Zaměřen na architekturu systému.

Neexistuje žiaden univerzálny proces. UP je flexibilný a rozširiteľný

### Fáze dle UP
- **Zahájení**: Definice rozsahu projektu, vytvoření byznisového cílu
- milník: vize
- **Příprava**: Naplánování projektu, specifikace funkcionality, navrhnutí architektury
- milník: základ architektury
- **Konstrukce**: Vývoj produktu
- milník: počáteční funkcionalita
- **Předávání**: Předání produktu uživatelům
- milník: release produktu

### Workflows

![](https://i.imgur.com/2vS4q8d.png)

### Modely
![](https://i.imgur.com/r6uY6d6.png)

- **Diagram tříd**: Popis objektového modelu systému. Znázorňuje objekty, jejich atributy, metody a vztahy mezi ostatními objekty.
- **Sekvenční diagram**: Sekvenčně popisuje nějaký proces v systému. Znázorňuje komunikaci mezi objekty pomocí zpráv (funkční volání). Objekty “žijí” v průběhu tzv. lifelines.
- **Kolaborační diagram**: Podobný sekvenčnímu diagramu. Sekvence je ale očíslována. Toto číslování specifikuje pořadí volání metod.
- **Stavový diagram**: Znázorňuje takovou událost probíhající v systému, která má konečný počet stavů. Má formu stavového automatu. Jeho součástí jsou stavy, přechody a události.
- **Diagram aktivit**: Zachycuje proměnné chování (flow) nějaké aktivity v systému. Popisuje sekvenci přechodu od jedné aktivity k druhé. Popisuje i paralelní, rozvětvené a souběžné flows systému.
- **Use case diagram**: Znázorňuje případy použití systému. Různé role (actors) mohou mít různé případy použtí.
- **Diagram komponent**: Znázorňuje komponenty použité v systému, tj. logické komponenty či fyzické komponenty
- **Diagram nasazení**: ukazuje rozmístění zdrojů (např. HW) a softwarové komponenty, procesy a objekty, které na nich žijí.


### Diagramy - Use case model
![](https://i.imgur.com/GHnamkj.png)
### Diagramy - Analysis & Design model
![](https://i.imgur.com/R1RXvDW.png)
### Diagramy - Deployment and Implementation model
![](https://i.imgur.com/SUYtnUA.png)
### Diagramy - Test model
Test model odkazuje na predchádzajúce modely a používa ich odpovedajúce diagramy


## Agilní vývoj SW
Agile = hbitý, čilý, bystrý, svižný.

### Manifest agilního programování

Umožnit změnu je mnohem efektivnější, než se jí snažit zabránit.

Je třeba být připraven reagovat na nepředvídatelné události,
protože ty nepochybně nastanou.

- **Individuality a interakce** mají přednost před **procesy a nástroji**.
- **Fungující software** má přednost před **obsáhlou dokumentací**.
- **Spolupráce se zákazníkem** má přednost před **sjednáváním smluv**.
- **Reakce na změnu** má přednost před **plněním plánu**.


![](https://i.imgur.com/hYcaRTd.png)

### Společné rysy agilních metodik
#### Iterativní a inkrementální vývoj s krátkými iteracemi
Vývoj probíhá v krátkých fázích, takže celková funkcionalita je dodávána po částech.

Zákazník tak má možnost průběžně sledovat vývoj, muže se k němu vyjádřit a oponovat změny.

Zákazník má na konci jistotu, že nedostane něco, co neočekával.

#### Komunikace mezi zákazníkem a vývojovým týmem
V ideálním případě je zákazník přímo součástí vývojového týmu, má možnost okamžitě vidět průběžné výsledky a reagovat na ně.

Zákazník se účastní sestavování návrhu, spolurozhoduje o testech a poskytuje zpětnou vazbu pro vývojáře.

#### Průběžné automatizované testování
Díky krátkým iteracím se aplikace mění velice rychle, proto je nutné pro zajištění co nejvyšší kvality  ověřovat její funkčnost průběžně.

Testy by měly být automatizované, předem sestavené a měly by být napsány ještě před samotnou implementací testované části.

Při každé změně musí být aplikována kompletní sada testů, aby nebyla porušena integrace jednotlivých částí 


### Konkrétní metodiky
#### Extreme Programming
Hodí se pro menší projekty a malé týmy, vyvíjející software podle zadání, které je nejasné nebo se rychle mění.

Jediným exaktním, jednoznačným, změřitelným, ověřitelným a nezpochybnitelným zdrojem informací je zdrojový kód.

Používá běžné principy a postupy, které dotahuje do extrému.
Například:
- Jestliže se osvědčují revize kódu, bude se neustále revidovat (myšlenka párového programování)
- Pokud se vyplácí testování, bude se nepřetržitě testovat, a to i u zákazníka (testování jednotek, funkcionality, akceptační testy).
- Osvědčuje-li se návrh, stane se součástí každodenní činnosti (refaktorizace).

##### Principy XP
- **Rychlá zpětná vazba**, která spočívá v rychlém zjištění stavu systému po provedené akci, vyhodnocení akce a uložení výsledku vyhodnocení co nejdříve zpět do systému.
- **Předpoklad jednoduchosti**, představuje v mnoha ohledech nejobtížnější princip,protože je v protikladu s tradičním pojetím programování, kdy se vše plánuje a navrhuje do budoucna tak, aby to bylo znovu použito. XP naopak předpokládá u řešitelského týmu schopnost přidat složitost tam, kde to bude v budoucnu účelné.
- **Přírůstková změna**, vychází z předpokladu, že velké změny provedené najednou nefungují. Veškeré změny v projektu se proto provádějí pomocí malých přírůstků. 
- **Využití změny**, vychází z předpokladu, že nejlepší strategie je ta, která si zachová co nejvíce možností řešení nejnaléhavějších problémů projektu.
- **Kvalitní práce**, která představuje fixní proměnnou ze čtyř proměnných pro posouzení projektu (šíře zadání, náklady, čas a kvalita) s hodnotou vynikající, při horší hodnotě členy týmu práce nebude bavit a projekt může skončit neúspěchem.

#### Feature-Driven Development
Vývoj po malých kouscích (vlastnostech, rysech), což jsou elementární části funkcionality přinášející nějakou hodnotu uživateli.

Vývoj probíhá v pěti fázích, první tri jsou sekvenční, poslední dvě pak iterativní.
Iterace trvají zpravidla 2 týdny. Začíná se vytvořením modelu, ten se převede do seznamu vlastností, které se postupně implementují.

Měří pokrok ve vývoji projektu, FDD detailně plánuje a kontroluje vývojový proces. 

Zaměření na dodávání fungujících přírůstku každé dva týdny

![](https://i.imgur.com/vtHJKqG.png)

#### SCRUM Development Process
Principem je opět iterativní vývoj definující 3-8 fází (tzv. sprintu), z nichž každá trvá přibližně měsíc.

Nedefinuje žádné konkrétní procesy, pouze zavádí pravidelné každodenní schůzky vývojového týmu (scrum meetings), kde si jednotliví členové sdělují, které položky byly od minulé schůzky dokončeny, které nové úkoly nyní přijdou na řadu a jaké překážky stojí vývoji v cestě a musí se řešit.

Každý sprint je zakončen předvedením funkční demo-aplikace zákazníkovi, který poskytne zpětnou vazbu.

##### Co je to product backlog?
Je to jednoduše seznam věcí které se na projektu musí udělat. Každá položka obsahuje odhad potřebného času na dokončení a prioritu. Nahrazuje klasickou specifikaci požadavků. Položky backlogu mohout mít jak technickou (přidat tuto funkcionalitu, fixnout tento bug) tak uživatelskou povahu (zjednodušit uživatelské rozhraní). Product owner ho používá při plánování sprintu k zadávání úkolů.

![](https://i.imgur.com/oMax0xG.png)
![](https://i.imgur.com/vCZxOWb.png)

#### Test-Driven Development
Nezabývá se tvorbou specifikací, plánu a dokumentace, to si každý tým musí zvolit sám podle toho, jak mu to vyhovuje. 

Doporučuje přistoupit k testům jako k hlavní fázi celého vývojového procesu.

Základním pravidlem je psát testy dříve než samotný kód a implementovat jen přesně ty části kódu, které projdou testem.


![](https://i.imgur.com/4nCgjmy.png)

#### Srovnání metodik z pohledu životního cyklu SW

![](https://i.imgur.com/uiBtZdz.png)

## Fáze testování a typy testů
### Produkty podle etap
![](https://i.imgur.com/hJjbRZG.png)


- Testování je proces spuštění programu s cílem nalézt chyby.
- Dobrý testovací případ má vysokou pravděpodobnost nalezení dosud nenalezené chyby.
- Úspěšný test je takový, který odhalí dosud neodhalenou chybu.

~~Test je úspěšný, pokud neodhalí žádné anomálie na výstupu programu.~~
Test je úspěšný, pokud zjistí přítomnost jedné či více chyb v programu. (Myers, 1979)

##### Co testování ukazuje?
- Testování nemůže ukázat nepřítomnost defektů, může pouze ukázat, že v softwaru jsou chyby.
- Testování také ukazuje funkce a výkon.
- A je také ukazatelem kvality software.

### V - procesní model

![](https://i.imgur.com/PfcKF5E.png)
- upravená varianta vodopádu, která zdůrazňuje verifikaci (studie proveditelnosti, revize, inspekce,…) a validaci (testování)
- testování produktu je plánováno paralelně s jednotlivými fázemi vývoje
- účinnost odhalení chyb se zvyšuje verifikací – může být až 80%!


**Validace**: test proti specifikovaným funkcím (“Dělat správné věci”)
**Verifikace**: test proti vnitřní činnosti (“Dělat věci správně)


- Testování je destruktivní činnost! 
- Programátor není dobrým testerem vlastního výtvoru.
- Detailní znalost struktury programu usnadňuje hledání a opravu chyb.
- Je nutná spolupráce dvou nezávislých, organizačně samostatných týmů.

#### Úplné testování není realizovatelné.
I u malých programů může být počet různých logických cest ohromný. Program se 100 řádky, několik vnořených cyklů, každý proveden 20 krát. Existuje přibližně 1014 možných cest, které mohou být provedeny. Při rychlosti 1 test/ms by testování trvalo 3170 roků! 

#### Selektivní testy
- I tehdy, kdy úplné testování není reálné (prakticky vždy!), testování „bílá skříňka“ by nemělo být vynecháno.
- Důležité logické cesty a cykly by měly být testovány.
- Selektivní testování validuje rozhraní a vytváří důvěru ve vnitřní činnost software.

#### Dynamické testování

- Provedení počítačového programu s předem určenými vstupy.
- Porovnání dosažených výsledků s očekávanými výsledky.
- Testování je vlastně vzorkování, nemůže absolutně prokázat absenci defektů.
- Každý software má vši, testování nezaručí odvšivení.

#### Testovací případy
- Klíčové položky plánu testování.
- Mohou obsahovat skripty, data, kontrolní seznamy.
- Mohou mít vztah k *Matici pokrytí požadavků* (nástroj pro sledování)

### Testování „černá skříňka“
- Funkční testování
- Program je “černá skříňka”
    - Nezajímá nás, jak to pracuje, ale co to dělá.
    - Zaměřeno na vstupy & výstupy
- Testovací případy založené na SRS (specifikacích požadavků)

![](https://i.imgur.com/a8g3kOA.png)


### Testování „bílá skříňka“
- Zohledňuje strukturu programu
- Pokrytí
    - provedené příkazy
    - cesty průchodu kódem


![](https://i.imgur.com/3VEEy5m.png)


- Vývojový diagram není nutný, ale obrázek pomůže vysledovat příslušné cesty.
- Testy základních cest by měly být provedeny u kritických modulů.

### Testování jednotek, modulů

- Typ testování „bílá skříňka“
    - někdy ale jako „černá skříňka“
- Kdo testuje jednotky?
    - vývojáři
    - testy jednotek jsou programovány
        – stejný jazyk jako moduly
        – alt.název “Testovací drivery”
- Individuální testy mohou být seskupeny
    - „Kolekce testů“ (Test suites)
- Kdy se testují jednotky?
    - postupně během vývoje
    - po dokončení individuálních modulů

### Integrace & Testování
- Vývoj/integrace/testování
    - nejčastější místo, kde dochází k překrývání aktivit
- Někdy je integrace/testování považováno za jednu etapu
- Postupně propojuje funkcionalitu
- QA tým pracuje souběžně s vývojovým týmem

### Integrační postupy
#### Shora dolů (TDT)
- Nejprve je implementováno jádro (kostra) systému.
- Zkombinováno do minimální „skořápky“ systému.
- Pro doplnění neúplných částí se použijí „protézy“ nahrazované postupně aktuálními moduly.

použití „stubs“ (pahýly, protézy) - jednoduché náhražkové objekty se shodným rozhraním.

**Testování shora-dolů odhaluje chyby analýzy a návrhu, je v souladu s prototypováním.**

**Nevýhody TDT:**
- Složité objekty, moduly, nelze jednoduše zaměnit za „protézu“.
- Výsledky testů na vyšších úrovních nemusí bý přímo „viditelné“.

#### Zdola nahoru (BUT)
- Začne s individuálními moduly a sestavuje zdola.
- Individuální jednotky (po testování jednotek) jsou kombinovány do subsystémů.
- Subsystémy jsou kombinovány do celku.

klasický testovací proces s nadřazenými testovacími objekty - „drivers“.

**Nevýhody BUT:**
- Čas a náklady na konstrukci „drivers“ pro testování jsou obvykle vyšší, než u „protéz“.
- Až v závěru vznikne program použitelný pro předvedení, ve formě „prototypu“.

**Obě metody mají své nevýhody, nelze říci, že jedna je nejlepší.**

### Atributy integrace
- Kdo dělá integrační testování?
    - vývojářský a/nebo QA tým
- Počet pracovníků a rozpočet jsou na vrcholu
- „Jde do tuhého“
- Problémy:
    - práce pod tlakem
    - blíží se datum odevzdání
    - neočekávaná selhání (vši)motivační problémy
    - konflikty při přejímání zákazníkem


![](https://i.imgur.com/nKvLQRU.png)

## Softwarové metriky
### Míra
Kvantitativní údaj o množství, rozměrech, kapacitě, nebo velikosti nějakého atributu, produktu nebo procesu. (Počet chyb)

- **Přímá míra** (vnútorné vlastnosti): počet řádek kódu (LOC), rychlost výpočtu, velikost paměti, počet chyb za určitou dobu, …
- **Nepřímá míra** (vonkajšie vlastnosti): funkčnost, kvalita, složitost, pracnost, spolehlivost, schopnost údržby,…
### Metrika 
Kvantitativní (číselně vyjádřená) míra, tj. ukazatel do jaké míry se nějaký atribut vyskytuje v systému, komponentě nebo procesu. (Počet chyb na 1000 řádků)
Metrika může mít i kvalitativní charakter, tj. nečíselné vyjádření. 

- **Procesné metriky**
    - Poskytujú náhľad do procesných modelov, úloh softwarového inžinierstva, produktov alebo míľnikov
    - Vedú k dlhodobému zlepšovaniu procesov
    - činnosti spojené s vývojem, doba strávená na jednotlivých úlohách, původní odhad a skutečná reálná doba
- **Produktové metriky**
    - Hodnotia stav projektu
    - Monitorujú riziká
    - Odhaľujú problematické miesta
    - Upravenie workflow
    - Vyhodnocujú schopnosť tímu kontrolovať kvalitu
    - Zdrojový kód, dokumentace, cyklomatická složitost (počet cest programem), počty funkčních bodů
- **Metriky zdrojů** 
    - HW, lidé, čas, nemocnost, výkonnost


### Metriky založené na veľkosti kódu
- Veľkosť softwarového produktu
- Lines Of Code (LOC)
- 1000 Lines Of Code (KLOC)
- Náročnosť v človekomesiacoch (E/MM)
- Počet chýb/KLOC
- Cena/KLOC
- Počet stránok dokumentácie/KLOC 

### LOC metriky
- Ľahké na použitie
- Ľahké na porovnanie
- Je možné vypočítať LOC existujúcich systémov, ale sledovateľnosť nákladov a požiadavkov môže byť stratená
- Závislé na programátorovi a jazyku

### Funkčne orientované metriky
- Metriky na základe funkčných bodov (FP)
- Odvodené pomocou empirických (založené na skúsenostiach) vzťahov založených na spočítateľných vlastnostiach systému

#### Function Points (FP) (viac rozpísané v Odhadování úsilí)
- Počet vstupov
    - Rôzne vstupy od užívateľa
- Počet výstupov
    - Reporty, obrazovky, error hlášky, ...
- Počet otázok
    - Vstup, ktorý generuje nejaký výstup
- Počet súborov
    - Logické súbory (databáza)
- Počet externých rozhraní
    - Pripojenie na iné systémy

FP = celkový počet * (0.65 + 0.01*Sum(F<sub>i</sub>))
Celkový počet vynásobený váhou získanou pre haždú organizáciu na základe empirických dát
F<sub>i</sub> (i = 1 až 14) je hodnota na úpravu zložitosti

- **Funkční body produktu** - při vývoji aplikace “na zelené louce” jsou tyto body takové body, které zůstanou v aplikaci na konci vývoje
- **Funkční body projektu** - prošly týmu rukama, zaplatili jsme za ně, nemusí na konci vývoje zůstat (např. body vynaložené na vyzkoušení nějakého postupu a následné předělání zpět), musíme s nimi však nutně počítat

Využitie FP:
- Chyby/FP
- Cena/FP
- Počet stránok dokomentácie/FP
- FP za človekomesiac

### Halsteadovy metriky
Softwarová metrika výpočtu složitosti na základě statistické analýzy kódu. Používá tyto proměnné:
n1 - počet unikátních operátorů
n2 - počet unikátních operandů
N1 - celkový počet operátorů
N2 - celkový počet operandů
Pomocí nich podle specifických vzorečků definuje tyto metriky:
Length: N = N1 + N2
Vocabulary: n = n1 + n2
Estimated length: Ñ = n1 log2 n1 + n2 log2 n2
Purity ratio: PR = Ñ / N
Volume: V = N log2 n

### McCabeovy flow grafy
Jsou založeny na zobrazování kontrolních toků programu. Graf slouží k zobrazení kontrolního toku. Uzly představují úlohy zpracování. Hrany představují tok řízení mezi uzly.

![](https://i.imgur.com/giCOuJG.png)

### Cyklomatická složitost
*Kolik je možných průchodů grafem nebo kolik je tam nezávislých větví*. Funguje také jako indikátor spolehlivosti. Pokud V(G) je větší než 10 má velký chybový potenciál a zle se testuje. V(G) je v podstatě počet uzavřených oblastí v rovinném grafu.

Nutná dobrá dekompozice tj. složitost do 10. Čím více rozhodování tím složitější graf.

Množina nezávislých cest v grafu
- V(G) = E – N + 2
    - E - počet hran grafu
    - N - počet uzlů grafu
- V(G) = P + 1
    - P - počet predikátových uzlů

### Coupling
Coupling metriky sa snažia zistiť, ako sa chyba v jednej komponente odrazí na zvyšku systému
##### Datový a regulační tok
d<sub>i</sub> - input data parameters
c<sub>i</sub> - input control parameters
d<sub>o</sub> - output data parameters
c<sub>o</sub> - output control parameters
##### Globální
g<sub>d</sub> - global variables for data
g<sub>c</sub> - global variables for control
##### Environmentální
w - fan in - number of modules called
r - fan out - number modules that call module
##### Metriky
Mc = k/m, k = 1
m = d<sub>i</sub> + ac<sub>i</sub> + d<sub>o</sub> + bc<sub>o</sub> + g<sub>d</sub> + cg<sub>c</sub> + w + r
a, b, c, k can be adjusted based on actual data

### Důvody pro měření metrik
- plánování projektu (odhad nákladů, pracnosti, času)
- kontrola kvality produktu
- odhad produktivity
- zdokonalení práce (růst výkonnosti organizace)

Příkladem může být tzv. Halsteadtova metrika, která je založena na teorii informací.
Výsledkem výzkumu SW metrik jsou metodiky vývoje (SOA, OO, strukturované programování, znalosti a vlivu kvality specifikací atd.) a metodiky odhadu pracnosti a doby řešení COCOMO, funkční body.

### Použití SW metrik
- Výzkum: podklad pro hledání metod realizace softwarových produktů, které by přinesly podstatné zvýšení jeho kvality a snížení nákladů a doby vývoje a hlavně rozsahu prací při údržbě softwaru (výzkum metod a zákonitostí vývoje softwaru).
- Normy: základ pro stanovení technicko-ekonomických podkladů pro řízení prací při tvorbě softwaru (normy pracnosti, odhady takových metrik, jako je pracnost či doba řešení) a uzavírání smluv (cena, termíny), předpoklad CMM.
- Kontrola kvality: prostředek sledování spolehlivosti softwaru při provozu a podklad pro řídící zásahy během údržby,procesy zajišťující kvalitu.
- Operativa: prostředek sledování průběhu prací při vývoji (dodržování termínů, procento testovaných komponent, trendy počtů chyb, počty nově zanesených chyb, komponenty s největším počtem chyb, atd.).

### Potíže s metrikami
- rozptyl hodnot
- druh SW, obtížně splnitelné termíny realizace
- kvalita zúčastněných
- omezení SW a HW

## Refaktoring kódu
Refaktorování je disciplinovaný proces provádění změn v softwarovém systému takovým způsobem, že nemají vliv na vnější chování kódu, ale vylepšují jeho vnitřní strukturu s minimálním rizikem vnášení chyb. Při refaktorování se provádí malé až primitivní změny, ale celkový efekt je velký, a to v podobě čistšího, průhlednějšího a čitelnějšího kódu, kód se také lépe udržuje a rozšiřuje. Zlepšuje se také celková kvalita kódu a architektura, snižuje se počet chyb a tím i zvyšuje rychlost vývoje programu. Refaktorování pomáhá pochopit a více si ujasnit kód, což je vhodné zejména upravování zdrojového kódu po někom jiném.

Existuje vazba mezi refaktorováním a návrhovými vzory, a to taková, že vzory popisují definovaný cíl a naopak refaktorování popisuje způsob, jak se k tomuto cíli dostat.

### Kdy refaktorovat?
- pokud přidáváme funkcionalitu
- když potřebujeme opravovat chyby
- revize kódu
- důležitá součást iterativního vývoje (povinná)
- když kód „smrdí“

### „Bad smells“

- **Duplicitní kód** – pokud je v kódu na více místech stejná struktura
- **Dlouhá metoda** – záleží na každém, kolik řádků už je pro něj dlouhá metoda, pokud se taková objeví, většinou se v takové metodě řeší více problémů najednou a měla by být rozdělena na metody menší, které řeší právě jeden problém. Pak je kód i čitelnější.
- **Velká třída** – pokud se třída snaží dělat více věcí najednou, není to z pohledu objektově orientovaného programování dobře, jelikož každá třída by správně měla řešit právě jeden problém, tudíž řešením je rozdělit třídu na více tříd
- **Dlouhý seznam parametrů** – metody s dlouhým počtem parametrů jsou většinou nesrozumitelné, pokud tyto předávané parametry obsahuje nějaký objekt, je řešením předat jako parametr tento objekt
- **Příkaz switch** – měl by být řešen pomocí polymorfismu a vyčleněn do samostatné metody
- **Komentáře** – pokud má programátor tendenci komentovat uvnitř metody svůj kód, je většinou lepší tento kód vyčlenit do samostatné metody, a pomocí vhodného názvu této metody odpadne nutnost komentáře
- **Shotgun Surgery** - abychom udělali jednoduchou změnu v kódu, je nutné sahat na mnoho míst, indikátor toho, že máme špatný model, že třídy mají špatnou zodpovědnost
- **Middle Man** - zprostředkované volání objektu zbytečně přes prostředníka
- **Lazy Class** - prázdná skořápka, třída, která nic nedělá 
- **Spekulativní obecnost** - kód, který je v programu obsažen, aby sloužil někdy do budoucna

### Systémový re-engineering
Znovu napsání celé části systému bez účelu změnit její funkcionalitu. Aplikovatelné, když některé, ale ne všechny subsystémy vyššího systému vyžadují častou údržbu. Re-engineering se praktikuje až potom, co byl systém nějakou dobu udržován a jeho cena za údržbu stoupá. K reingeneeringu se používají automatitozovaná zařízení, aby se vytvořil nový systém, který by se lépe udržoval (i snížení ceny za údržbu).
- Reverzní engineering
- Vylepšení struktury programu
- Modularizace programu
- Re-engineering dat

<details>
  <summary>Techniky refaktoringu</summary>
  
  - Úpravy metod
    - nahradit algoritmus
    - nahradit dočasnou proměnnou dotazem (metodou, která spočítá její hodnotu)
    - nahradit metodu metodou objektu
    - odstranit přiřazení parametrům
    - přejmenovat metodu a přejmenovat položku – změna názvu na lepší a výstižnější
    - rozdělit dočasnou proměnnou
    - vložit metodu
    - vložit dočasnou proměnnou
    - vyjmout metodu – z dlouhé metody se vyjme část kódu, který je vložen do nové metody
    - zavést vysvětlující proměnnou
- Přesouvání prvků mezi objekty
    - odstranit prostředníka
    - přesunout metodu a přesunout položku – přesun do vhodné třídy
    - skrýt delegáta
    - vyjmout třídu – vyjme se část kódu třídy a vloží do třídy nové
    - vložit třídu
    - zavést cizí metodu
    - zavést místní rozšíření
- Organizace dat
    - nahradit datovou položku objektem
    - nahradit pole objektem
    - zapouzdřit soukromou položku – k přístupu k proměnné použít gettery a settery
    - změnit hodnotu na odkaz
    - změnit odkaz na hodnotu
    - zavést objekt null
    - zavést předpoklad
- Generalizace
    - nahradit dědičnost delegováním
    - nahradit delegování dědičností
    - přesunout metodu výš, přesunout položku výš – přesun do předka
    - přesunout metodu níž, přesunout položku níž – přesun do potomka
    - přesunout tělo konstruktoru výš – přesun do předka
    - vyjmout podtřídu
    - vyjmout rodičovskou třídu – vyjmutí předka
    - vyjmout rozhraní – vyjmutí rozhraní
    - vytvořit šablonovou metodu
    - zrušit hierarchii
- Zjednodušení volání metod
    - nahradit chybový kód výjimkou
    - nahradit konstruktor tovární metodou
    - nahradit parametr explicitními metodami
    - nahradit parametr metodou
    - nahradit výjimku testem
    - oddělit dotaz a modifikátor
    - odstranit parametr
    - odstranit přístupovou metodu pro zápis
    - parametrizovat metodu
    - přejmenovat metodu a přejmenovat položku – změna názvu na lepší a výstižnější
    - přidat parametr
    - skrýt metodu
    - zachovat celý objekt
    - zapouzdřit přetypování na potomka
    - zavést objekt pro parametry
- Velké programování
    - roztrhnout dědičnost
    - převést procedurální návrh do objektů
    - vyjmout hierarchii
    - oddělit datový model od prezentace
- Ostatní techniky
    - duplikovat sledovaná data
    - nahradit kód typu podtřídami
    - nahradit kód typu třídou
    - nahradit magické číslo symbolickou konstantou
    - nahradit podtřídu položkami
    - nahradit vnořenou podmínku varovnými klausulemi
    - nahradit podmínku polymorfismem
    - nahradit kód typu stavem nebo strategií
    - odstranit příznak
    - zachovat celý objekt
</details>

### 


## Odhadování úsilí
### Funkční body (FP) = normalizovaná metrika softwarového projektu
- Měří aplikační oblast, nezkoumá technickou oblast
- Měří aplikační funkce a data, neměří kód
##### Princip
- Předběžný odhad s použitím omezené informace
- Měří vstupy, výstupy, dotazy, vnitřní paměti, vnější paměti

Princip odhadu:
velikost projektu X složitost X rizikové faktory = odhad

##### Typy funkčních bodů
Funkční body vztažené k transakčním funkcím:
- Externí vstupy (EI - External Inputs)
- Externí výstupy (EO - External Outputs)
- Externí dotazy (EQ - External Enquiry)

Funkční body vztažené k datovým funkcím:
- Vnitřní logické soubory (ILF - Internal Logical Files)
- Soubory vnějšího rozhraní (EIF - External Interface Files)

### Interní logické soubory (ILF)
Každá velká logická skupina uživatelských dat nebo informací použitých pro řízení aplikace představuje jeden ILF. 

Zahrneme každý logický soubor, nebo v případě DB, každé logické seskupení dat z pohledu uživatele, které je vytvořeno, používáno, nebo udržováno aplikací.

Spíše než fyzické soubory započteme každé logické seskupení dat tak, jak je viděno z pohledu uživatele a jak je definováno při analýze požadavků nebo návrhu dat.

Nezapočteme soubory, které nejsou přístupné uživateli prostřednictvím vnějšího výstupu nebo dotazu a které nejsou nezávisle udržovány.

1. Logická entita nebo skupina entit z pohledu uživatele. (1 ILF)
2. Logický interní soubor generovaný nebo udržovaný aplikací. (1 ILF)
3. Uživatelem udržovaná tabulka(y) nebo soubor(y). (1 ILF)
4. Datový soubor nebo soubor s řídící informací, který aplikace použije při sekvenčním zpracování a údržbě. (1 ILF)
5. Atributová entita udržovaná pouze prostřednictvím hlavní entity. (0 ILF)
6. Asociativní entity vytvořené průnikem nebo spojením obsahující pouze klíčový atribut (0 ILF)
7. Přechodný nebo třídicí soubor (dočasný soubor) (0 ILF)
8. Soubor vytvořený proto, že byla použita určitá technologie (např. indexový soubor) (0 ILF)
9. Soubor s předlohou (vzorem), který aplikace pouze čte. (0 ILF, 1 EIF)

### Soubory externího rozhraní (EIF)
Započteme každou velkou logickou skupinu uživatelských dat nebo řídící informace používané aplikací.

Tato informace musí být udržována jinou aplikací. Zahrňte každý logický soubor nebo logickou skupinu dat z pohledu uživatele.

Započteme každou velkou logickou skupinu uživatelských dat nebo řídící informace, která je extrahována aplikací z jiné aplikace ve formě souboru externího rozhraní.

Extrakce nemá mít za následek změnu v některém z interních logických souborů. Pokud ano, pak započteme do EI místo do EIF.

1. Soubory nebo záznamy extrahované z jiné aplikace (použité pouze jako odkazy) (1 EIF)
2. Databáze čtená pomocí jiné aplikace (1 EIF)
3. Vnitřní logický soubor jiné aplikace použitý jako transakce (0 EIF, 1 EI)
4. Systém HELP, bezpečnostní soubor, chybový soubor čtený nebo odkazovaný aplikací, který pochází z jiné aplikace, která soubory udržuje (2 EIF)

### Externí vstupy (EI)
Započteme každá unikátní uživatelská data nebo zadání uživatelských povelů, která vstoupí přes externí rozhraní do aplikace a přidá, mění, ruší nebo jinak pozmění data (např. přiřazení, přemístění, ...) v interním logickém souboru.

Započteme také řídící informaci, která vstoupí přes aplikační hranici a zajistí soulad s funkcí specifikovanou uživatelem.

Externí vstup by měl být považován za unikátní, pokud logický návrh vyžaduje logiku zpracování odlišnou od ostatních externích vstupů.

1. Datová obrazovka s přidáním, změnou a rušením (3 EI)
2. Více obrazovek pohromadě zpracovaných jako jedna transakce (1 EI)
3. Dvě datové obrazovky s odlišným uspořádáním dat, ale se shodnou logikou zpracování (1 EI)
4. Dvě datové obrazovky se shodným formátem, ale s odlišnou logikou zpracování (2 EI)
5. Datová obrazovka s více unikátními funkcemi (1 EI za každou funkci)
6. Automatický vstup dat nebo transakcí z jiné aplikace (1 EI na každý typ transakce)
7. Vstup uživatelských povelů do aplikace (1 EI)
8. Vstupní formuláře (OCR) s jednou transakcí (1 EI)
9. Funkce úpravy dat, která následuje za dotazem (1 EI a 1 EQ)
10. Individuální výběry na obrazovce s menu (0 EI)
11. Oprava uživatelem udržované tabulky nebo souboru (1 EI)
12. Duplikát obrazovky, která již byla započtena jako vstup (0 EI)
13. Externí vstupy zavedené pouze kvůli technologii (0 EI)
14. Výběr položky ze seznamu (0 EI)

### Externí výstupy (EO)
Započteme každá unikátní uživatelská data nebo řídící data, která opouští externí hranici měřeného systému. 

Externí výstup je považován za unikátní, pokud má odlišná data, nebo pokud vnější návrh (jiná aplikace) vyžaduje odlišnou logiku zpracování oproti jiným externím výstupům.

Externí výstupy se často skládají z hlášení, výstupních souborů zasílaných jiné aplikaci nebo zpráv pro uživatele.

1. Výstup dat na obrazovku (1 EO)
2. Souhrnná zpráva - dávkové zpracování (1 EO)
3. Automatická data nebo transakce směrem k jiným aplikacím (1 EO)
4. Chybové zprávy vrácené jako výsledek vstupní transakce (0 EO)
5. Záložní soubory (0 EO)
6. Výstup na obrazovku a na tiskárnu (2 EO)
7. Výstupní soubory vytvořené z technických důvodů (0 EO)
8. Výstup sloupcového a zároveň koláčového grafu (2 EO)
9. Dotaz s vypočtenou informací (1 EO, 0 EQ)

### Externí dotazy (EQ)
Jako vnější dotaz započti každou unikátní vstupně/výstupní kombinaci, kde vstup je příčinou a generuje výstup.

Vnější dotaz je považován za unikátní, pokud se od ostatních dotazů odlišuje typem výstupních datových elementů, nebo pokud vyžaduje odlišnou logiku zpracování v porovnání s ostatními externími dotazy.

1. On-line vstup a on-line výstup beze změny v datových souborech (1 EQ)
2. Dotaz následovaný změnovým vstupem (1 EQ/1 EI)
3. Vstup a výstup na obrazovce s nápovědou (na dané úrovni) (1 EQ)
4. On-line vstup s bezprostředním tiskem dat beze změny dat (1 EQ)
5. Výběr ze seznamu nebo umístění s dynamickými daty (1 EQ)
6. Výběr ze seznamu nebo umístění se statickými daty (0 EQ)
7. Požadavek na zprávu obsahující neodvozená data (1 EQ)

### Výpočet funkčních bodů
**Před výpočtem musíme EI, EO, EQ, ILF, EIF roztřídit do skupin podle vah.**


| Váhy | nízká | průměrná | vysoká | celkem |
| -------- | -------- | -------- | -------- | -------- |
| EI   |  ___ x3+  | ___ x 4 +  | ___ x 6 = | ___ |
|EO  |   ___ x 4 + |___ x 5 + |___ x 7 = | ___ |
|EQ  |   ___ x 3 +| ___ x 4 +| ___ x 6 =| ___ |
|ILF  |   ___ x 7 +| ___ x 10 +| ___ x 15 =| ___ |
|EIF  |   ___ x 5 +| ___ x 7 +| ___ x 10 =| ___ |

Neupravené funkční body celkem ___

### Matice složitosti
- FTR = File Types (User Data Groups) Referenced
- DET = Data Element Type (Attribute)
- RET = Record Element Type (User View)

#### Matice složitosti vstupů (EI, EQ)
| FTRs | 1-4 DETs | 5-15 DETs | 16+DETs |
| -------- | -------- | -------- | -------- |
| 0-1 | nízká | nízká | průměrná |
| 2-3 | nízká | průměrná | vysoká |
| 4+ | průměrná | vysoká | vysoká |
#### Matice složitosti výstupů (EO, EQ)
Rovnaka ako Matice složitosti vstupů



#### Matice složitosti souborů (ILF, EIF)
| RETs | 1-19 DETs | 20-50 DETs | 51+ DETs |
| -------- | -------- | -------- | -------- |
| 1 | nízká | nízká | průměrná |
| 2-4 | nízká | průměrná | vysoká |
| 5+ | průměrná | vysoká | vysoká |

### Obecné charakteristiky systému
14 charakteristik hodnocených podle stupně vlivu na aplikaci
Každý faktor je hodnocený ve stupnici 0 – 5 takto:
- 0 = bez vlivu
- 1 = náhodný
- 2 = mírný
- 3 = průměrný
- 4 = významný
- 5 = podstatný

1. Vyžaduje systém spolehlivé zálohování a zotavení?
2. Jsou vyžadovány datové komunikace?
3. Existuje distribuované zpracování?
4. Je výkonnost kritická?
5. Poběží systém v stávajícím intenzivně využívaném operačním prostředí?
6. Systém požaduje on-line vstup dat?
7. Vyžaduje on-line vstup dat použití vstupní transakce přes více obrazovek nebo operací?
8. Jsou hlavní soubory opravovány on-line?
9. Jsou vstupy, výstupy, soubory a dotazy složité?
10. Je vnitřní zpracování složité?
11. Je kód navrhován s cílem znovupoužití?
12. Jsou konverze a instalace zahrnuty v návrhu?
13. Je systém navrhován pro násobné instalace u různých organizací?
14. Je aplikace navrhovaná tak, aby zajistila změny a snadné používání na straně uživatele?

### Počet funkčních bodů
Počet funkčních bodů = [0.65 + (0.01 x součet hodnocení charakteristik systému)] x [počet nepřizpůsobených funkčních bodů]

##### Nové a upravované projekty
![](https://i.imgur.com/3EE3zfz.png)

#### Postup výpočtu FP
1. Identifikujte a spočtěte ILF, EIF, EI , EO, EQ. Pro každou ILF a EIF identifikujte počet RET a počet DET. Pro každou EI, EO a EQ, identifikujte počet FTR a DET
2. S použitím matice složitosti spočtěte počet jednoduchých, průměrných a složitých položek EI, EO, EQ, ILF, EIF.
3. Spočtěte Počet neupravených funkčních bodů.
4. Určete hodnoty 14 charakteristik systému.
5. Sečtěte charakteristiky a určete Faktor technické složitosti systému.
6. Určete Počet upravených FP systému.

#### Odhady velikosti (Capers Jones)
1 Funkční bod = X příkazů
- 320 - základní asembler
- 213 - makro asembler
- 128 - C
- 107 - COBOL
- 107 - FORTRAN
- 80 - PL/I
- 71 - Ada 83
- 64 - C++
- 54 - Ada 95
- 32 - Visual BASIC
- 22 - Smalltalk
- 16 - PowerBuilder
- 13 - SQL

#### Další odhady
- FP<sup>1.15</sup> předpovídá přibližný počet stran papírové dokumentace SW projektu
- FP <sup>1.2</sup> předpovídá přibližný počet vytvořených testovacích případů
- FP <sup>1.25</sup> předpovídá přibližný chybový potenciál u nových SW projektů
- FP <sup>0.4</sup> předpovídá přibližný plán vývoje v kalendářních měsících
- FP / 150 předpovídá přibližný počet pracovníků potřebných pro řešení aplikace
- FP / 750 předpovídá přibližný počet pracovníků údržby, kteří budou udržovat aplikaci v aktuálně požadovaném stavu

##### Přibližné velikosti aplikací
- Vstup objednávky 1,250 FP
- Zpracování daňového přiznání 2,000 FP
- Účtování telefonních služeb 11,000 FP
- Rezervace letenek 25,000 FP
- OS Windows 95 85,000 FP
- Telefonní přepojovací systém 12,000 FP

## COCOMO (Constructive Cost Model)
- Cena vývoje aplikace přímo závisí na velikosti SW.
- Přesnost odhadu velikosti SW závisí na etapě vývoje.
    - V pozdějších etapách je odhad přesnější.
    - Přesnost odhadu se může lišit až čtyřikrát (4:1) oběma směry.

#### 3 úrovně detailu:
- **Základní model**: hrubý odhad E(KSLOC) a T(KSLOC) založen na odhadu KSLOC.
- **Střední model**: vliv jiných faktorů na E(KSLOC) a T(KSLOC).
- **Pokročilý model**: bere v úvahu vlivy vývojové etapy, ve které se projekt nachází.

#### 3 vývojové módy:
- **Organický mód** – jednodušší, dobře řešitelné projekty, zpravidla menšího rozsahu
- **Bezprostřední mód** – středně obtížné projekty
- **Vázaný mód** – rozsáhlé projekty s vysokými nároky na řízení

### Úsilí a čas
Výpočet E(KSLOC) a T(KSLOC):

E = a.(KSLOC)<sup>b</sup>
T = c.E<sup>d</sup>

a,b,c,d: parametry volené podle úrovně modelu a vývojového módu
- tabulky hodnot a,b,c,d pro všechny kombinace úrovně modelu/vývojové módy
    - základní model, bezprostřední mód:
a=3.0, b=1.12, c=2.5, d=0.35
    - střední model, vázaný mód:
a=2.8.Fc, b=1.2, c=2.5, d=0.32

Intervaly hodnot parametrů:
- a ∈ [2.4, 3.6] pro základní model
- a ∈ [2.8 F<sub>c</sub>, 3.2 F<sub>c</sub>] pro střední a pokročilý model
- b ∈ [1.05, 1.20 ]
- c = 2.5 ve všech případech
- d ∈ [0.32, 0.38 ]

V základním modelu mají všechny parametry konstantní hodnoty.
Korekční faktor **F<sub>c</sub>** je součinem hodnot 15 atributů (cost drivers) specifických pro vývojový proces.

Atributy, mohou nabývat 6 možných hodnot ve stupnici:
velmi nízký, nízký, normální, velký, velmi velký, extrémně velký

Atributy:
- atributy SW produktu
    - RELY - požadovaná spolehlivost (0.75 - 1.40) (velmi nízká: 0.75, extrémně velká: 1.40)
    - DATA - velikost databáze (0.94 - 1.16)
    - CPLX - složitost produktu (0.70 - 1.65)
- HW atributy
    - TIME - omezení času výpočtu (1.00 - 1.66)
    - STOR - využití paměti/disku (1.00 - 1.56)
    - VIRT - spolehlivost (zranitelnost) virtuálních strojů, tj. HW + DBMS + OS + … (0.87 - 1.30)
    - TURN - doba obrátky (0.87 - 1.15)
- atributy vývojového týmu
    - ACAP - schopnost analytická (1.46 - 0.71)
    - PCAP - schopnost programátorská (1.42 - 0.70)
    - AEXP - zkušenost s podobnými aplikacemi (1.29 - 0.82)
    - VEXP - zkušenost se specifickým „virtuálním strojem“ (1.21 - 0.90)
    - LEXP - zkušenost se specifickým programovacím jazykem (1.14 - 0.95)
- atributy projektu
    - MODP - použití moderních programovacích technik (1.24 - 0.82)
    - TOOL - použití SW nástrojů (1.24 - 0.83)
    - SCED - přesné plánování (1.23 - 1.10)


### Kroky při použití COCOMO
#### Určení nominálního úsilí E<sub>n</sub>
- definujte (odhadni) úroveň modelu a vývojový mód
- nastavte odpovídající hodnoty *a* a *b* podle tabulky
- vypočtěte E<sub>n</sub>
#### Určení korekčního faktoru F<sub>c</sub>
- na základní úrovni není třeba řešit
- určete popisné hodnoty pro každý z 15 atributů
- převeďte na numerické hodnoty podle tabulky
 ![](https://i.imgur.com/27JBE4A.png)

#### Určení aktuálního (zpřesněného) úsilí E
- na základní úrovni E = E<sub>n</sub>
- E [člověk-měsíc] = F<sub>c</sub> . E<sub>n</sub>
- F<sub>c</sub> vyjadřuje nárůst pracnosti E<sub>n</sub> podle vlivu a významu jednotlivých atributů vývojového procesu
#### Určení doby vývoje T a dalších faktorů relevantních pro projekt
- nastavte odpovídající hodnoty *c* a *d* podle tabulky
- T[měsíc] = c . E<sup>d</sup>
- COCOMO také umožňuje:
    - výpočet odhadovaných nákladů
    - rozložení práce a ceny v jednotlivých etapách řešení projektu
    - ...

### Původní COCOMO
Hodnoty a,b,c,d jsou shodné pro střední a pokročilou úroveň modelu
- pro střední úroveň se aplikuje výpočet na celý projekt
- pro pokročilou úroveň se výpočet aplikuje pro jednotlivé etapy životního cyklu

COCOMO lze také použít pro odhad nákladů při modifikaci existujících aplikací

ESLOC = ASLOC . (0,4 DM + 0,3 CM + 0,3 IM) / 100

ESLOC - ekvivalentní počet SLOC
ASLOC - odhadnutý počet modifikovaných SLOC
DM - procento modifikace v návrhu
CM - procento modifikace v kódu
IM - integrační úsilí (procento původní práce)

**Existují různé verze COCOMO pro různé účely a prostředí**

## COCOMO 2
- nové softwarové procesy
- nové jevy měření velikostí
- nové jevy znovupoužití software
- potřeba rozhodování na základě neúplné informace

3 různé modely
- **ACM (Aplication Composition Model)**
pro projekty s použitím moderních nástrojů a GUI
- **EDM (Early Design Model)**
pro hrubé odhady v úvodních etapách, kdy se architektura vyvíjí
- **PAM (Post Architecture Model)**
pro odhady poté, co byla specifikována architektura

#### Předběžný návrh a Post-architektura


Úsilí = (multiplikátory okolí)[velikost]<sup>(faktory procesu)</sup>
Plán = (multiplikátor)[Úsilí]<sup>(faktory procesu)</sup>
- Okolí: výrobek, platforma, lidé, faktory projektu
- Místo nasazení: nelineární znovupoužití a proměnlivost
- Proces: omezení, riziko/architektura, tým, faktory vyspělosti

### ED a PA modely
(ED-Early Design model, PA-Post-Arch model, PM - PersonMonth)

**Úsilí**
![](https://i.imgur.com/3yVzMoN.png)
- Velikost určena několika přístupy
    - KSLOC (tis.řádek zdroj. kódu)
    - UFP (neupravené fukční body)
    - EKSLOC (ekvivalentní velikost zdroj. kódu)
- SF: měřítkové faktory určené pomocí driverů exponentu
- EM: multiplikátory úsilí (7 pro ED, 17 PA)

### Nový přístup k měřítk. exponentu
![](https://i.imgur.com/a4r4kwr.png)

A v rozsahu 1.01 - 1.26
SF - upravený součet 5 driverů s hodnocením 0 – 5

Drivery exponentu
- návaznost na předchozí výsledky
- flexibilita vývoje
- rozhodnutí architektury/rizika
- koheze týmu
- vyspělost procesu (podle SEI CMM)

### Nové atributy ovlivňující EM
- RUSE - požadovaný stupeň znovupoužitelnosti
- DOCU - souběžná úprava dokumentace při vývoji
- RCPX - složitost a spolehlivost produktu
- VMVH - proměnlivost virtuálního stroje – host
- VMVT - proměnlivost virtuálního stroje – periferie
- PVOL - proměnlivost HW platformy
- PDIF - složitost HW platformy
- PERS - personální schopnosti
- PREX - personální zkušenosti
- PCON - personální kontinuita na projektu
- PEXP - zkušenost s platformou
- LTEX - zkušenosti s jazykem a nástroji
- SECU - bezpečnost
- SITE - vývoj ve více místech

Většina nových atributů vychází z kombinace dříve používaných atributů. Nové atributy mají 6 možných hodnocení, každému hodnocení odpovídá kladné číslo určené kalibrací z předchozích projektů

#### 2 společné vlastnosti C a C2
- Oba způsoby při odhadu ceny zahrnují jistou množinu faktorů, která ji ovlivňuje
- Oba využívají stejný druh modelů na rozlišení výpočtu
#### 3 rozdíly C a C2
- COCOMO 2 zahrnuje některé nové atributy na měření odhadu ceny, které vznikly kombinací předchozích z COCOMO.
- Modely v COCOMO 2 jsou na rozdíl od COCOMO zaměřené spíše na vývojovou etapu projektu
- Při odhadu nákladů na úpravu aplikace využívá COCOMO 2 i tzv. AA a SU koeficienty

### Rozšířené a upravené modely
ESLOC = ASLOC . (AA+SU+0,4 DM+0,3 CM+0,3 IM)/100
- ESLOC, ASLOC, DM, CM, IM - stejné jako dříve
- AA (Assessment and Assimilation) - práce potřebná pro určení, zda a v jakém rozsahu může být existující modul použit beze změn
- SU (pochopení SW) = čitelnost a „uchopení“

## Softwarová fyzika
N - délka programu (počet řádek, SLOC)
T - spotřeba práce (člověkoměsíce, MM)
P - produktivita P=N/T
D - doba realizace programu
S - průměrný počet řešitelů
#### Práce a délka programu
![](https://i.imgur.com/c5HeXPT.png)
#### Produktivita
![](https://i.imgur.com/nHJWCdB.png)
S rostoucí délkou programu klesá produktivita programátorů.
### Putnamova rovnice
![](https://i.imgur.com/uje6gTU.png)

Důsledky Putnamovy rovnice
- Programy psané ve spěchu jsou delší.
- Při zkrácení termínu na 83% je pracnost je dvojnásobná.

![](https://i.imgur.com/R0f5Xov.png)
![](https://i.imgur.com/ceHmHOd.png)

## Údržba a znovupoužitelnost
Údržba je spíše u zakázkového SW. Snaží se reagovat na chyby a přizpůsobovat se měnícímu se prostředí. Velmi nákladná v čase, finance odpovídají tomu jak dlouho ho chceme udržet. Náklady jsou 2x-100x větší než na vývoj. Na údržbu se mělo myslet již při vývoji.


- Oprava softwarových chyb
- Adaptace softwaru na jiné operační prostředí
- Přidat nebo měnit systémovou funkcionalitu → každá implementace degraduje kvalitu systému

#### Faktory ceny údržby
- Stabilita týmu
- Smluvní zodpovědnost
- Um zaměstanců
- Věk a struktura programu

#### Vývoj relativní ceny údržby v závislosti na kvalitě produktu
Cena se odvíjí od toho jak dlouho se to udržuje a kolik je provedeno zákroků do systému. Do ceny zahrnuje také incident managment, konzultace, změna/přidání funkcionality a školení.

![](https://i.imgur.com/ajxE8hM.png)

### Znovupoužitelnost
Hlavní výhodou je několikanásobné finanční ohodnocení jednou vyvinuté komponenty.
#### Úrovně znovupoužitelnosti (reuse levels)
- Abstrakce (The abstraction level): analytické prvky
- Objekty (The object level): třídy
- Komponenty (The component level): kolekce tříd
- Systém (The system level): celý systém a různé platformy

#### Reuse-Oriented software engineering
Model vývoje SW, založen na systematickém znovuužití, kde jsou systémy integrovány z existujících komponent (commercial-off-the-shelf = COTS)
- Zbylou funkcionalitu (kterou ještě nemáme) doprogramujme, především proxy, adaptéry a GUI.
- Jedná se o standardní budování business systémů.

### Lehmanovy „zákony“ (1980, 1985)
Zákony se zabývají fází evoluce, popisují rovnováhu mezi novými požadavky a údržbou na straně jedné a zvyšující se složitostí, snižující se “business value” na straně druhé.

- **Z. trvalé proměny**: Systém používaný v reálném prostředí se neustále mění, dokud není levnější systém restrukturalizovat, nebo nahradit zcela novou verzí.
- **Z. rostoucí složitosti**: Při evolučních změnách je program stále méně strukturovaný a vzrůstá jeho vnitřní složitost. Odstranění narůstající složitosti vyžaduje dodatečné úsilí.
- **Z. vývoje programu**: Rychlost změn globálních atributů systému se může jevit v omezeném časovém intervalu jako náhodná. V dlouhodobém pohledu se však jedná o seberegulující proces, který lze statisticky sledovat a předvídat.
- **Z. invariantní spotřeby práce**: Celkový pokrok při vývoji projektů je statisticky invariantní. Jinak řečeno, rychlost vývoje programu je přibližně konstantní a nekoreluje s vynaloženými prostředky.
- **Z. omezené velikosti přírůstku**: Systém určuje přípustnou velikost přírůstku v nových verzích. Pokud je limita překročena, objeví se závažné problémy týkající se kvality a použitelnosti systému. 

### Brooksův zákon
Přidání řešitelské kapacity u opožděného projektu může zvětšit jeho zpoždění. 
(Náklady na začlenění nového pracovníka do týmu jsou zpravidla větší než jeho přínos)


## Kvalita softwaru
**Každý program dělá něco správně; nemusí však dělat to, co chceme, aby dělal.**

**Kvalita**: Dodržení explicitně stanovených funkčních a výkonových požadavků, dodržení explicitně dokumentovaných vývojových standardů a implicitních charakteristik, které jsou očekávány u profesionálně vyrobeného software.

**Aspekty kvality**:
- odchylky od požadavků na software
- nedodržení standardů
- odchylky od běžných zvyklostí (implicitních požadavků)

### Spojité chápání kvality
![](https://i.imgur.com/286zYCj.png)

### Kvalita - IEEE Std. 610.12-1990
Stupeň, do jaké míry systém, komponenta nebo proces splňuje *specifikované požadavky*.

Stupeň, do jaké míry systém, komponenta nebo proces splňuje *zákazníkovy nebo uživatelovy potřeby nebo jeho očekávání*.

### Faktory kvality software
- Přímo měřitelné faktory
    - #chyb/KLOC/čas
- Pouze nepřímo měřitelné faktory
    - použitelnost, udržovatelnost
- Kategorie faktorů kvality:
    - operační charakteristiky
    - schopnost akceptovat změny
    - adaptibilita na nové prostředí

### Faktory kvality - McCall et al. (1977)
- **Korektnost**: Rozsah toho, jak program splňuje specifikaci splňuje uživatelovy záměry.
- **Spolehlivost**: V jakém rozsahu lze očekávat, že program bude plnit zamýšlené funkce s požadovanou přesností.
- **Efektivita**: Množství výpočetních prostředků a kódu, které program potřebuje na splnění svých funkcí.
- **Integrita**: V jakém rozsahu mohou být program nebo data používána neoprávněnými osobami.
- **Použitelnost**: Úsilí vyžadované na učení, operování, přípravu vstupu a interpretaci výstupu programu.
- **Udržovatelnost**: Úsilí vyžadované na vyhledání a opravu chyby v programu.
- **Flexibilita**: Úsilí vyžadované na modifikaci provozovaného programu.
- **Testovatelnost**: Úsilí potřebné na testování programu tak, abychom se ujistili, že plní zamýšlené funkce.
- **Přenositelnost**: Úsilí potřebné na přemístění programu na jiný HW/SW.
- **Znovupoužitelnost**: Rozsah, v jakém lze program nebo jeho části znovu použít v jiné aplikaci (funkce a balení produktu).
- **Schopnost spolupráce**: Úsilí, které je nutné vynaložit pro připojení daného systému k jinému.

![](https://i.imgur.com/fUD8vDV.png)
![](https://i.imgur.com/F1D4qBZ.png)

### Globální hodnocení kvality výroby
**Vyspělost organizace**: model CMM
**Systémy kvality**: norma ISO 9001
**Ocenění kvality**: cena MBNQA

#### CMM - Capability Maturity Model
Hodnotí vyspělost organizací podle stupně a kvality využívání SW procesů.

##### Úroveň 1: Výchozí
Chaotický proces, nepředvídatelná cena, plán a kvalita.

##### Úroveň 2: Opakovatelný
Intuitivní; cena a kvalita jsou vysoce proměnlivé, plán je pod vědomou kontrolou, neformální metody a procedury.
Klíčové prvky:
- řízené požadavky
- plánování softwarového projektu
- řízené subkontrakty na software
- zajištění kvality software
- řízení softwarových konfigurací

##### Úroveň 3: Definovaný
Orientován na kvalitu; spolehlivé ceny a plány, zlepšující se, ale dosud nepředvídatelný přínos (výkon) systému kvality.
Klíčové prvky:
- zlepšování organizačního procesu
- definice organizačního procesu
- školicí program
- řízení integrovaného software
- aplikace inženýrských metod u softwarového produktu
- koordinace mezi pracovními skupinami
- detailní prověrky a oponentury

##### Úroveň 4: Řízený
Kvantitativní; promyšlená statisticky řízená kvalita produktu.
Klíčové prvky:
- měření a kvantitativní řízení procesu výroby
- řízení kvality

##### Úroveň 5: Optimalizující
Kvantitativní základ pro kontinuální investice směřující k automatizaci a zlepšení výrobního procesu.
Klíčové prvky:
- prevence chyb
- inovace technologie
- řízené změny výrobních procesů

![](https://i.imgur.com/BXuJHVv.png)

### Principy systémů SQA (Software Quality Assurance)
- Definovaná a dokumentovaná politika kvality a manažerský podíl
- Definice zodpovědností, autorit a vztahů mezi všemi osobami, které svojí prací mohou ovlivnit kvalitu
- Dokumentované postupy a instrukce pro kvalitu
- Efektivní implementace dokumentovaného systému kvality na všech úrovních organizace
- Záznam všech aktivit SQA

### Standardy ISO 900x

- **ISO 9001: 1994**
    - Systémy kvality - model zajištění kvality při návrhu, vývoji, výrobě, instalaci a servisu
- **ISO 9000 - 3: 1991**
    - Doporučení, jak aplikovat ISO 9001 při vývoji SW
- **ISO 9004 - 2: 1994**
    - Řízení kvality a prvky systému kvality - doporučení

#### ISO 9001 - Systémy kvality
1. Zodpovědnost vedení
2. Systém kvality
3. Přehled zakázek
4. Řízení návrhu
5. Řízení dokumentace
6. Nakupování
7. Zakoupené produkty
8. Identifikace a sledování produktu
9. Řízení procesu
10. Inspekce a testování
11. Inspekční, měřicí a testovací vybavení
12. Stav inspekce a testování
13. Zvládnutí nevyhovujícího produktu
14. Opravné akce
15. Manipulace, skladování, balení a doručení
16. Záznamy o kvalitě
17. Vnitřní prověrky kvality
18. Školení
19. Služby
20. Statistické techniky

#### Vztah mezi MBNQA a ISO 9001
![](https://i.imgur.com/hEM3hdN.png)

#### Jak začít SQA?
1. Formulace hypotézy
2. Pečlivý výběr vhodných metrik
3. Sběr dat
4. Interpretace dat
5. Iniciace akcí vedoucích ke zdokonalení
6. Iterace s vyhodnocením vlivu přijatých opatření, formulace dalších hypotéz

### Přínos SQA
| Etapa | Cena nalezení a opravy |
| ----- | ----- |
| Požadavky | 0.75 |
| Návrh | 1.0 |
| Kódování | 1.5 |
| Testování | 3.0 |
| Systémové testy | 10.0 |
| Provoz | 60-100.0 |
Pozn.: Cena normalizovaná vzhledem k ceně v etapě návrhu

### Efektivita přezkoušení

![](https://i.imgur.com/VDg0MtP.png)

### Různé „review“ techniky
| TYP METODY | TYPICKÉ CÍLE | TYPICKÉ VLASTNOSTI |
| ----- | ----- | ----- |
| **Prohlídky** |Minimální náročnost<br/>Školení vývojářů<br/>Krátká doba | Malá/žádná příprava<br/>Neformální proces<br/>Žádné měření<br/>Žádné FTR (FormalTechnical Review) |
| **Odborné recenze** | Zjištění požadavků<br/>Rozlišení nejednoznačností<br/>Školení | Formální proces<br/>Představení autora<br/>Rozsáhlá diskuze |
| **Inspekce** | Účinné a efektivní zjištění a odstranění všech defektů | Formální proces<br/>Kontrolní seznam<br/>Měření<br/>Fáze přezkoušení |

| | INSPEKCE, RECENZE | PROHLÍDKA |
| ----- | ----- | ----- |
| **Požadavky** | Výchozí požadavky | Detailní požadavky |
| **Plány** | Plány vývoje | |
| **Vývoj** | Návrh podrobného kódu | Návrh systému |
| **Publikace** | | Pracovní & finální publikace |
| **Testování** | | Implementace testu |

### Cíle formálního přezkoušení

- Odhalit chyby ve funkci, logice a implementaci software.
- Ověřit, že zkoumaná položka splňuje požadavky (odpovídá požadavkům).
- Zajistit, že položka byla prezentována s použitím předdefinovaných standardů.
- Zajistit jednotný vývoj.
- Zvýšit řiditelnost projektů.

### Závažnost chyb, defektů
- Kritické
    - Defekty, které mohou způsobit pád systému, vznik chybných výstupů či chování nebo narušit uživatelská data. Není známa cesta, jak se těmto defektům vyhnout.
- Vážné 
    - Defekty, které způsobují chybné výstupy či chování a je známa cesta, jak se těmto defektům vyhnout. Zasažena je významná část systému.
- Středně závažné
    - Defekty ovlivňující omezenou část funkcionality, které je možné se vyhnout nebo ji ignorovat.
- Málo závažné
    - Defekty, které mohou být opomenuty bez narušení funkčnosti

### Indikátory kvalitních inspekcí jsou:
- Produkty jsou prověřovány až v době, kdy na to jsou připraveny.
- Termíny schůzek jsou přísné, ale zvládnutelné.
- Komentář autora je zařazen jen pokud je užitečný.
- Kontrolní seznamy a související materiály jsou užitečné.
- Schůzka recenze se zaměřuje na detekci problémů.
- Autor se nesmí cítit ohrožen.
- Úpravy jsou pečlivě prověřeny.
- Jsou odhaleny cesty na zlepšení inspekcí a vývojového procesu.
- Účastníci považují metody za způsob efektivního zvýšení kvality.
- Každý se chce účastnit znovu!

### Chyby

#### Názvoslovie
**Porucha** je neschopnost systému nebo systémové komponenty provádět požadovanou funkci ve specifikovaných hranicích. Porucha může nastat, když se narazí na chybu, jejímž výsledkem je ztráta očekávané uživatelské služby.

**Fault** je chyba (defekt) v kódu, která může být příčinou jednoho nebo více selhání případně náhodná podmínka, která způsobuje, že funkční jednotka selhává při plnění požadované funkce (bug).

**Error** je chyba (omyl), kdy nesprávná nebo chybějící akce uživatele zapříčiní chybu (defekt) v programu.

- Čím později v životním cyklu detekujeme chybu, tím nákladnější bude její oprava.
- Mnoho chyb zůstane skryto a je odhaleno až po ukončení fáze, v níž byly udělány.
- V požadavcích je mnoho chyb.
- Chyby v požadavcích jsou především chybná fakta, opomenutí, rozpory a nejednoznačnosti.
- Chyby v požadavcích lze detekovat.

#### Chyby a opotřebení HW
- Na začátku je nový HW dostatečně výkonný, ale má poměrně dost chyb, které se ale zpravidla podaří časem odstranit.
- Na konci se začne projevovat opotřebení a HW začne zaostávat za svým výkonnějším okolím. Je třeba ho nahradit

#### Chyby a opotřebení SW
Je naivní si myslet, že s postupem času odstraníte v SW všechny chyby a zmizí tak veškeré problémy

Realita je taková, že zákazník požaduje během provozu nové a nové úpravy, což dělá systém složitějším zanáší do systému další chyby. Jednou přijde den, kdy bude lepší to celé naprogramovat znovu. (Lehmanovy zákony)

![](https://i.imgur.com/CNqixOm.png)

#### IBM ortogonální klasifikace defektů (ODC)
- **funkce** – chyba ovlivňující schopnosti, rozhraní uživatelů, rozhraní výrobku, rozhraní s HW architekturou nebo globální datovou strukturou.
- **rozhraní** – chyba při interakci s ostatními komponentami nebo ovladači přes volání, makra, řídící bloky nebo seznamy parametrů.
- **ověřování** – chyba v logice programu, která selže při validaci dat a hodnot před tím, než jsou použity.
- **přiřazení** – chyba při inicializaci datové struktury nebo bloku kódu.
- **časování/serializace** – chyba, která zahrnuje časování sdílených a RT prostředků.
- **sestavení/balení/spojování** – chyba související s problémy s repozitory projektu, změnami vedení, nebo správou verzí.
- **dokumentace** – chyba, která ovlivňuje publikace a návody pro údržbu.
- **algoritmus** – chyba, která se týká efektivity nebo správnosti algoritmu nebo datové struktury, ne však jejich návrhu.

