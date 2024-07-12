---
title: Najčastejšie sa vyskytujúce pojmy
slug: pojmy
publish: true 
---

## Adresa verejná, privátna
Verejná adresa je IP číslo, ktoré je v rámci celej siete internet unikátne a v prípade, že nie je blokované firewallom či iným bezpečnostným zariadením, aj z celého internetu dostupné. Tieto adresy sú evidované v centrálnej databáze organizácie RIPE (Réseaux IP Européens, www.ripe.net), ktorá ich za poplatok prideľuje jednotlivým organizáciám. Práve postupný nedostatok týchto unikátnych adries je dôvodom zvyšujúcich sa tlakov k prechodu na novú verziu protokolu IPv6.

Druhou skupinou sú adresy privátne, použiteľné v rámci firmy či domácnosti bez nutnosti registrácie. Tieto adresy nie sú dostupné zo siete internet a zariadenia s privátnymi adresami nemôžu do siete internet pristupovať – teda až na veľmi rozšírené využitie technológie NAT a PAT, kedy sa viacero privátnych adries maskuje pred verejným internetom pod jednu verejnú adresu, čím sa nie len zníži počet potrebných verejných adries, ale aj zvýši ochrana zariadení vo vnútornej sieti. 

Pri troche skúseností je možné takéto adresy rozoznať na prvý pohľad, sú totiž v tvare 10.x.x.x, 172.16.x.x – 172.31.x.x alebo 192.168.x.x. Je dôležité vedieť, že informácia o IP adrese sa prenáša v rámci celej komunikačnej trasy – výnimkou je iba použitie technológie NAT/PAT.

## AP, Access Point (prístupový bod), tiež WAP (Wireless Access Point)
prístupový bod, zariadenie, ktoré prepája fyzickú časť siete s bezdrôtovými zariadeniami alebo navzájom prepája bezdrôtové sieťové komunikačné zariadenia. Obsluhuje ich pripájanie a zabezpečuje overovanie a ochranu informácií. Bezdrôtový prístupový bod funguje ako fyzický opakovač (repeater) alebo ako smerovač (router). Prístupový bod sa obvykle pripája k pevnej sieti typu Ethernet, čo umožňuje prenášať dáta medzi bezdrôtovými a drôtovými zariadeniami.

## APIPA
schopnosť systému Windows nastaviť IP adresu pre sieťové rozhranie v prípade, že sa mu nepodarí kontaktovať DHCP server. Adresa je z rozsahu 169.254.0.1 = 169.254.255.254

## Autosensing
automatické rozpoznanie pripojeného sieťového kábla, označované aj ako Auto MDI/MDI-X.

## Brána
IP adresa sa pod systémom Windows konfiguruje nezávisle pre každé sieťové rozhranie. Pokiaľ má náš počítač viacero sieťových rozhraní, môže sa nezávisle pripájať do viacerých sietí s viacerými IP adresami. Zoznam sieťových adaptérov nájdeme v zložke Ovládacie panely po kliknutí na položku Sieťové pripojenia. Informácie o protokole IP získame po kliknutí pravým tlačidlom na zvolený sieťový adaptér, výbere možnosti Vlastnosti a zvolení položky Protokol siete Internet (TCP/IP). 

Okrem samotnej IP adresy a adresy siete je tu prvá zaujímavá položka. Tou je brána, ktorá slúži ako výstupný bod pre komunikáciu odchádzajúcu mimo siet. Povedzme, že máme počítač s IP adresou 192.168.0.1 a maskou 255.255.255.0. Komunikácia v rámci siete, teda na adresy 192.168.0.x bude doručovaná lokálne priamo na zariadenia. 

Čo však iné adresy? Napríklad server google.com? Práve táto komunikácia bude odoslaná na adresu, ktorú uvedieme do políčka brána, v našom prípade teda 192.168.0.254. Bránou je väčšinou internetový smerovač, ktorý sieť pripája k internetu cez NAT. Pozri tiež Maska podsiete.

## DHCP (Dynamic Host Configuration Protocol)
protokol, pomocou ktorého sieťové zariadenia získavajú konfiguráciu IP protokolu pre dané rozhranie. Jednoduchý príklad využitia DHCP servera je napr. v kanceláriách, kde je množstvo klientskych staníc s Windows a Linux, alebo ho môžete využiť, ak poskytujete internetové služby a máte mnoho klientov.

