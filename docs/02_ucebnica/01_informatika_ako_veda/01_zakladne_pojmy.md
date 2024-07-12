---
title: Základné pojmy informatiky
slug: zakladne-pojmy
publish: true 
---

## Počítač
Prvým pojmom, ktorý by sme si mali objasniť, je samotný pojem počítač. Inak vyzerá domáci počítač, inak počítač vo výpočtovom stredisku a ešte inak superpočítač. Každý z nich rieši iné úlohy. Jeden vie napr. množstvo hier, iný vydáva miestenky na autobus a pod. Niektoré počítače sú univerzálne, teda sú schopné riešiť rozličné úlohy, iné sú jednoúčelové, napr. hodinky, kalkulačka. Mnoho ľudí definuje počítač ako stroj, ktorý dokáže myslieť. Je to hlboký omyl. Žiadny počítač nedokáže myslieť. Dokáže robiť len to, čo mu predpíše človek. 

**Počítač je (elektronický) stroj, ktorý dokáže vyriešiť rôzne typy úloh podľa vopred zadaného programu.**

Počítače využívame z týchto dôvodov:

- počítač dokáže vyriešiť zadanú úlohu podstatne rýchlejšie ako človek,
- počítač býva pri riešení zložitých úloh spoľahlivejší ako človek,
- počítač si dokáže zapamätať viac údajov ako človek.

Povedali sme, že počítač dokáže riešiť úlohy podstatne rýchlejšie ako človek. Tá rýchlosť je čoraz väčšia - dnes nie je zvláštnosťou, keď počítač dokáže spracovať miliardy operácií za sekundu. To nám umožňuje nasadzovať ho do oblastí, ktoré by bez takýchto výkonných počítačov nemohli vôbec existovať - kozmický výskum, predpoveď počasia, letectvo, vojenská technika...

Čo sa týka spoľahlivosti - vieme, že každý človek je omylný. Niekto viac, iný menej. Pri počítači je to trocha iné. Ak chceme mať istotu, že daná úloha bude počítačom vyriešená správne, musíme mať overený program na riešenie danej úlohy. Potom máme veľmi veľkú pravdepodobnosť, že počítač chybu nespraví. Ak chceme túto pravdepodobnosť zmeniť takmer na istotu, môžeme použiť nasledujúce riešenie: Zoberieme nepárny počet počítačov, (napr. 3, 5, 7, ...), vhodne ich prepojíme, a necháme ich riešiť danú úlohu samostatne každým počítačom. 

Keď sa počítače dopracujú k riešeniu, porovnajú si výsledky. Ak sú výsledky na všetkých počítačoch zhodné - úloha je vyriešená správne. Ak sa výsledky nezhodujú, potom sa za správny výsledok bude považovať ten, ku ktorému sa dopracovala väčšina počítačov. Súčasne sa bude hľadať príčina, prečo prišlo pri riešení danej úlohy ku chybe. (Tento postup sa úspešne využíva napr. v programe amerických raketoplánov.)

## Algoritmus

V definícii počítača boli použité slová program a algoritmus. Vo výpočtovej technike pod pojmom algoritmus rozumieme postup, ako riešiť zadanú úlohu. Každý program musí obsahovať návod, ako riešiť daný typ úlohy a musí byť zapísaný v nejakom programovacom jazyku.

**Algoritmus je postup alebo návod ako riešiť zadanú úlohu.**

**Algoritmus** je formálne opísateľný, mechanicky vykonateľný postup na riešenie triedy problémov, ktorý v tvare programu môže realizovať počítač.

**Program** je návod na činnosť počítača, ktorý musí byť zapísaný v nejakom programovacom jazyku.

**Programovací jazyk** je sústava slov a pravidiel na zápis algoritmu tak, aby mohol byť spracovaný počítačom.

Každý algoritmus sa skladá z elementárnych príkazov (inštrukcií), ktoré sú za sebou uložené v takom poradí, aby sa ich vykonávaním vyriešila zadaná úloha.

Informatika sa však neobmedzuje iba na čistú programátorskú prácu, ale sa zaoberá aj úplne všeobecným skúmaním štruktúry algoritmov, spracovaných dát (údajov), ako aj jazykov umožňujúcich vhodné formulovanie algoritmov a programov.

## Hardvér a softvér
**Hardvér** tvoria všetky tie časti počítača, ktoré súvisia s jeho konštrukciou. Nazývame ho aj technickým vybavením počítača.

**Softvér** zahŕňa v sebe všetky programy, podľa ktorých počítač pracuje. Označujeme ho aj ako programové vybavenie počítača.


## Informácia

Do počítača zadávame údaje, ktoré poznáme a od počítača čakáme, že keď danú úlohu vyrieši, dozvieme sa od neho niečo nové, čo sme dosiaľ nevedeli. Tieto nové údaje nazývame informácie. Informácia umožňuje odstraňovať neurčitosť, spresňovať nejasnosti, vnášať poriadok do dejov.

**Informácia má dve základné charakteristiky:**

1. možno ju merať - jej množstvo (kvantitu), napr. na pošte sa platí za telegram podľa počtu slov (počet slov je vyjadrením množstva informácie)
2. má svojho adresáta - pre ktorého môže, ale nemusí mať význam.

## Údaje (dáta)
Údaj je každá správa bez ohľadu na to, či má pre nás nejaký informačný obsah alebo nie - inými slovami - či nám daná správa povie niečo nové, alebo nie. Údaje (dáta) sú správy, ktoré vyjadrujú určité fakty o procesoch, alebo prvkoch reálneho sveta. Údajmi môžu byť písmená, čísla, slová, znaky, prípadne ich kombinácie. 

