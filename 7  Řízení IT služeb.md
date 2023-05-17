# 7  Řízení IT služeb

###### tags: `řsss-základ`, `it-services-management`, `management`

> _Řízení IT služeb. Princip, procesy, outsourcing. Information Technology Infrastructure Library (ITIL), základní koncepty, řízení infrastruktury služeb. (PV203, PV214)_

## Princip, procesy, outsourcing

### Princip

Riadenie IT služieb (IT Services Management, ITSM) je strategický prístup k riadeniu informačných technológií a poskytovaniu služieb zákazníkom. Pokrýva IT služby, procesy, technológie a praktiky riadenia personálu, ktoré prispievajú k riadeniu infraštruktúry. Jedná sa o všeobecný pojem, ktorý má svoje frameworky. Môže byť taktiež v skratke definovaný ako to, čo robíme pre riadenie služieb poskytovaných zákazníkom.

Príklady ITSM v praxi:
* riešenie incidentov
* najímanie profesionálov
* vzdelávanie zamestnancov
* riešenie IT bezpečnosti

**Služba** je spôsob doručenia hodnoty zákazníkovi. Hodnota predstavuje dosiahnutie želaných výsledkov bez toho, aby musel zákazník niesť špecifické náklady a riziká.

**Manažment služieb** je množina špecializovaných organizačných oblastí pre doručenie hodnoty zákazníkovi vo forme služieb. Medzi tieto oblasti patria:
* Aktivity - stav, v ktorom sa veci dejú alebo sú vykonávané
* Funkcie - tím alebo skupina ľudí a nástroje používané k vypracovaniu procesu alebo činnosti.
* Procesy - súbor akcií vykonávaných za účelom dosiahnutia nejakého výsledku. 
* Role - súbor povinností a právomocí udelených osobe alebo tímu.

Cieľom ITSM je zaistiť, že _správne procesy, ľudia a technológie sú využité tak, aby firma mohla dosiahnuť svoje obchodné ciele_. Prínosy ITSM sú:
* Porozumenie službe
* Overenie výsledkov služby
* Porozumenie významu služby
* Pochopenie a riadenie nákladov a rizík

ITMS potrebuje stabilný framework (súbor dobrých praktík) pre kontinuálne poskytovanie kvalitných služieb, dosahovanie zlepšenia procesov a redukovanie nákladov a rizík. Najznámejšími frameworkmi sú:
* **ITIL** (Information Technology Infrastructure Library) - preberaný detailne neskôr.
* **COBIT** (Control Objectives for Information and Related Technologies), ktorý špecifikuje dobré praktiky pre riadenie IT procesov.
* **Microsoft Operations Framework** (MOF) - alternatíva k ITIL. Poskytuje inštrukcie k celému životnému cyklu služby.
* **ISO 20000** - medzinárodný štandard ITSM. Dáva inštrukcie k tomu, *čo robiť*, zatiaľ čo ITIL hovorí o tom, *ako to robiť*.

ITSM ako manažérska disciplína pozostáva z troch oblastí:
* Ľudia
* Nástroje
* Procesy

Jedným zo spôsobov, ako je možné vyhodnotiť úroveň riadenia služieb vo firme, je **Gartnerov I&O Maturity Model**. Zohľadňuje ľudí, procesy, technológie, obchodný management a predstavuje spôsoby zvýšenia úrovne vyspelosti. Tieto faktory tvoria tzv. _obchodnú hodnotu_, ktorá zahŕňa kvalitu, agilitu, ekonomické faktory (cost-efficiency), spokojnosť zákazníka a obchodný prínos. Model obsahuje celkovo 6 úrovní:
1. Level 0 - **Survival** - minimálne alebo žiadne zameranie na IT infraštruktúru a operácie (I&O).
2. Level 1 - **Awareness** - uvedomenie si, že I&O sú extrémne dôležité pre firmu. Začínajú sa prijímať opatrenia pre získanie operačnej kontroly a prehľadnosti.
3. Level 2 - **Committed** -  presun do riadeného prostredia (napr. procesy IT podpory na dennej báze) a zvýšenie úspešnosti v projektovom riadení tým, že sa firma zamerá na zákazníka a splnenie jeho predstáv.
4. Level 3 - **Proactive** - firma sa stáva efektívnou a zvyšuje kvalitu služieb cez štandardizáciu, vývoj interných politík, štruktúr riadenia a implementáciou proaktívnych procesov naprieč oddeleniami.
5. Level 4 - **Service-aligned** - riadi IT ako business. Firma je zameraná na zákazníka a je skúsený poskytovateľ IT služieb s preukázateľnými výsledkami.
6. Level 5 - **Business partnership** - dôveryhodný partner pre zvyšovanie hodnoty a kompetitívnosti obchodných procesov a businessu ako takého.