DHCP server sa stará o to, aby klient na základe vyslanej požiadavky do siete a následného overenia dostal IP adresu potrebnú pre fungovanie. Klient v sieti dostane odpoveď od servera a sám nakonfiguruje sieťové zariadenie, sieťovú kartu. Server prenajme klientovi IP adresu na určitý čas. Ten je závislý od nastavenia. Niekedy však potrebujeme, aby server pridelil klientom vždy tú istú IP adresu. No aj to sa dá. Všetky tieto informácie a ešte veľa ďalších funkcií je nastavených v konfiguračnom súbore.

## DDNS
Dynamické DNS, služba umožňujúca pristupovať na počítač užívateľa cez doménové meno aj v prípade, že má dynamickú IP adresu (napríklad pri DSL pripojení).

## DNS (Domain Name System)
prekladá doménové mená serverov na ich IP adresy a je prevádzkovaný na DNS serveroch.

## Extranet
je koncept rozšírenej podnikovej komunikácie (Extended Enterprise Communications), ktorá presahuje rámec hraníc podniku. Na vzájomnú komunikáciu medzi spolupracujúcimi podnikmi, ich partnermi, zákazníkmi, dodávateľmi slúži internet a jeho komunikačné služby. Každý z účastníkov tvorí individuálnu uzol na internete, či už interný v rámci podnikovej siete, respektíve externý mimo rámec lokálnej siete. Na rozdiel od internetu, extranet nie je široko otvorený. V protiklade od intranetu, extranet nie je zasa obmedzený na interné (vnútropodnikové) použitie.

## Firewall
bezpečnostná brána, definuje pravidlá komunikácie medzi rôznymi sieťami, určuje, ktorá komunikácia je povolená a ktorá nie, a tým chráni ostatné zariadenia pred únikom dát alebo iným zneužitím.

## Full DupleX
Duplexný prenos - prenos dát oboma smermi. Používa dva alebo viac kanálov, môže prebiehať v rovnakom okamihu oboma smermi. Na duplexné prenosy môžeme pozerať ako na dva simplexné prenosy.

## Half Duplex
Half-duplexný (poloduplexný) prenos dovoľuje výmenu informácií v oboch smeroch, avšak v každom časovom momente iba jedným smerom. Komunikujúce zariadenia sa spravidla musia vedieť dohodnúť, kedy ktoré z nich bude vysielať a kedy prijímať dáta.

## Hotspot
alebo hotzone predstavuje miesto pokryté signálom bezdrôtovej siete LAN pomocou ktorej sa dá pripojiť na internet. Táto služba je býva poskytovaná na verejne prístupných miestach ako sú hotely, kaviarne, letiská, námestia alebo akékoľvek iné miesta, kde sa zdržiava veľké množstvo potenciálnych používateľov (obchodní cestujúci, študenti...).

## Hub
rozbočovač, kopíruje prijaté dáta z jedného rozhrania na všetky ostatné rozhrania, ku ktorým sú pripojené iné zariadenia. Nepracuje s adresami a neobsahuje pokročilejšiu inteligenciu ako tomu je v prípade prepínača (switch).

## Intranet
je počítačová sieť, ktorá používa rovnaké technológie ako internet (TCP/IP, HTTP) založené na klient/server architektúre; je určená iba pre malé skupiny používateľov, napríklad pre pracovníkov podniku. Je to "interný internet".

## IPv4
je verzia 4 Internet Protocol-u o IP adresách zariadení na internete. IPv4 používa 32-bitové adresy, čo obmedzuje adresný priestor na 4 294 967 296 jedinečných adries, z ktorých je množstvo vyhradených pre zvláštne účely ako lokálne siete alebo multicastové adresy, čo redukuje počet adries použiteľných ako verejné internetové adresy. Zapisujeme ich najčastejšie v tvare: štyri celé čísla od 0 po 255 oddelené bodkami, napr. 193.87.175.245.

## IPv6
má nahradiť (okolo roku 2025) štandard IPv4, ktorý podporuje iba 4 miliardy adries, zatiaľ čo IPv6 podporuje až približne 3.4×1038 (340 sextiliónov) adries. 128-bitová IPv6 adresa sa zvyčajne zapisuje ako osem skupín po štyroch hexadecimálnych čísliciach. Napríklad 2001:0db8:85a3:08d3:1319:8a2e:0370:7334

