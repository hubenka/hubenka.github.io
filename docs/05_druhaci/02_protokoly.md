---
title: Prečítaj správy medzi počítačmi
slug: protokoly
publish: true
---

## Návod

1. Nainštaluj si program [Wireshark](https://www.wireshark.org/)

2. Odskúšaj si nahrávanie *sieťovej premávky* - to sú všetky správy, ktoré si posielajú počítače medzi sebou. Naprv zatvor všetky nepotrebné programy (karty prehliadača), ktoré môžu posielať nadbytočné správy.

3. Kliknutím na sieťovú kartu sa spustí nahrávanie premávky určenej tvojmu počítaču.
![Vyber sieťovej karty](/2-rocnik/assets/vyber-rozhranie.png)

4. Spusti program, ktorý sa pripája na internet a chceš ho zaznamenať. Chvíľu potom zastav nahrávanie pomocou červeného štvorčeka
![Tlačidlá](/2-rocnik/assets/ws-tlacidla.png)

5. Nájdi správu na ktorú sa pýta úlohu a rozklikni si vrstvy TCP/IP na nájdenie odpovede

6. Spusti nahrávanie znovu pomocou zeleného tlačidla

## Úlohy

1. Aké všetky sieťové protokoly sú použité v HTTP správe pri dopyte na webovú stránku?: [http://example.net](http://example.net)

2. Koľko milisekúnd prejde medzi dopytom od tvojho počítača na webovú stránku (z úlohy 1) do prijatia odpovede?

3. Aká je IP adresa tvojho počítača a adresáta z úlohy 1?

4. Čím sa líši dopyt na webovú stránku [https://example.net](https://example.net) od úlohy 1?

5. Podľa akého údaju v HTTP správe počítač vie, že sa stránka našla (vyskúšaj: [https://www.raca.sk/](https://www.raca.sk/)) alebo sa nenašla (vyskúšaj: [https://www.raca.sk/stranka](https://www.raca.sk/stranka)). Ako sa líšia tieto dve situácie?

6. Čo všetko vieš zistiť z HTTP správy o počítači, ktorý ti posiela naspäť webovú stránku (o serveri)?

7. Z vrstvy pre Ethernet II z ľubovoľnej predošlej úlohy vypíš MAC adresu susedného uzla v sieti (adresáta).

8. Aké všetky skratky protokolov aplikačnej vrstvy si zachytil v záznamoch sieťovej premávky? Napíš aspoň 5 so stručným vysvetlením ich činnosti (načo sú dobré?)

9. Napíš vymyslené prihlasovacie meno a heslo do toho formulára [http://vbsca.ca/login/login.asp](http://vbsca.ca/login/login.asp). Akými názvami sú v správe označené meno a heslo, dajú sa vôbec odčítať zo správy?

10. (Bonus) Aký sieťový protokol a obsah správy používa `tracert google.sk` na zistenie routerov po ceste?