Alternatívnou k Gartnerovmu I&O Maturity Modelu je *Capability maturity model* (preberaný v otázke *Softwarové inženýrství*).

### Procesy

Proces je súbor akcií, ktoré sú vykonávané za účelom dosiahnutia _konkrétneho výsledku_ a _poskytovania hodnoty zákazníkom_. Každý proces reaguje na udalosti a má merateľný a špecifický výstup. V prípade, že nie je dostatok zdrojov pre dokončenie procesu, hodnota nebude doručená.

Servisný model popisuje ako poskytovateľ služby vytvára hodnotu pre zákazníka. Popisuje _štruktúru_ (jednotlivé prvky potrebné potrebné pre doručenie služby a ich konfiguráciu) a _dynamiku_ (aktivity, tok zdrojov, koordináciu a interakcie medzi zákazníkom a prvkami v štruktúre). Servisný model zvykne zahŕňať procesné mapy, diagramy workflow, a activity patterns.

Veľmi dôležitým nástrojom používaným v ITSM je **RACI** matica (Responsible, Accountable, Consulted, Informed). Pomáha riadiť zdroje a role pre vykonanie úlohy tým, že zaraďuje ľudí s rôznymi zodpovednosťami do procesu a dokumentuje vzťahy v procese. Tým umožňuje odstrániť nedorozumenia plynúce z nejasne pridelených kompetencií. RACI matica definuje nasledujúce vzťahy:
* Len jedna osoba môže máť autoritu nad celým procesom (_accountable_), no nemusí sa priamo podieľať na jej vykonávaní.
* Ľubovoľný počet ľudí môže byť _zodpovedný_ (responsible) za vykonanie jednotlivých úloh. O priebehu a výsledkoch svojej práce informujú accountable osobu.
* K splneniu úlohy sú niekedy potrebné konzultácie. Zamestnanci sa môžu radiť s osobami, ktoré majú potrebné znalosti a zručnosti, no taktiež môžu využiť uložené dokumenty alebo aj internetový search engine. Tieto _konzultované_ (consulted) zdroje potrebujú byť evidované, aby bolo možné overiť ich dostupnosť.
* Iné zdroje potrebujú byť _informované_ (informed). Obvykle sa jedná o stakeholderov, ktorí potrebujú sledovať postup vypracúvania úloh, alebo potrebujú výstup danej úlohy. Často sa do tejto skupiny radia firemní sponzori.

