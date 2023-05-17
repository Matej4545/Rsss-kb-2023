# 6  Projektové řízení I

###### tags: `řsss-základ`, `project-management`, `management`


**Definica statnicovej otazky:**

- Projektové řízení. Mezinárodní standardy projektového řízení. Projekt, program, portfolio (PPP). Životní cyklus IT projektů. Procesní skupiny v projektu. Plánování projektů. Výpočet nákladů projektu. Ganttovy diagramy a projektové milníky. Síťová analýza, metoda kritické cesty (CPM), Program Evaluation and Review Technique (PERT). Zajištění kvality projektu, testy, přezkoumání, měření a standardy. (PA179)
- poznamky som pisala rovno popri pozerani prednasok, je tu toho dost

## PROJEKTOVE RIADENIE 

Kazdy standard ho definuje trochu inak ale spaja ich, ze to je: Set metod, technik, nastrojov, kompetencii, ktore sa aplikuju na projekty, aby splnili projektove poziadavky, naplnili svoj ciel a udrzuju balans medzi cost-time-scope.

Je dost citlive na zmeny, rizika. 

### CO JE **PROJEKT**

Kazdy standard ma svoju definiciu projektu, su odlisne no spaja ich, ze kazdy projekt smeruje k dodávke produktu. Projekt je teda casovo ohranicene usilie (*temporary*), ktore ma unikatnu vlastnost (*unique*), dochadza pocas neho k zmenam(*change driving*), nachadza sa v nom miera neistoty(*uncertain*) a ultimatne, smeruje k dosiahnutiu cieľa. 

*Temporary* - kazdy projekt ma start a koniec a svoj lifecycle (typicky pre-project, inititation, execution, closing):
- Pre-project: studie proveditelnosti, priprava ziadosti
- Initiation: detailny harmonogram, rozpocty, zostavovanie timu
- Execution: vytvorenie realizacie, neni tak zaujimave pre projektaka
- Closing: predavanie, akceptacia, fakturacie, archivacia a retrospektiva vo firme

*Change driving* - riadenie zmenami. Projekt ma mat prinos(value - kvantifikovatelny benefit)  pre stakeholdrov (ktokolvek, kto zasahuje alebo je zasiahnuty projektom). Prinos je popisany v business case

*Unikatnost* - projekt nie je bezny biznis, nie je to rutinny delivery packagu. Kombinacia jednotlivych faktorov ho robi unikatnym no kazdy projekt ma repetitive elementy = procesy

*Uncertainty* - Je to vlastne riziko, pravdepodobnost ze sa stane udalost, ktora sposobi skodu. Pri projektoch je vela rizik pretoze ide o novu cinnost, treba pocitat s rizikami a pripravit nejaku risk strategy, assessment ap..

Hranice projektu definuje **projektový trojimperatív** - rozsah, cena, čas. Zmena jedného parametru vedie k zmene *minimálne* jedného ďalšieho.

### CO JE **PROCES**

Sled samostatnych cinnosti, ktore na seba nadvazuju a na zaklade vstupnych poziadavkov vytvara vystup. Procesy su designovane ako opakovatelne, su na zaciatku detailne skumane, odladene, odsimulovane a casom sluzia ako sablona.

Projekt je vlastne unikatny set procesov, ktore mozu byt opakovate a automatizovane. Procesy mozu byt pouzivane v roznych projektov.