## LAN (Local Area Network)
rozlohou malá sieť lokálneho charakteru, zväčša prepájajúca počíta če v domácnosti alebo firme.

## MAN (Metropolitan Area Network)
sieť pokrývajúca rozsiahlejšie územie mesta a jeho okolia, obvykle slúži pre prístup obyvateľov do internetu či špecifickým službám mesta.

## Maska podsiete
V súvislosti s IP adresami sa vyskytuje pre bežného užívateľa podstatne záhadnejšia maska podsiete. Jej formát je rovnaký ako formát IP adresy, v domácich sieťach má najčastejšie hodnotu 255.255.255.0 a väčšina užívateľov ju pokladá iba za zbytočnosť, ktorú treba vyplniť pri konfigurácii sieťového zariadenia. Dnes si však vysvetlíme, že až taká zbytočná nie je. 

IP adresa je tvorená z dvoch častí: adresy siete a adresy koncového zariadenia. Adresa siete hovorí odosielateľovi kam presne má informácie poslať, adresa koncového zariadenia zase kam bude informácia odovzdaná až do cieľovej siete dorazí. Mechanizmus je podobný telefónnemu číslu: predvoľba 02 hovorí o tom, že volaná osoba je v Bratislave, číslo ktoré nasleduje už konkrétne identifikuje jeho telefón.

Zrejme vám teraz prišla na um otázka ako sa dá napríklad z adresy 192.168.1.1 určiť, ktorá časť je adresa siete a ktorá adresa zariadenia. V časoch, keď platili pevne definované dĺžky sieťových adries by táto adresa patrila do triedy C, čo znamená, že prvé 3 čísla určujú adresu siete a posledné číslo je adresou zariadenia. Moderné siete však používajú takzvané beztriedne adresovanie a práve tu sa ukazuje dôležitosť masky podsiete. Práve tá totiž túto hranicu stanovuje. 

Pre príklad použijeme masku 255.255.0.0. Tá určuje, že prvé dve čísla sú adresou siete a posledné dve zase adresou zariadenia v sieti. Že nevidíte význam? Povedzme, že pri adresovaní cez triedy by sme v sieti s adresou 192.168.1.1 mohli mať iba 254 zariadení (počítačov, tlačiarní, IP kamier), pri použití masky 255.255.0.0 však ich počet narastie až na 65 000, čo už je obrovské číslo. I keď sa v praxi takto veľké siete z rôznych dôvodov nepoužívajú, pre ukázanie významu masky tento príklad vyhovuje.

## NAT (Network Address Translation)
mechanizmus prekladania jednej IP adresy na druhú, používa sa najmä pri prístupe z počítačov s privátnou IP adresou na internet.

## P2P, peer-to-peer
čo je spôsob sieťovej komunikácie, keď sú oba počíta če rovnocenné – teda opak pripojenia klient-server. Často sa využíva pri zdieľaní súborov vo výmenných sieťach.

## Ping
diagnostický príkaz, ktorý obsahujú všetky dnešné operačné systémy, ktorý pomocou protokolu ICMP overí dostupnosť cieľového zariadenia a zobrazí štatistické údaje o stave trasy.

## Proxy server
Jeho úlohou je vystupovať voči iným serverom v mene klientov. Ak klient chce z ľubovoľ ného FTP servera prevziať súbor, obráti sa na svoj proxy server a povie mu, že chce daný súbor z daného FTP servera. Proxy server sa potom pripojí na zvolený FTP server, prevezme vybraný súbor a odovzdá ho klientovi. 

Do proxy serverov sa zabudovaná vyrovnávacia pamäť (cache), ktorá zachytáva najčastejšie prenášané súbory z FTP serverov a najč astejšie navštevované stránky WWW serverov. Keď klient požiada o stránku, ktorá sa nahrala do vyrovnávacej pamäte proxy servera, proxy server iba skontroluje, či objekty na stránke na WWW serveri sú zhodné s objektmi na danej stránke v jeho vyrovnávacej pamäti, a klientovi odošle stránku z pamäte. Veľkosť cache pamäte proxy serverov môže byť až niekoľko GB.

## Repeater
opakovač, používa sa najmä pri bezdrôtových sieťach na zosilnenie signálu siete pri väčších vzdialenostiach.