![](https://i.imgur.com/eULnboX.png)


### Outsourcing

Outsourcing (odvodené z _outside resource using_) predstavuje odovzdanie vnútropodnikových aktivít zvyčajne nesúvisiacich s hlavnou činnosťou podniku na externý subjekt (napr. na subdodávateľa). Jedná sa o zmluvný vzťah prenášajúci zodpovednosť za nejakú funkčnú oblasť na externé zdroje. 

Rozdiely medzi insourcingom (vývojom vlastných služieb) a outsourcingom:
* Insourcing je obvykle nákladnejší, keďže firma potrebuje založiť nové oddelenie a implementovať nové procesy. Pri outsourcingu sa o tieto veci stará poskytovateľ služby.
* Outsourcing využíva zdroje inej firmy, čo firme umožňuje sa zamerať čiste na jej hlavný predmet podnikania. To vedie k vyššej produktivite.
* V outsourcingu nesie zodpovednosť za riadenie služby externá firma. Zároveň má klient minimálnu kontrolu nad použitými manažérskymi metódami použitými pri vývoji.
* Insourcing je obvykle on-site, zatiaľ čo outsourcing je väčšinou mimo sídla spoločnosti, často v inom meste alebo inej krajine.

Dôvody pre využitie outsourcingu:
* _Nižšie náklady_
* _Umožnenie zamerania sa na hlavnú činnosť podniku_
* Prístup k novým znalostiam
* Prístup k novým technológiám
* Flexibilita
* Presun zodpovednosti

#### Modely doručenia IT služieb

**Rozšírenie personálu** (staff augmentation) umožňuje prístup k špecializovaným zdrojom, nákladovú flexibilitu a spĺňa krátkodobé time-to-market požiadavky. Týmto modelom môže spoločnosť rozšíriť existujúce tímy o dodatočných pracovníkov s požadovanými znalosťami. Typickou motiváciou pre voľbu tohto modelu je minimalizácia nákladov.

Obvykle vyžaduje minimálne zmluvné viazania, náklady sa zväčšia odvíjajú od počtu odpracovaných hodín, model je ľahko škálovateľný a má nízky vplyv na už existujúci operačný model IT funkcií v spoločnosti.

Rozsah povinností je zväčša malý - obvykle zahŕňa prototypovanie, implementáciu a testovanie. Vízia pre produkt a riadiace funkcie najatých pracovníkov sú limitované, pretože ich riadi klient, ktorý si ich najal.

Výhodou modelu je, že v krátkom čase umožňuje prístup k znalostiam, ktoré v spoločnosti chýbajú bez nákladov spojených s prijímaním stálych zamestnancov a prepúšťaním. Zároveň umožňuje firme flexibilne reagovať na neočakávané udalosti.

Na druhej strane nie je vhodným dlhodobým riešením, pretože náklady by mohli prerásť tie, ktoré by plynuli z modelu riadených služieb.

**Out-tasking** je vhodný pre krátkodobé obchodné potreby ako je napríklad doplnenie chýbajúcich zručností. Problémom pri tomto modeli býva integrácia výsledkov viacerých out-taskingov.

**Projektový outsourcing** (project-based outsourcing) umožňuje poskytovateľovi služby a klientovi zdieľanie rizík a tržieb. Veľkou výhodou pre klienta je, že poskytovateľ služby je zodpovedný za celý projekt a zároveň model umožňuje aplikovovať best practices v procese outsourcingu.

Nevýhodou však je, že outsourcing je plánovaný v samostatných fázach. Viac konsolidovaný prístup môže byť dosiahnutý modelom riadených služieb, ktorý je založený na dlhodobej spolupráci.

**Model riadených služieb** (managed services model) predstavuje dlhodobú spoluprácu založenú na service-level agreemente. Poskytovateľ služby prijíma zodpovednosť za výsledky stanovené v zmluve. Projekty majú väčšinou veľký rozsah a získané znalosti poskytovateľ služby využíva pri ďalšom vývoji systému, čo postupom času poskytuje klientovi väčšie výhody.

Základom modelu je detailné plánovanie, v ktorom musí klient jasne určiť požiadavky na výsledky projektu a kľúčové indikátory výkonnosti (key performance indicators - KPI). Cieľom poskytovateľa služby je dosiahnuť výsledky spĺňajúce klientove predstavy a cena služby závisí na týchto výsledkoch.

Spolupráce založené na tomto modeli umožňujú zdieľanie rizík a tržieb. Klient takto znižuje svoje náklady, keďže poskytovateľ služby akceptuje riziká a preberá kontrolu nad riadením a vykonaním projektu. Vyúčtovania prebiehajú mesačne s tým, že je garantovaná úroveň služieb. To zase umožňuje obom stranám presnejšie odhadnúť a riadiť rozpočet celého projektu.

Obsahuje tieto kroky:
1. **Riadenie príležitostí** - aké služby predávame? Čo typický zákazník chce a potrebuje?
2. **Návrh riešenia a ponuka** - ako je riešenie navrhnuté?
3. **Uzatvorenie predaja** - aké sú hlavné príčiny nákladov?
4. **Prechod a transformácia** - kto a kde doručuje službu? Ako vytvoríme a využijeme riešenie? Aké procesy a pracovné aktivity využívame?
5. **Ustálené operácie** (steady state operations) - ako plníme zmluvne určené služby? Ako zlepšíme naše existujúce služby?

V tomto modeli sa vyskytujú tri "páky" pre zvýšenie kvality a produktivity:
* _Štandardizácia_ zavádza štandardné riešenia pre všetky služby, čím maximalizuje úspory z rozsahu a zjednodušuje celý proces tým, že odstraňuje kroky, ktoré nezvyšuju hodnotu služby.
* _Automatizácia_ vedie k odstráneniu manuálnych úloh, čím sa znižuje chybovosť a zvyšuje sa kvalita.
* _Globalizácia_ vedie k využitiu pracovníkov z celého sveta, čo umožňuje prístup k znalostiam za optimálnu cenu. Umožňuje ľahšie škálovanie vďaka väčšiemu množstvu potenciálnych pracovníkov.

**Service-level agreement** (SLA) je dokument špecifikujúci úroveň služieb, ktorú klient očakáva od poskytovateľa. Špecifikuje metriky, pomocou ktorých je služby možné merať, a určuje penále pre prípad, ak služby dohodnutú úroveň nedosiahnu. Dokument taktiež jasne vymedzuje povinnosti oboch strán a penále, ak ich jedna zo strán nedodrží.

Príkladom špecifikovanej úrovne služieb môže byť dostupnosť serveru 99,9999 % času za rok. Ak poskytovateľ túto dostupnosť nedodrží, klient zaplatí len 90 % z pôvodne dohodnutej čiastky.

SLA obsahuje komponenty z dvoch oblastí:
* **služby** - obsahuje špecifiká poskytovaných oblastí, podmienky dostupnosti služby, štandardy, povinnosti oboch strán.
* **management** - zahŕňa definície štandardov merania a metód, proces reportovania, proces vyriešenia sporov, právne klauzuly a mechanizmy pre aktualizáciu SLA. Tieto mechanizmy sú extrémne dôležité, pretože požiadavky a možnosti poskytovateľa sa v priebehu projektu budú meniť a je potrebné upraviť SLA podľa týchto skutočností.

Časté metriky, ktoré SLA definuje, sú:
* Dostupnosť služby (service availability), ktorá zvykne byť meraná v % za určité časové obdobie.
* Frekvencia chýb reprezentujúca neúplné zálohy, chyby v kóde a nedodržané deadliny.
* Technická kvalita, ktorá zohľadňuje veľkosť programu a chyby v programe.
* Bezpečnosť programu

## Information Technology Infrastructure Library (ITIL)

### Základné koncepty

ITIL predstavuje best practices v ITSM a poskytuje firmám v rôznych odvetviach špecifické návody pre riadenie služieb. Tvorí ho 5 kníh, ktoré sa snažia o integráciu businessu s IT.

* Stáva sa medzinárodným štandardom.
* Firma si ho osvojuje a prispôsobuje ho firemným požiadavkám (adopt & adapt).
* Pomocou neho sa prepája business a IT.
* Robí procesy konzistentné.

Hlavné výhody ITILu sú:
* Môže byť osvojený a prispôsobený. Firma si osvojí ITIL procesy a praktiky, ktoré si neskôr môže prispôsobiť podľa svojich podmienok.
* Zvyšuje efektivitu vo firme.
* Spĺňa predstavy zákazníkov tým, že zlepšuje organizačné schopnosti poskytovateľa, čo vedie k službám odpovedajúcim zákazníkovým potrebám.
* Je škálovateľný - nezáleží, či má IT oddelenie 6 alebo 600 zamestnancov.

Využitie ITIL vedie k vyššej kvalite, nižším nákladom a lepšiemu prepojeniu IT s business. ITIL je dôležitý najmä kvôli týmto faktorom:
* Znižuje narušovanie IT služieb.
* Umožňuje väčšiu kontrolu nad IT infraštruktúrou a jej zmenami.
* Znižuje náklady na IT prostredníctvom centralizovania a štandardizovania služieb.
* Prepája IT infraštruktúru s businessom tak, že investície do IT sú zamerané na najvyššie priority firmy.
* Poskytuje jeden kontaktný bod pre koncových užívateľov v prípade incidentov, dotazov a informácií (namiesto viacerých helpdeskov existuje jeden).
* End-to-end integrácia procesov riadenia IT.

ITIL je tvorený štyrmi hlavnými prvkami:
* **Životný cyklus služby** - život služby od jej vzniku, cez vývoj projektu a nasadeniu do bežného provozu. 
* **Procesy** - množina postupov ako vykonávať činnosti
* **Funkcie** - zdroje ľudí vykonávajúcich činnosti nutné k riadeniu IT služieb
* **Role** - množina povinností alokovaných ľuďom alebo oddeleniam

Okrem toho ITIL delí poskytovateľov IT služieb do troch kategórií:
1. **Typ I - interný poskytovateľ služby**. Jedná sa o interné oddelenie, ktoré slúži jednej firme.
2. **Typ II - zdieľaná servisná jednotka** (shared services unit). Jedna interná IT organizácia alebo oddelenie, ktoré poskytuje služby viacerým firmám.
3. **Typ III - externý poskytovateľ služieb**. Organizácia poskytujúca služby externým zákazníkom. Jedná sa o klasické podnikanie.

V ITILe je taktiež potrebné sa zameriať na to, ako firma zvláda komunikáciu so zákazníkom a doručovanie hodnoty. Ak napríklad zákazník odchádza nespokojný, zmätený alebo s pocitom, že nebol vypočutý, poskytovateľ služby nedoručuje hodnotu. Preto je potrebné tento proces pre zákazníka čím viac zjednodušiť. Typickými "chvíľami pravdy" v IT, keď firma zistí, ako dobre dokáže doručiť hodnotu, sú:
* **Zákazník kontaktuje poskytovateľa, keď nastane nejaká chyba**. Môže sa jednať o pokazený PC, zlyhania siete, alebo čokoľvek iné spojené s IT. Je nutné zohľadniť, koho každého musí zákazník v kontaktovať a ako dlho potrvá, kým sa chyba opraví.
* **Štandardná požiadavka**. Napríklad nový zamestnanec potrebuje pracovný počítač alebo mobil. Ako rýchlo dokáže byť táto požiadavka splnená?
* **Nová obchodná požiadavka**. Ako efektívne a presne dokáže firma zachytiť nové požiadavky zákazníkov? Ako rýchlo vie doručiť službu spĺňajúcu tieto požiadavky?
* **Zmena stratégie** alebo zmena služby, prípadne aj nová služba. Ako vie firma zareagovať?
* **Operačná služba**. Zakaždým, by malo byť prihlásenie a navigovanie v službe jednoduché. Zákazník by mal byť schopný rýchlo nájsť presne to, čo hľadá. Napríklad stránka predajcu je zbytočná, ak zákazník nevie nájsť, kde má prebehnúť platba.

Časté omyly o ITIL sú:
* Využívanie ITIL ako len ako tréningového procesu.
* Chápanie ITIL ako "dogmu" (ako implementáciu procesov namiesto toho, že slúži k podpore businessu).
* Názor, že ITIL je len pre helpdesk a podporu.
* Presvedčenie, že procesy zavádzajú zbytočnú byrokraciu.
* Predpoklad, že ITIL vyžaduje veľa času, personálu a peňazí.

### Řizení infrastruktury služeb

_Užitočnosť_ je funckionalita ponúkaná službou s cieľom splniť nejakú potrebu. Niekedy je aj opisovaná ako "čo služba robí".

ITIL definuje _záruku_ ako uistenie, že služba splní to, čo bolo vopred dohodnuté. Je možné ju zhrnúť ako "ako to služba robí". Záruka sa skladá z nasledujúcich položiek:
* Dostupnosť
* Kontinuita
* Kapacita
* Bezpečnosť

Hodnota v ITILe je definovaná ako **užitočnosť + záruka**. Je potrebné mať na vedomí, že za doručenie hodnoty zákazníkovi sú zodpovedné obe strany, avšak za meranie hodnoty je zodpovedný výlučne zákazník. 

Generické role v ITIL:
* **Vlastník služby (service owner)** - zodpovedný za doručenie služby a je kontaktnou osobou pre danú službu. Nemusí o nej vedieť všetko, no vie, kto dokáže požadované informácie poskytnúť. Zúčastňuje sa interných mítingov, reprezentuje službu vo firme, je zodpovedný za kontinuálne zlepšenie služby a rozumie jej a jej komponentám.
* **Vlastník procesu (process owner)** - zaisťuje, že proces je vhodný pre daný účel. Taktiež je zodpovedný za nájdenie možných zlepšení a za zaistenie, že proces prebieha efektívne a v súlade s tým, čo bolo dohodnuté. Navyše dokumentuje daný proces a určuje metriky merania procesu. Táto rola by sa mala vyskytovať v každom riadení služieb.
* **Manažér procesu (process manager)** - zaisťuje, že process je vykonaný správne. Je zodpovedný za riadenie procesu na dennej báze, plánuje, koordinuje a kontroluje priebeh procesu.
* **Vykonávateľ procesu (process practitioner)** - vykonáva jednu alebo viac procesových aktivít. Má jasný zoznam zodpovedností vzťahujúcich sa k procesu, ktorý vykonáva.

Organizačné aspekty ITILu sú:
* _Proces_ reprezentujúci štruktúrovanú množinu aktivít, ktoré smerujú k dosiahnutiu určitého cieľu.
* _Procedúra_ zahŕňa inštrukcie predané personálu o tom, ako majú vykonať danú aktivitu.
* _Funkcia_ je tím alebo skupina ľudí a nástroje, ktoré používajú pri procesoch alebo aktivitách.
* _Rola_ je množina povinností, aktivít a oprávnení pre osobu alebo tím. Rola je definovaná v procese.

Životný cyklus služby obsahuje nasledujúce fázy (vzťahuje sa priamo na ITIL):

>Zdroj: [https://cio-wiki.org/wiki/ITIL_Service_Strategy](https://cio-wiki.org/wiki/ITIL_Service_Lifecycle)

**Stratégia** je prvá fáza životného cyklu služby. _Je hnaná obchodnými potrebami a je hodnotená podľa hodnoty, ktorú poskytuje firme_. Počas nej sú identifikované a schválené nové alebo zmenené požiadavky na službu, ktoré sú následne zdokumentované aj s ich želanými výsledkami. V tejto fáze poskytovateľ služby navrhuje stratégiu, pomocou ktorej bude môcť splniť požiadavky klienta. 

Jedná sa o jadro životného cyklu služieb. Firma musí mať konzistentnú servisnú stratégiu, aby bolo možné zlepšiť riadenie služieb. Obchodné ciele a stratégie firmy musia byť v súlade s dlhodobou víziou.

Kľúčové otázky v tejto fáze sú:
* Kto je zákazník?
* Aké služby majú byť ponúkané?
* Ako bude meraná výkonnosť služieb? Ako bude zákazník merať hodnotu služieb?
* Ako budú kontrolované financie?
* Existuje konkurencia na trhu? V čom sa jej služby líšia?
* Ako budú zaistené strategické investície do aktív služieb?

Stratégiu životného cyklu služby môžeme ďalej rozdeliť na štyri fázy:
1. **Definícia** - Čo je firemná stratégia?
2. **Analýza** - Ako bude stratégia implementovaná? Aké prekážky môžu nastať?
3. **Súhlas** - senior management musí odsúhlasiť stratégiu pred jej implementáciou.
4. **Implementácia** (charter)

Stratégia zároveň obsahuje tzv. **4P**:
* **Perspektíva** (vízia, smer)
* **Pozícia** (základňa, kde firma pôsobí)
* **Plán** (ako bude dosiahnutá vízia)
* **Profil** (spôsob realizácie)

Procesy definované pre servisnú stratégiu:
* **Riadenie obchodných vzťahov (business relationship management)** - zaoberá sa budovaním vzťahu medzi poskytovateľom služby a klientom. Identifikuje zákazníkove potreby a zaisťuje, že poskytovateľ je schopný ich napliť aj napriek ich zmenám a meniacim sa okolnostiam. Riadi ich **manažér obchodných vzťahov**.
* **Riadenie portfólia služieb (service portfolio management)** - riadenie množiny poskytovateľových služieb naprieč ich životným cyklom. Spravuje ho **manažér portfólia**.
* **Finančný management IT služieb (Financial management for IT services)** - riadenie rozpočtu, účtovníctvo a vystavovania faktúr za IT služby. Identifikovanie nákladov poskytovania IT služieb. Je za ňu zodpovedný **manažer financií**.

**Design** prijíma výstup stratégie. Počas tejto fázy sa vypracuje servisné riešenie a definuje sa všetko, čo bude potrebné pre prevedenie služby zvyšnými fázami životného cyklu. V podstate sa jedná o produktový management.

Obchodné požiadavky sa analyzujú a následne sa vytvárajú návrhy vhodného riešenia služby, technológie, procesov a meraní služby. Taktiež sa v tejto fáze vytvárajú a udržiavajú politiky a návrhové dokumenty.

Pri návrhu služieb sa využíva Holistický prístup, pomocou ktorého sa zaistí konzistencia a integrácia všetkých činností a procesov IT (na systém sa pozerá ako na celok a sleduje sa, aby nové služby nerozbili existujúci systém).

Medzi hlavné ciele fázy designu patria:
* Návrh služieb vyhovujúcich obchodným výstupom.
* Identifikácia a správa rizík.
* Návrhy procesov podporujúcich životný cyklus zlužby.
* Návrh metód pre merania a návrh metrík.
* Vytváranie a správa plánov, procesov, politík a štandardov pre podporu návrhu kvalitných riešení.
* Realizácia stratégie.
* Zaistenie, že doručenie služby je kvalitné, zákazníci sú spokojní a je dosiahnutá efektivita nákladov (cost-effectiveness).

Vybrané procesy spojené s designom služieb sú:
* **Koordinácia designu** zaisťuje, že ciele designu služby sú dosiahnuté.
* **Riadenie úrovne služby (Service level management)** zaisťuje, že definovaná úroveň je schválená a doručená. Je udržiavaná **service level manažérom**.
* **Riadenie informačnej bezpečnosti (Information security management)** zaisťuje, že integrita dát je zachovaná v IT službách. Riadi ju manažér bezpečnosti.
* **Riadenie dostupnosti (availability management)** sa zaoberá dostupnosťou služieb tak, aby spĺňali dohodnutú úroveň.
* **Riadenie kontinuity služby (IT Service continuity management)** rieši obnovenie služby po prírodnej katastrofe alebo udalosti, ktorá výrazne ovplyvnila fungovanie firmy.

**Prechodná fáza** (transition) prijíma definíciu vytvorenú v dizajne (tzv. **service design package**). V tejto fáze sa služba vytvorí, otestuje, vyhodnotí, a nasadí do operačného prostredia. Taktiež v tejto fáze prebieha podpora služby a postupné odstavenie nepotrebných služieb.

Vo fáze prechodu sa zameriava na implementáciu všetkých aspektov služby a je potrebné zaistiť funkčnosť služby aj v neštandardných situáciách. Ak nastane chyba, je nutné mať dostupnú podporu.

Ciele fázy prechodu sú:
* Porozumenie všetkým službách, ich užitočnnosti a zárukám, aby sme mohli dodať službu v patričnej kvalite.
* Podpora prenosu znalostí, podpora rozhodovania, znovupoužitia procesov a systémov.
* Vytvorenie formálnej politiky a spoločného rámca pre implementáciu zmien.
* Predvídanie a riadenie. Je nutné byť proaktívny a zisťovať pravdepodobné požiadavky.

Niektoré procesy pre prechod (transition) služby sú:
* **Riadenie zmeny (change management)** - riadi zmeny od ich vyžiadania až po uzatvorenie (príkladom môže byť výmena starého PC za nový aj so zachovaním dát). Je za ňu zodpovedný **manažér zmien**.
* **Plánovanie a podpora prechodu (transition planning and support)** poskytuje koordináciu všetkých aktivít spojených s prechodom služby.
* **Knowledge management** je proces bežiaci naprieč celým životným cyklom služby, v ktorom sa zlepšuje kvalita robenia manažérskych rozhodnutí zaistením, že správne informácie sú dostupné počas životného cyklu. Riadi ju **knowledge manager**.

**Fáza operácií** (operations) sa zameriava na poskytovanie efektívnych operačných služieb s cieľom doručenia požadovaných výsledkov a hodnoty zákazníkovi. **V tejto fáze je teda obvykle hodnota doručená a meraná.**

Taktiež je potrebné vyvážiť konfliktné ciele:
* Vnútorný pohľad IT oddelenia *vs* vonkajší pohľad businessu
* Stabilita *vs* vnímavosť
* Kvalita služby *vs* náklady na služby
* Reaktivita *vs* proaktivita

Vo fáze operácií je potrebné spravovať **udalosti**, ktoré predstavujú významné zmeny stavu pre správu konfiguračnej položky alebo služby IT.

Udalosť môže indikovať, že niečo nepracuje správne. Na základe toho sa zaznamenajú **incidenty**.

Kľúčovou funkciou je **service desk**, ktorý umožňuje bod kontaktu pre všetkých užívateľov IT. Zaznamenáva a a spravuje všetky incidenty a servisné požiadavky. Je potrebné rozhodnúť, či service desk bude lokálny alebo centralizovaný.

**Technická správa** je ďalšou funckiou, ktorá zahŕňa všetok personál zaisťujúci technickú odbornosť a správu infraštruktúry. Identifikuje znalosti a odborné požiadavky, definuje štandardy architektúry a poskytuje podporu správy kontraktov.

Vybrané procesy fázy operácie:
* **Riadenie incidentov** sa zameriava na riadnie prerušení alebo znížení kvality služieb a zaisťuje, že služba je obnovená do dohodnutej doby. Je za ne zodpovedný **manažér incidentov**.
* **Riadenie udalostí** identifikuje upozornenia prichádzajúce z IT zariadení a využíva ich k zaisteniu normálneho chodu služieb a k správnej reakcii pre prípad odchýliek od normálu.
* **Riadenie problémov** sa zaoberá problémami, ktoré sú dôvodom jedného alebo viacerých incidentov. Ich príčiny nebývajú známe v dobe vytvorenia záznamu o probléme. Riadenie problémov skúma problémy a kategorizuje ich. Po vytvorení záznamu o probléme hľadá jeho riešenie.
* **Spĺňanie požiadaviek (request fulfillment)** spracúva požiadavky užívateľov; môže sa jednať o jednoduché otázky týkajúce sa používania aplikácie alebo žiadostí o nový software alebo hardware. 

**Kontinuálne zlepšovanie služby** identifikuje príležitosti k zlepšeniu zaregistrované na základe meraní a reportov o efektivite a zhode služieb s požiadavkami. Návrhy na zlepšenie môžu byť nájdené v každej fáze životného cyklu služby. Pre zlepšenie služby sa používa _Demingov cyklus_ pozostávajúci z nasledujúcich fáz:
1. Plan
    * **Identifikácia prístupu k zlepšeniu**. Pred implementáciou stratégie zlepšenia je potrebné porozumieť nutnosti kontinuálneho zlepšenia. Je potrebné zvážiť finálne ciele a taktiež je nutné brať do úvahy súčasné a budúce plány.
    * **Definícia toho, čo bude merané**. Je potrebné porovnať, čo je ideálne merať, a čo je možné merať. Rozdely majú byť identifikované a realistický plán by mal byť zavedený do stratégie zlepšenia.
2. Do
    * **Zber potrebných dát**. Dáta sú získané cez monitoring, ktorý môže byť manuálny alebo automatizovaný.
    * **Spracovanie dát**. Zozbierané dáta sú prevedené z metrík na výsledky KPI.
3. Check
    * **Analýza dát**. Viaceré zdroje dát sú skombinované za účelom premeny informácií na znalosti (knowledge), ktoré sú ďalej vyhodnocované s ohľadom na všetky interné a externé faktory.
    * **Prezentácia a utilizácia informácií**. Analyzované informácie potrebujú byť odprezentované správnym spôsobom tak, aby boli zmienené potrebné detaily, no zároveň aby bolo jednoduché informáciám porozumieť.
4. Act
    * **Implementácia zlepšení**. Implementovaná zmena nastavuje novú základnú úroveň celého procesu. Získané poznatky majú byť kombinované s predošlou skúsenosťou a využité pri robení informovaných rozhodnutí. Zlepšenia sa musia zamerať na optimalizáciu a opravu služieb, procesov a nástrojov.

Kontinuálne zlepšovanie služby sa zameriava predovšetkým na maximalizáciu efektívnosti a efektivity. Ďalšími cieľmi kontinuálneho zlepšienia v ITIL sú:
* Analýza, vyhodnotenie a odporúčanie vylepšení pre akúkoľvek fázu životného cyklu služby.
* Zvyšovanie efektivity nákladov (cost-effectiveness) IT služieb.
* Implementácia aktivít zameraných na zvýšenie kvality IT služieb.
* Zvyšovanie efektivity nákladov doručenia IT služby pri zachovaní rovnakej spokojnosti zákazníkov.
* Zaistenie, že je použitá štandardná a relevantná metóda pre riadenie kvality.

![](https://i.imgur.com/fzIsztu.jpg =550x)