![](https://i.imgur.com/bDomQ2F.png)



## **PPP - PORTFOLIO, PROGRAM, PROJECT**

**PROJECT** - Cinnosti co maju spolu nieco urobit v istom case. Riadi ich projektovy manazer a ten dava pozor najme na terminy, rozpocet a na vysledok projektu. Co chceme vytvorit, za kolko penazi a kedy. 

**PROGRAM** - Set docasnych projektov, ktore maju spolocnu vlastnost a smeruju ku common objective - spolocnemu cielu. Prinasa hodnotu stakeholdrom.

**PORTFOLIO** - Prebiehajuci set projektov a programov, ktore spolu nesuvisia a smeruju ku strategic objectives - strategickym cielom. =firma Pridava hodnotu businessu.

## **MEDZINARODNE STANDARDY PROJEKTOVEHO RIADENIA**

Vyuzivaju sa aby sme mali lepsie vysledky, pracovali efektivne, zvysili transparenciu, nevynalezali zas kolo.

- *PRINCE2* = Project in controlled environments
- PMI PMBOK = Project management institute project management body of knowledge
- *IPMA ICB* = International project management association  individual competence baseline

### **PRINCE2**

Procesne orientovana metodika  roku 2017 (druha verzia). Ma preskriptivny charakter, je to proste vyplnanie formularov, papierov, nic pre kreativnych ludi. Ma 7 principov (e.g. learn from experience), 7 tem (e.g. risk = what if) a 7 procesov (e.g. assign key people in  starting up a project).

Tuto metodu je najlepsie dodrziavat od zaciatku do konca, vhodna rovnako pre zacinajucich aj skilled managerov. Tato medoda neadresuje managements poziadavkov a budget - na to treba iny standard. PRINCE2 najcastejsie vyuzivaju firmy, ktore potrebuju dokladne reporty, detailnu dokumentaciu a manazment typu “kontrola a rozkazy” -> statne zakazky na ministerstve, jadrove elektrarne. Certifikacia je sice okej, ale nikto na tom uz teraz nebaziruje.

### **PMBOK**

Procesne orientovana metodika no dava vacsiu volnost. Spravna metodika ak sa rozhodneme, ze zacneme PRINCE2 a potom sa zamyslime, ze projekt je mensi a teda PRINCE je overkill. Ma 10 knowledge areas (e.g., Cost, Quality), 5 process groups (Inicializace, Planovani, Exekuce, Monitoring a kontrola, Closing) a 49 procesov (ma popisane co je vstup, ake ma kriteria, nastroje a outputy).

Nenajdeme tu zakladne myslineky co robit, principy ale je to tam nejak vsadene. Ku PMBOK existuje PMBOK Process flow co je diagram popisujuci kazdu process group, jej procesy ktore sa maju odohrat.
Relativna novinka je PMI Talent Triangle, ktory reaguje na vlastnosti project managera - mal by mat hard skills, leadership skills, strategicke a business skills.

Najlepsie je pouzivat tuto metodu ako guide, poradi ake techniky a nastroje pouzit, moze ho pouzit zaciatocnik aj pokrocily project manager. Certifikat z PMI je dost vyzadovany v USA.

### **IPMA ICB**

Popisuje jednotlive kompetencie (kompetencia=aplikacia vedomosti, znalosti a schopnosti za ucelom dosiahnutia vysledku), ktore by mal projektovy manager splnovat cize ide o kompetencne orientovany pristup k riadeniu projektu. 

Knowledge (pochopenie Gantt chart) < Skills (vytvorenie Gantt chart) < Abilities (schopnost uspesne menezovat project schedule)

ICB ma 3 oblasti kompetencii a pre kazdy su popisane pozadovane dovednosti a aj sposoby ako ich zmerat:
- 5 perspektivnych kompetencii - e.g., strategy, culture and values
- 10 “people” kompetencii - e.g., leadership, teamwork
- 13 praktickych kompetencii - e.g., finance, stakeholders

IPMA moze byt vyuzita kedykolvek, je skor uzivana ako guide a obsahuje detailnu sekciu a soft skills. Je vhodna pre pokrocilych projektovych manazerov. Certifikacia ma 4 urovne.

Vsetky 3 standardy su dokopy ako paradajkova polievka: PMBOK je ako kucharska kniha sefkuchara,  PRiNCE2 ako recept na obycajnu paradajkovu polievku a IPMA ako navod na ziskanie sefkucharskych kompetencii.

## PROCESNE SKUPINY
V PMBOK ide o logicke zoskupenie do  Inicializace, Planovani, Exekuce, Monitoring a kontrola, Closing (Ukončenie).

**Inicializace**
Pomáha nastaviť víziu, čoho chceme v projekte dosiahnuť.

**Plánovanie**
Zostavenie všetkých detailných dokumentov o projekte (milníky, rozpočet, požiadavky, riziká, dokumentácia atď.), tzv. *projektový plán*.

**Exekuce**
Uskutočnenie projektového plánu zostaveného v predošlej fáze.

**Monitoring a kontrola**
Pomáha vyhodnocovať aktuálny stav projektu a hľadať riešenia v prípade odchýlok od plánu (cena, rozsah, čas).
Je aktívna po celú dobu projektu

**Ukončenie (Closing)**
Uzavretie projektu, predanie výstupov, podpisy zmluvných strán, platby, zhrnutia projektu atď.

Good practise je aj identifikácia chýb pre poučenie sa do ďalších projektov.

## **ZIVOTNY CYKLUS IT PROJEKTOV**

Rozdiel medzi standardnym projektom a IT projektom je, ze IT projekt pouziva na delivery informacne technologie. Ich vyvoj je rychlejsi, IT projekty sa casto navzajom ovplyvnuju, rizika sa nedaju tak dobre predpokladat (potrebny risk management!) a tak sa IT projekty typicky realizuju iterativnym inkrementalnym sposobom. Vysledok projektu je sucastou sluzieb a produktov, ktore firma ponuka a vyzaduje dalsi manazment.


ITIL -  IT Infrastructure Library - popisuje best-practice pre IT service management, ma 5 levelov:
- Service strategy
- Service design
- Service transition
- Service operation
- Nasledny service improvement

### **ZIVOTNE CYKLY**
#### **WATERFALL**
Je to stare a nepouzitelne na SW development. Na zaciatku su poziadavky, potom ich zanalyzujem, spravim, testujem nasadim. Kazda faza sa robi za cely system, no je to obrovske, neflexibilne, tazky na zapracovanie zmien.

#### SPIRAL
Inkrementalny (vzdy pridavame po troske) a iterativny (designovany v opakujucich sa cykloch). Vhodnejsi na SW development, vacsina momentalne pouzivanych metod je nejaka variacia spiraloveho modelu.

### PRISTUPY K SW DEVELOPMENT

#### PREDIKTIVNY
Rigidny, zamerieva sa na procesy, ma fixovane poziadavky, planuje dopredu => ***Unified process***

Dost vyuziva UML, je to prediktivna, iterative-inkrementalna technika. Cely projekt sa deli z pohladu vyvoja na iteracie:
- Inception - ziskame poziadavky
- Elaboration - analyza, design, vytvorenie UML diagramov
- Construction - vytvorenie
- Transition - uzavrenie, testovanie, odovzdanie

Kazda z tychto faz by nemala trvat viac ako 3 mesiace, rozdiel medzi dvomi po sebe nasledujucimi iteraciami sa nazyva inkrement. Kazda faza musi obsahovat 6 workflows:
- Business Modeling - Activity Diagram
- Poziadavky - Use Case Diagram
- Analyza a design - Class, Sequence, Collaboration Diagram
- Implementacia - Class, Object, Component Diagram
- Testovanie - UC, Class, Activity Diagram
- Deployment - Deployment Diagram


Pouziva sa ked vacsina poziadavkov musi byt specifikovana dopredu, potrebujeme kompletnu kontrolu nad procesmi a timami a detialnu dokumentaciu (vo forme UML).

![](https://i.imgur.com/V7og6fY.png)

#### AGILNY
Flexibilny, zamierava sa na ludi, poziadavky su pravidelne aktualizovane, neplanuje dopredu => ***SCRUM***

Agilna, iterative-inkrementalna metoda. Teoria SCRUMU je popisana v “The SCRUM Guide” co je kratky dokument so striktnymi pravidlami, ktore tvoria SCRUM tym, cim je. Ocakava sa, ze dalsie metodiky, techniky a nastroje su pridane aby sme dosiahli ciel projektu. SCRUM je charakterizovany:
- 5 Udalostami
- 3 Artefaktami
- 3 Rolami

![](https://i.imgur.com/Es2JJeB.png)


*ROLES*

- *Product Owner* - ten, kto hovori, co chce za svoje peniaze. Vybera si poziadavok zo Product Backlogu a co si on vyberie do nasledujucej iteracie (Sprint), sa nazyva Sprint Backlog. Na konci sprintu vznika Product Increment. Vytvorenie Sprint Backlogu sa nazyva Sprint Planning.
- *SCRUM Master* - je to vlastne projektak, zameriava sa na procesy, jeho zodpovednostou je davat pozor na to, aby SCRUM ostal SCRUMom a menezuje cely tento proces.
- *Team of Developers* - 3 az 9 ludi, udrziavaju Sprint Backlog, ich zodpovednstou je vytvorit produkt.

*ARTIFACTS*

- *PRODUCT BACKLOG* - Reprezentuje celkovu specifikaciu a odhaduje pracnost (technika na odhadovanie mnozstva prace - Planning Poker).Jednotliva funkcionalita je vyjadrena vo forme User Stories a tie maju Story Points. Product backlog vytvara cely SCRUM  tim, zvycajne je vo forme nejakej tabule kde su sticky notes. Product backlog sa musi nacenit.
- *SPRINT BACKLOG* - Cast User Stories z product backlogu, ktora definuje pracu, ktora sa planuje vykonat v ramci sprintu, vytvara ho tim developerov. Vybrane User Stories su zmenene do uloh a maju priradeny casovy odhad. User Stories mozu byt pridavane/odoberane ak sa tym nenarusi Sprint Goal.
- *PRODUCT INCREMENT* - Reprezentuje vsetky polozky z Product Backlogu, ktore sa vykonali pocas Sprintu + minuly inkrement. Vsetky polozky musia byt v stave “Done”, nie in progress ani to-do.

*EVENTS*
- *SPRINT PLANNING* - 2h meeting na zaciatku kazdeho sprintu, kde sa stretne cely SCRUM tim a nastavia si Sprint Goal, vyberaju polozky z Product Backlogu a priradzuju k nim ulohy.
- *SPRINT* - Jedna iteracia, ktora ma vyustit vo funkcny a product inkrement, ktory moze byt releasnuty. Nemal by byt dlhsi nez 1 mesiac. Podiela sa na nom cely SCRUM tim. Typicky analyse-design-build-test pristup.
- *DAILY SCRUM* - 15min meeting kazdy den, kde je iba team developerov, mozno SCRUM Master. Kazdy z clenov zodpovie otazky: “Co som robil vcera? Co budem robit dnes? Mam nejaky problem?”
- *SPRINT REVIEW* - 4h meeting po 1 mesacnom sprinte. Pritomny je cely tim a klucovy stakeholdri. Prekontroluje sa inkrement, zhodnoti sa, prejde sa product backlog, spocita sa progres, prekalkuluju sa datumy.
- *SPRINT RETROSPECTIVE* - 3h meeting za 1 mesacny sprint. Je tam cely SCRUM team, diskutuje sa aktualny sprint, jeho clenovia, vztahy, procesy a nastroje. Cielom je prist s aspon jednym vylepsenim do nasledujuceho sprintu.

SCRUM sa moze skoncit napr.:
- Product backlog je prazdny
- Nesu peniaze, cas
- Product owner sa rozhodne zastavit projekt

SCRUM sa pouziva ked presne poziadavky nevieme dopredu, tim dobre spolupracuje a komunikuje a zakaznik chce nejaku formu produktu ASAP.

## **PLANOVANIE PROJEKTU**

Pri planovani projektu a vybere pristupu k menezovaniu musime zobrat do uvahy rozne veci, e.g., velkost timu, dlzka projektu, komunikaciu a kooperaciu v time, delivery (chceme produkt cim skor, hoci aj vo verzii ktora sa este bude upravovat?), typ poziadavok (budu pribudat casom alebo ich vieme vsetky na zaciatku?). 

### AGILNY PRISTUP - IS pre disabled students

Sklada sa z 3 casti:
- Planning
- Sprinting
- Closing

#### PLANNING

Mozeme konzultovat IPMA ICB a PMBOK, ktore nam pomozu s formalou stranou projektu:
- Vytvorenim Projektoveho Chartru - Poskytuje ho IPMA. Ma 5 otazok:
    - BUSINESS CASE = WHY - vysvetlime oficialne dovody, benefity projektu z pohladu firmy. (skoro ako marketing). Nacrtneme najvacsie risky, vydaje a budget.
    - OUTCOME = WHAT - jednoduchy popis produktu, poziadavky, ciele, hlavne ciele
    - STAKEHOLDER = WHO - indentifikacia klucovych externych+internych stakeholdrov
    - APPROACH = HOW - popis ako bude menezovany projekt - llifecycle, pouzite standardy, vybrat vhodne nastroje, metody, koncepty.
    - SCHEDULE = WHEN - klucove milniky
- Manazmentom klucovych strategii (komunikacia, risks, cena, kvalita, kompetencie, changes)
    - *Communication management strategy* - Nastavit si, ako sa bude komunikovat - face-to-face, dokumentacia, show-don’t tell, rychle meetingy. Treba kratko spisat ake budu meeting, reporty, kto sa ich bude ucastnit a ake budu uzivane mechanizmy. 
    - *Risk management strategy* - Vytvorenie risk strategy ktora sa typicky sklada z (v IPMA, PMBOK):
        - Identifikovania zakladnych rizik
        - Ohodnotenia riskov - hodnotenie = pravdepodobnost ze sa prejavi * dopad, definovat nasledky
        - Odpovede na jednotlive risky - Transfer/Avoid/Reduce/Accept
        - Specifikacie monitoringu riskov - kto je zodpovedny? Kde budu risky definovane, reviewed?
        - Vytvorenia registra riskov
Medzi najcastejsie rizika patri nedostatok ludi, nerealisticke odhady cien a casu, nepochopenie poziadavkov. Znizuje rizika: transparentnost co sa deje, feedback, pouzivanie user stories (cize popis toho, co ma byt urobene), zaclenenie zakaznika do planovania, kratke iteracie.
    - *Change management strategy* - Jak sa bude postupovat, ked pride zakaznik so zmenou pocas vyvoja. Pri novom poziadavku sa rozhoduje ci sa zastavi alebo nezastavi aktualny sprint.
    - *Quality management strategy* - Otazky ohladom kvality riadenia procesu, timu kde si stanovime quality objectives (e.g., deliver on-time s maximom 2% chybovostou), miery ktore zlepsuju procesnu kvalitu (nastroje). V SCRUME napr. User storied s akceptacnymi kriteriami, sprint retrospektivy, burndown chart (meria schopnost timu prinasat inkrementy nacas, osa x reprezentuje cas od zaciatku sprintu/projektu a osa y zbyvajici story points = imaginarna jednotka pracnosti). Team velocity = kolko story points vie tim dokoncit za den (sprint)
    
![](https://i.imgur.com/sLExlvb.png)
    
    
- Manazmentom *Product backlogu* 
Do product backlog sa davaju user stories (1), ktore ohodnotime z pohladu pracnosti (2) a dame im priority (3)
    - User stories jednoducho popisuju funkcionalitu z pohladu uzivatela, sucastou su i akceptacne kriteria (co znamena, ze poziadavok je splneny).a mozne suvisiace rizika.
    - Odhadovanie pomocou *planning poker* (hlasuje sa s kartickami, kym sa nepride k spolocnemu cislu. Ak sa ludia nezhodnu, musia svoje volby okomentovat)  na pracnosti user stories.
    - Prioritizovanie cez MoSCoW metodu (must have, should have, could have, won’t have)

#### SPRINTING

- Sprint planning - z product backlog sa nieco vyberie a to sa stane Sprint goal
- Daily SCRUM - Podporuje transparentnost, progres, adaptaciu.
- Sprint review - Zamerany na novy inkrement, co sa ma spravit, co sa spravilo,kontrola product backlogu. Meria progres
- Sprint retrospective - Zamerany na tim, komunikaciu, nastroje a procesy. Meria vykonnost (peformance)
- Updating key strategies - Ak sa zisti, ze sa nieco robi nespravne, tak sa updatuju strategie


Do samotneho sprintu patri i:

- Riesenie timovych konfliktov
Fazy konfliktov: 
    - Latent (mozne, zatial nebadatelne) 
    - Emergent (viditelne, zatial rozumne)
    - Escalated (open conflict)
    Mozme vyuzit napr.*De-escalation technique*, kde zmiernime najprv emocie, ideme sa niekde pokojne porozpravat, aktivne pocuvame a hlavne, komunikujeme s respektom a nie posudzujuco
- Zmena poziadaviek - jedina vec, ktoru treba rozhodnut je, ci sa sprint zastavi alebo nie

#### CLOSING THE PROJECT
- Finisovanie produktu - na konci sa zvycajne dohodne na poslednom sprint review
- Prechod k operations, dokumentacia - uzivatelska dokumentacia je vyrabana priebezne, technicka dokumentacia zalezi na dohodnutej forme supportu (viac o tech. Dok. hovori ITIL)
- Timeline retrospective - co sme sa naucili? Co sa malo stat a co sa stalo naozaj? 

### PREDIKTIVNY PRISTUP - mestske kiosky

V priklade kombinujeme PRINCE2 (pomaha s terminologiou, rolami, zakladnymi principmi, reporting, projektovou dokumentaciou, projektovy plan => cize s riadenim projetu) a unified process (pomaha s procesom vyvoja produktu, zberom poziadavkov, produktovou dokumentaciou => cize s vyvojom produktu). Manazment bude velmi administrativny s detailnou dokumentaciou, praca je kontrolovana a udavana, scope definovany dopredu. 

#### STARTING PHASE

- Project brief (PRINCE2) - zakladny dokument, prakticky rovnake ako project charter + definovat tim, role + definovat aky manazmentovy pristup zvolime
- High-level requirements (UP) + definovat viziu, core funkcionalitu
- Feasibility analysis (UP) + odhad ceny, casoveho planu, riskov
- Outline architecture (UP) - navrhneme aspon 1 mozne riesenie 
- Next stage plan (PRINCE2) - vytvorit detailny day-to-day plan => WBS, identifikacia aktivit, odhadutie ich trvania, milestones. Vytvorit Gantt/Network diagram


#### INITIATION = ELABORATION PHASE

- *Project Initiation Documentation (PID)* (spisane zakladne principy projektařiny - spravi sa detialny business case, rozpracovať detailnejsie strukturu timu, change, quality, risks, communication management approach … je to vlastne detailny project brief) + jeho sucastou je *Project plan* (PRINCE2)
    - Detailny business case definite dovody na projekt, ocakavane benefity, analyzu výdajov a prijmov, najvacsie risky, …
    - Struktura timu - Project board (Executive = zadavatel + Zastupca dodavatela + Zastupca koncového užívateľa) a pod nimi su projektovi manazeri, timovi manazeri. Project board schvaluje vsetky plany, vynimky a odchylky od planu
    - Quality management approach - vytvára sa Quality register (zaznamy o vsetkych aktivitach, ktore sa maju robit), quality manager kontroluje napr. ci sa dodrziavaju ISO standardy, ako casto sa testuje, co sa testuje
    - Change control approach - vytvara Issue register (definica co sa spravi, ak pride požiadaviek na zmenu)
    - Risk management approach - vytvara sa Risk register (identifikujeme rizika, planujeme opatrenia)
    - Communication management approach - definovat napr. Kto komu co posiela, ake reporty, ako casto
    - *Project plan* - vytvorenie WBS (popísané nizsie), vypocitat casove a cenove odhady (PERT, popísané nizsie), identifikovanie závislosti a odhadnutie aktivit (Precedence diagramming method, popisane pri agilnom projekte),, rozvrh (Gantt chart vyssie + Network chart nizsie)
- *Detailed requirements* (UP)
    - Zhromazdit detaily vacsiny poziadavkov
    - Vytvorenie detailych use-casov na vacsinu funkcionality (zacinaju tu pracovat analytici)
    - Vytvorenie špecifikácie produktu - dvojita špecifikácia, jednak use-cases pre vyvojarov a jednak scenare pre uzivatelov (tu kliknes a zobrazi sa obrazovka). Produktova specifikacia je základom pre kontraktovanie (zakaznik plati az na konci za cely produkt)
- *Stage report* (PRINCE2) - report za prave prebehnutu etapu, popisuje progres, celkovu situaciu projektu, ohodnocuje timovy performance, produkt a jeho kvalitu, obsahuje sumar aktualnych riskov, problemov
- Next stage plan (PRINCE2) - rovnake ako pri starting phase

#### DELIVERY PHASE

Zvycajne je komponovaná z viacerých fáz, kazda je ako malý projekt a nemala by trvat viac ako 3 mesiace. V tejto fáze je rola projektového manažéra udrzat projekt *cas, budget, scope a kvalitu tak, ako bolo dohodnute v Project Initiation Documentation*. Zacina uz analyzou, dizajnom, pokracuje programovanim a konci testovaním, integrovanim. PRINCE2 nerozlisuje praktickú implementáciu ako delivery narozdiel od UP, ktory povazuje za delivery práve tu praktickú implementáciu.

- *Robust Architecture *(UP)
    - V UP je to este sucast elaboration ale PRINCE2 to uz povazuje za delivery kedze ide o navrh architektury - moduly, technologie, identifikácia rizik ( napr. kompatibilita, vykon HW)
- *Controlling a stage* - projektovy manazer vedie dokumentaciu v ktorej popisuje, ako vyvoj vyzera. Obsahuje dokumenty ako:
    - Work package - popis cinnosti, co sa prave robi, kto to robi, kym sa akceptuje, ...
    - Highlights report - sumar o faze, ktory sa predava project board
    - Daily log
    - Issue/Risk register updates - zmenove poziadavky i rizika sa chovaju podobne, treba na to reagovat. Ak poziadavok alebo riziko presiahne toleranciu/projektu => eskalacia na project board a vyplni sa Exception report => na neho sa viaze Exception plan, ktory pokryva cas od teraz do konca faze
- *Managing product delivery* - z pohladu timoveho manazera
    - Team plan - dokument, ktory hovori kto bude na com pracovat
- *Managing a stage boundary* = kontrolovnie hranic jednotlivych faz vykonavane projektovym manazerom
    - End stage report - ako stage report v initiation phase
    - Next stage plan - ako pri starting phase
    - Project plan update
    - Risk register/Issue register/Quality register update
    - Business case update - to sa obvykle nedeje

#### TRANSITION (UP) AND CLOSING (PRINCE2) PHASE

**Transition phase**:
- *System acceptance (UP)* - Acceptance existuje v UP pretoze PRINCE2 je metoda pre rozne typy projektov,, nie len IT. V poslednej faze Construction v UP mame k dispozicii uz Beta system - relativne stabilny system, integrovany, testovany, pripravene k uzivaniu ale beta verzia sa pouziva 2-3 mesiace a potom sa prejde na produkcnu
- *Transition phase (UP)*
    - Cielom je urobit akceptovatelny system, aby sa dal pouzivat
    - Dopisuje sa dokumentacia - uzivatelska, vyvojarska, operations, trainings
    - Zacina trening uzivatelov, ktory budu so systemom pracovat
    - Beta testing - prinasa user feedback cize vlastne poziadavky na zmeny, treba si vymysliet sposob spracovania a zbierania feedbacku. V tomto bode je dolezity *Configuration management*  pretoze je bezne mat aj 3 rozne prostredia (production, testing, dev)
- *Product acceptance testing* je formalne testovanie systemu, finalna verifikacia pozadovanej funkcionality, ktora overi ci boli splnene vsetky poziadavky kontraktu. Vypisuje sa dokument *Acceptance protocol*

**Closing phase**:
- *Product handover*(PRINCE2)
    - Co bude dalej so SW - definujeme SLA = Service level agreement, zmluva o servisnej podpore, kde sa definuje ake su typy chyb, reakcne doby, pokuty, cena servisu, … SLA je sucast Service Level Managementu, ktory je sucastou ITIL Service Designu
    - Presunut zodpovednost za produkt z projektu na operations a udrzbu
- *Zatvorenie vsetkych registrov, logov, archivacia dokumentacie*
- *End project report* (PRINCE2) - formalny report s “tvrdymi” cislami
- *Lessons learned report* (PRINCE2) - menej formalne, skor pre tim. Doporucenia do buducna, pohlad zakaznika, necakane udalosti, review uzitocnych technik

![](https://i.imgur.com/7UQatEE.png)

![](https://i.imgur.com/QsSqt45.png)



## **VYPOCET NAKLADOV PROJEKTU**

Napriklad pomocou PERTu, kde od pracnosti odvinieme ohadovany cas potrebny na dokoncenie prace, priradime cenu cloveka, ktory to bude robit. Je potrebne mysliet na pridavanie buffrov.

Existuje viacero sposobov, akym sa vytvara budget, jeden z nich je:

- Urci sa cenu vsetkych aktivit. Z PERTu vieme, kolko budu stat jednotlivy ludia. K tomu treba pridat dalsie vydaje ako SW licencie, cestovne, ceny nastrojov a materialov, PR, HR, …
- Traverzovanim WBS zdola hore urcime cebu kazdeho work packagu a z toho vyvodime cenu nazyvanu *Project estimate*
- K project estimate sa prida *Contingency reserve*, ktora reprezentuje sumu vsektych projektovych riskov. Project estimate a contingency reserve spolu tvoria *Cost baseline*, cislo ktore sa pouziva na urcenie CPI / CV
- Na vrch cost baseline sa pridava *Management reserve* na zatial neurcene vydajne
- Toto vsetko spolu tvori *Cost budget*

## **SIETOVA ANALYZA, KRITICKA CESTA**

### SIETOVA ANALYZA

Sietova analyza sa vyuziva hlavne na zobrazenie tokov penazi, casu v projektu. Na sietovu analyzu sa pouziva aj Gantt chart, ktory moze zobrazovat kriticku cestu.

## GANTT CHART A PROJEKTOVE MILNIKY

Ganttov diagram je esencialny nastroj na projektove planovanie. Reprezentuje planovane aktivity vo forme “kalendaru” (os x reprezentuje aktivity, os y datumy), ktory obsahuje ich start a koniec a zavislosti medzi nimi. Moze byt vylepseny o milniky (dolezite body delivery), zdroje (kto robi co).

Sucastou Gantt chart je casto Precedence Diagramming Method, pouzivana na zobrazenie moznych zavislosti medzi projektami: 

- Finish-to-start - aktivita 2 nemoze zacat, kym aktivita 1 neskonci
- Finish-to-finish - aktivita 2 nemoze skoncit, kym aktivita 1 neskonci
- Start-to-start - aktivita 2 nemoze zacat, kym aktivita 1 nezacala
- Start-to-finish - aktivita 2 nemoze skoncit, kym aktivita 1 nezacala (malo uzivane)

### KRITICKA CESTA

Metoda, ktora pomaha s kontrolou, ci stihame projekt dokoncit nacas. Vyzera ako sietovy diagram, ktory definuje aktivity a doby ich trvania. Do grafu sa pomocou dopredneho a spätneho priechodu dopisuju:

**Dopredný prechod**
- Určuje časy brzkého začátku (**Early Start - ES**) a brzkého konce (**Early Finish - EF**) pro každou úlohu.
- Postupuje se zleva doprava.
- Přidávají se časy na každé cestě.
- Pravidlo: pokud několik úloh konverguje do jednoho uzlu, pak čas ES následující úlohy je roven největšímu z EF časů předchozích úloh.
- Pomocou dopredneho prechodu pocitame najskorsie mozne zaciatky a konce projektu. Zaciname v bode 0, ak vidim ze trvanie = 10, zacnem v 0 a skoncim najskor v 10ty den. Aktivity F,B,H mozu zacat najskor v 11. F trva 15, cize najskor moze skoncit v 25. Na vypocitanie konca pripocitame DUR ku zaciatku, v pripade ak ide o vazbu Finish-to-start (prenasam koniec na start), ktora je najcastejsia. Start-to-start by preniesol start z A do startu B,F,H (1->1) , finish-to-finish by preniesol koniec aktivity A na koniec aktivit B,F,H a musim dopocitat start. Je to dobre pre alokaciu zdrojov.

**Spätný prechod**

- Určuje čas nejpozdějšího konce (**Late Finish - LF**) a čas nejpozdějšího začátku (**Late Start - LS**).
- Začíná se v koncovém uzlu.
- Vypočítají se spodní páry čísel.
- Odečte se trvání od času brzkého konce v připojeném uzlu
- Pravidlo: pokud několik úloh konverguje do jednoho uzlu, pak čas LF následující úlohy je roven nejmenšímu (opačně jako u dopředného průchodu) z LS časů předchozích úloh.
- Pomocou spätneho prechodu pocitame najneskorsie mozne zaciatky a konce. Po vypocitani dopredneho prechodu postupujeme od poslednej aktivity a odratavame DUR ( E 65-20=45, na 46 den najneskor musim zacat poslednu aktivitu). G,D,H musi najneskor skoncit na 45ty den aby posledna aktivita mohla zacat hned o den neskor. H musi zacat najneskor na 31. Den (45(skonci v tento den)-15(DUR)=30, cize nasledujuci den). Tu vidime, ze H moze zacat najskor na 11ty den a najneskor na 31.den, inak sa projekt omeska.
 
**Výsledná Critical Path**
- Cesta poskladaná z uzlov, kde **EF** a **LF** sú rovnaké.

Objavi sa linia, kde najskorsie a najneskorsie mozne zaciatky a konce su rovnake. Tu sa nesmiem omeskat, pretoze potom sa cely projekt omeska a to je kriticka cesta.


Optimalizacia mimo kriticku cestu NEMA vplyv na cele trvanie projektu, cize skratenie projektu ma zmysel hladat v aktivitach v ramci kritickej cesty. Po ich skrateni ale moze nastat kriticka cesta inde!

![](https://i.imgur.com/5Ffvz3x.png)



## WBS

NIE JE sucastou hlavnych otazok. Je to hierarchicka dekompozicia prace, ktora sa ma vykonat na celom projekte. Cely projekt dekompunujeme na casti= Work packages, co su najmensie dekomponovatelne jednotky. Tie sa mozu skladat z dalsich cinnosti ale su uz tak male, ze nema zmysel ich dalej rozoberat.

Pravidla pre tvorbu WBS:
- Dekomponujeme cely projekt, v sucte by cely diagram mal vyjadrovat prave 100%
- Kazda cinnost by mala byt zahrnuta v celom diagrame prave 1 krat

![](https://i.imgur.com/0opZwth.png)


## **PERT = PROGRAM EVALUATION AND REVIEW TECHNIQUE**

Probabilisticka technika na odhad pracnosti potrebnej na vykonanie jednej cinnosti. Cinnost je definovana tromi typmi casoveho odhadu:
- Optimisticky cas *o* (mozne minimum)
- Pesimisticky cas *p* (mozne maximum)
- Pravdepodobny cas *m* (najlepsi odhad)

Z tychto casov je vypocitany ocakavany cas *te; te = (o+4m+p) / 6*

Zakladny PERT, ktory odhaduje cas, moze definovat aj odhad ceny. Ku kazdej cinnosti sa prida cenova kategoria cloveka , ktory bude danu cinnost vykonavat (wage level MD), usilie ktore tomu bude venovat dana cenova kategoria (effort per wage level MD) a pocet pracovnych dni, ktore su potrebne na dokoncenie cinnosti (expected duration WD).

![](https://i.imgur.com/j31yYMJ.png)


## **ZAISTENIE KVALITY PROJEKTU, TESTY, PRESKUMANIE, MERANIA A STANDARDY**

Vsetky tieto veci boli nejakym sposobom popisane pri agilnom a prediktivnom pristupe. Tu uvadzam informacie, ktore neboli v prednaske ale v ISe v interaktívnej osnove.

Vhodne pozriet:

https://docs.google.com/document/d/1VdDZRrxK3bJLfXBRhOBmjmYBoZ4FMElaI-lsUGigl9w/edit#heading=h.ljn1iiwwgsfb

https://www.projectsmart.co.uk/project-management-scope-triangle.php

### MERANIA

Projektovi manazeri su vzdy nejakou formou kontrolovani - ci uz ide o zakaznika, spozora alebo vrchny manazment. Tito ludia sa mozu zucastnovat meetingov a byt tak v obraze no castejsie vyzaduju iba reporty o statuse. Zvycajne sa pouzivaju 4 metriky:
- SPI = Schedule performance index - vyjadrene ako pomer mnozstvo zatial urobenej prace / mnozstvo prace, ktora bola planovana, ze bude doteraz urobena. CPI>1 znamena ze sme popredu, CPI<1 znamena ze meskame
- SV = Schedule variance - rovnake ako SPI ale hodnoty sa odcitaju. Vysledok <0 znamena, ze meskame
- CPI = Cost performance index - kolko budget sa zatial minulo v porovnani s hodntou, co zatial vznikla. Interpretacia je analogicka ku SPI
- CV = Cost variance - rovnake ako CPI, ale hodnoty sa odcitaju

Pri standardoch sa dava pozor na to, ci sa dodrziavaju napr. ISO normy, platna legislativa, GDPR, ...

![](https://i.imgur.com/m36omH8.png)


### ZAISTENIE KVALITY

So zaistenim kvality suvisi hlavne hrozba riskov, ktore moznu projektu znacne poskodit. V risk managemente rozlisujeme kvalitativnu a kvantitativnu cast ohodnocovania riskov.
- Kvalitativna cast
    - Najprv definujeme vsetky mozne udalosti, ktore sa mozu udiat. Tieto udalosti nemusia byt iba negativne (=threat), mozu mat ja pozitivny dopad (=opportunity). Kazdy risk ma priradene 2 dimenzie na ohodnotenie pravdepodobnosti a dopadu daneho risku na projekt. Obe hodnoty su v istej mierke, napr. 1-5, kde nizsia hodnota znaci mensiu pravdepodobnost alebo mensi dopad na projekt. Tieto 2 hodnoty sa potom vynasobia a ziskame konecnu hodnotu, ktora nam stanovi ako velmi by sme sa mali zaujimat o dany risk

![](https://i.imgur.com/DLB5e7G.png)


- Kvantitativna cast
    - Vsetky pravdepodobnosti sa prerataju do percent (ak sa incident I stane raz za 10 rokov a projekt je planovany na 2, pravdepodobnost je 20%). Tiez sa transformuju “abstraktne dopady” na nieco konkretne, najcastejsie na napr. zarobene/utratene peniaze navyse.

Na risky treba nejak zareagovat, a teda sa planuje *Risk response plan*, ktory hovori o tom, co s danym riskom urobime. Rozlisujeme 4 kategorie:

- Avoid / Exploit (pri pozitivnych)
- Mitigate / Enhance (pri pozitivnych)
- Transfer / Share (pri pozitivnych)
- Accept

Ako dalsiu polozku v manazmente riskov vytvarame *Contingency plan*, ktory hovori o akciach vykonanych ak riskova udalost nastane. Risk management je nepostradatelny pre uspesneho projektoveho manazera, vdaka tomuto manazmentu je tim pripraveny na mozne udalosti a vie na nich promptne reagovat.

### TESTING

Unit testy => Komponentove testy => Integracne testy => Test celeho systemu

Acceptance testing