Všetky údaje nesú určitý informačný obsah. Ak nám daný údaj nepovie nič nového, hovoríme, že jeho informačný obsah je nulový. Z toho nám vyplýva vzťah medzi údajom a informáciou:

Každá informácia musí byť súčasne údajom, ale nie každý údaj musí byť pre nás informáciou s nenulovým obsahom.

Rozdiel medzi údajom a informáciou je napr. takáto situácia: Keď sa nás niekto spýta, koľko je hodín - my sa pozrieme na hodinky a povieme: "Je 8 hodín." Pre nás to bol údaj, pretože sme po pohľade na hodinky vedeli, koľko je hodín. Ale pre toho, kto sa nás pýtal, koľko je hodín - pre toho to bola informácia, pretože mu povedala niečo nové.

**Údaje** delíme na:

- Vstupné a výstupné
- Analógové a digitálne

## Súbor 
(angl. file) je označenie pre množinu dát (údajov) väčšinou rovnakého typu (text, obrázok, hudba). Súbor pozostáva z postupnosti rovnako skonštruovaných dátových záznamov; každý dátový záznam sa vo všeobecnosti skladá z viacerých rozličných zložiek – polí.

**Charakteristika súboru:**

- Názov (meno.prípona)
- Veľkosť ( v bajtoch)
- Umiestnenie
- Dátum a čas vzniku a poslednej zmeny
- Atribúty (vlastnosti)


## Informatika

Rozvoj výpočtovej techniky podnietil vznik a rozvoj nových odborov. V 70. rokoch nášho storočia na báze **Computer Science** - počítačovej vedy - vznikla nová vedná disciplína - **informatika**.

V roku 1978 na Medzinárodnom kongrese v Japonsku bola vymedzená definícia predmetu informatiky.

Predmetom informatiky sú oblasti súvisiace s vývojom, tvorbou, využitím, materiálno-technickým zabezpečením a organizáciou spracovania informácií vrátane ich priemyselného, ekonomického, správneho, sociálneho a politického pôsobenia.

Veda, ktorá skúma zákonitosti vzniku, spracovania a využívania informácií sa nazýva informatika.

Informatika patrí medzi najrýchlejšie sa rozvíjajúce sa vedy. Poznatky z nej sa okamžite zavádzajú do praxe a prinášajú výrazný ekonomický efekt.

Na základe rôznych hľadísk rozlišujeme:

- teoretickú,
- praktickú,
- technickú
- aplikovanú informatiku.

### Teoretická informatika
Zaoberá sa matematickým popisom procesov a počítačových systémov. Matematické metódy a modely hrajú dôležitú úlohu tak pri formulácii a skúmaní algoritmov, ako aj pri konštrukcii počítačov. Nakoľko štruktúra počítačov smeruje k stále vyššej zložitosti, zvyšuje sa aj stupeň abstrakcie zodpovedajúceho popisu. Na riešenie otázok z tejto oblasti sú potrebné dobré poznatky z modernej štrukturálnej matematiky, ktorá poskytuje celý rad formálnych metód na popis systémov. 

Kým však matematika uvažuje prevažne o statických štruktúrach, v informatike je spôsob myslenia charakterizovaný dynamickým priebehom procesov. Príkladmi
podoblastí teoretickej informatiky sú teória formálnych jazykov, teória automatov, teória zložitosti a sémantika.

### Praktická informatika
Zaoberá sa základnou komunikáciou medzi užívateľom a počítačom a medzi počítačmi navzájom. Algoritmy síce principiálne možno formulovať nezávisle od počítača, aby sa však dali spracovať na výpočtových zariadeniach, potrebné sú presné znalosti o architektúre a spôsobe práce počítačov. Programy napísané v strojovo nezávislých programovacích jazykoch treba pomocou špeciálnych prekladacích programov previesť do počítaču zrozumiteľného a počítačom vykonateľného tvaru; operačný systém dozerá na vykonávanie programov, ktoré v prípade väčších výpočtových zariadení často prebiehajú súčasne a riadi vstup a výstup.

Na druhej strane majú tieto alebo podobné úlohy vplyv na návrh nových počítačových architektúr. Informatik potrebuje mať vedomosti aj z elektrotechniky, aby vedel odhadnúť možnosti a hranice technickej realizácie. Príkladmi podoblastí praktickej informatiky sú tvorba prekladačov, informačné systémy, operačné systémy, simulácia a umelá inteligencia.

### Technická informatika 
Zaoberá sa funkčnou architektúrou počítačov a príslušných zariadení, ako aj logickým návrhom počítačov, zariadení a obvodov. Príkladmi podoblastí technickej informatiky sú prevádzka počítačov, riadenie procesov a návrh obvodov.

### Aplikovaná informatika
Informatika je v tomto ponímaní aplikovanou vedou, ktorá ovplyvňuje iné odbory a mnohé vedné disciplíny. Aplikovaná informatika zahrňuje aplikácie metód teoretickej, praktickej a technickej informatiky a iných vied. Skúma automatizovateľnosť procesov v najrozličnejších oblastiach pomocou počítača. Popri aplikačne orientovaných analýzach sa skúmajú aj inžinierske metódy pri vyvíjaní softvéru, t.j. programových systémov, ktoré majú pokryť spomínané aplikácie. Príkladmi podoblastí aplikovanej informatiky sú podniková informatika, právnická informatika a lekárska informatika.