## Router
smerovač, smeruje balíčky na základe cieľovej IP adresy von niektorým zo sieťových rozhraní. Jeho základnou funkciou je prepájanie odlišných sietí.

## Simplexný prenos
umožňuje iba jednosmerný prenos dát medzi vysielačom a prijímačom. Príkladom simplexného prenosu je televízne vysielanie. Informácie môžu by ť vysielané len z televíznej stanice k televíznym prijímačom.

## SSID (Service Set Identifier)
identifikátor, respektíve názov bezdrôtovej siete. Tento názov zdieľajú všetky zariadenia v jednej bezdrôtovej sieti.

## Switch
prepínač, smeruje rámce na základe MAC adresy von niektorým z rozhraní, pre ktoré má danú cie ľovú MAC adresu priradenú.

## TCP, UDP
V dnešnej dobe najpoužívanejšími protokolmi prenosovej vrstvy sú TCP (Transmission Control Protocol) a UDP (User Datagram Protocol). A aký je medzi nimi rozdiel? Zjednodušene môžeme povedať, že zatiaľ čo protokol TCP patrí do skupiny spoľahlivých protokolov, ktoré zabezpečujú doručenie jednotlivých balíčkov s informáciami v správnom poradí a do správneho cieľa, UDP takúto funkcionalitu neobsahuje, a tak ju v prípade potreby musí zabezpečovať samotná aplikácia. 

Naproti tomu sú však prenosy protokolom UDP rýchlejšie, keďže sa minimalizuje množstvo prenášaných kontrolných informácií a zasielanie správ medzi odosielateľom a príjemcom potvrdzujúcich príjem informácie. I keď by sa na prvý pohľad mohlo zdať, že nespoľahlivý prenosový protokol je nepoužiteľný, opak je pravdou. Napríklad video aplikácie tolerujú určité percento stratených dát, čo im umožňuje čerpať výhody rýchlejšieho prenosu.

## Traceroute
príkaz, ktorý zistí všetky prechodové smerovače na trase k cieľovej adrese a zobrazí aj štatistické informácie o ich dostupnosti.

## WPA (WiFi Protected Access), WEP (Wired Equivalent Privacy)
typ zabezpečenia pre siete Wi-Fi. Prekonané je zabezpečenie WEP, bezpečnejšie je WPA, dnes WPA2 (štandard 802.11i). Označenia WPA-Personal, WPA-Enterprise, WPA2-Personal, WPA2-Enterprise, 802.1x.

## WAN (Wide Area Network)
počítačová sieť pokrývajúca geograficky rozľahlú oblasť (štát, kontinent, svet), typickou sieťou WAN je napríklad internet.

## WAP (Wireless Application Protocol)
je skratka pre aplikačný protokol pre bezdrôtové zariadenia. Pozri tiež AP.

## Zdroje, rozširujúce štúdium

- http://www.linuxexpres.cz/praxe/domaci-pocitacova-sit-1
- http://www.pcspace.sk/content/view/413/36/
- http://pc-network.aspweb.cz/ine/OSI_ISO.htm
- http://sk.wikipedia.org/wiki/OSI_model
- http://sk.wikipedia.org/wiki/Po%C4%8D%C3%ADta%C4%8Dov%C3%A1_sie%C5%A5
- http://www.gymmt.sk/~alica/matury/matury2002/siete.htm
- http://www.cnl.tuke.sk/audio/by/album/pocitacove_siete_2007
- http://www.meraki.sk/
- http://informatika.schoolo.org/category/pocitacove-siete/topologia-lan/
- http://www.linuxzone.cz/index.phtml?ids=4&idc=1148
- http://referaty.atlas.sk/ostatne/informatika/48065/?page=0
- http://referaty.atlas.sk/ostatne/informatika/39443/?page=0
- http://sk.wikipedia.org/wiki/Wi-Fi
- http://referaty.atlas.sk/ostatne/informatika/33691/technologia-bluetooth-a-jej-vyuzitie
- http://sk.wikipedia.org/wiki/Global_System_for_Mobile_Communications
- http://www.wrx.sk/satellite/index.html
- http://www.owebu.cz/pc-site/vypis.php?clanek=2417
- http://www.pcspace.sk/content/view/413/36/1/1/
- http://www.gdunaba.sk/egyeb/siet.pdf
- http://www.itapa.sk/index.php?ID=3029