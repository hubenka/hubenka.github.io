---
title: Projekt: Počítačová sieť u nás doma
slug: projekt-siet
publish: true
---

Zisti ako funguje vaša domáca LAN sieť! :)  Kresbu ponechám na tvojej fantázii, musí však obsahovať nasledujúce:

1. **Zakresli všetky zariadenia v LAN sieti** pripojené cez akékoľvek prenosové médium. Patria sem hlavne aktívne sieťové prvky, koncové zariadenia ako sú počítače, mobily, televízor a pod.
2. **Pomenuj zariadenia** v sieti a zapíš ich **IP adresy (IPv4), MAC adresy, informácie o sieťovej karty** zistené podľa MAC adresy (napr. [https://macaddress.io](https://macaddress.io) alebo [https://maclookup.app](https://maclookup.app)).
    - Adresy zariadení nemusia byť priamo vo vašom obrázku, môžu byť napr. v tabuľke veďla. Adresy zistíte buď priamo v zariadení (cez sieťové nastavenia / `ipconfig`) alebo z iného zariadenia skenovaním siete: (v `cmd.exe` cez príkaz: `arp -a`)
3. Zisti **vlastnosti svojho internetové pripojenia**. Nápoveda aké vlastnosti je potrebné zistiť nájdeš na: [http://porovnavacinternetu.sk](http://porovnavacinternetu.sk), ale minimálne: **poskytovateľ, rýchlosť sťahovania, rýchlosť nahrávania, typ pripojenia**).
    - Veľa z vlastností dokážeš priamo zmerať: [https://meracinternetu.sk](https://meracinternetu.sk) alebo [https://www.speedtest.net/](https://www.speedtest.net/)
4. Zisti a vypíš **cestu z vašej LAN siete cez WAN (internet) k tebou vybranej doméne** (webovej stránke). Použi príkaz `tracert`. Pre viac detailov si môžeš prečítať [popis trasovania cesty](https://cs.wikipedia.org/wiki/Traceroute).
    - Zapíš aj časy k jednotilivým miestam na trase.
    - Pre IP adresy po trase zisti aj ich zemepisnú polohu pomocou napr. [https://ipinfo.io/](https://ipinfo.io/)
4. *(riešiť len v prípade že `tracert` nevypisuje trasu)* Zapíš IP adresy pre aspoň tri rôzne domény. Použi príkaz `nslookup` v `cmd.exe`.

Projekt môže byť spracovaný ľubovoľne podľa dohody s učiteľom: na papieri, v počítači, na výkrese.

**Bonus:**

Ľubovoľná jedna z úloh je bodovaná:

- Umelecký nákres počítačovej siete
- Podľa masky siete LAN zistite koľko najviac koncových zariadení sa dokáže pripojiť cez tvoj smerovač v LAN.
- Používate vo vašej lokálnej siete IPv6 adresy? - ak áno zapíšte ich do tabuľky ku zariadeniam


### Body:
- Termín: do 28.10.2024
- Maximum 20 bodov

1. 6 b
2. 6 b
3. 4 b
4. 4 b

Bonus
5. (Bonus) 2 b

