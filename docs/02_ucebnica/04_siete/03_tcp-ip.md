---
title: Referenčný model TCP/IP
slug: model-tcp-ip
publish: true 
---

Predpokladalo sa, že koncepcia sieťovej architektúry daná referenčným modelom OSI bude vo svete dominantná. Vývojom siete Internet vznikol model TCP/IP (Transmission Control Protocol/Internet Protocol), ktorý sa vďaka rozšíreniu internetu stáva dominantným. Veľmi často sa označenie TCP/IP chápe iba ako len označenie sady sieťových protokolov TCP a IP používaných v sieťach s počítačmi s operačným systémom UNIX. 

V skutočnosti však TCP/IP označuje model sieťovej architektúry, ktorému je priradený súbor protokolov, ktoré nie sú viazané iba na operačný systém UNIX. Model je štvorvrstvový a na nasledujúcom obrázku je „prirovnanie“ vrstiev TCP/IP k referenčného modelu OSI.

Model TCP/IP nevznikol len zlúčením niektorých vrstiev modelu ISO/OSI. Internetový model vznikol ako riešenie praktického inžinierskeho problému, OSI model je výsledkom teoretického prístupu. Rozdiel je napríklad v pohľade na zaistenie spoľahlivosti prenosu, kým OSI model počíta so sústredením čo možno najviac funkcií, vrátane zaistenia spoľahlivosti prenosov, už do komunikačnej podsiete (kontrolné mechanizmy má skoro v každej vrstve), model TCP/IP nedáva až taký dôraz na zaistenie spoľahlivosti (na potvrdzovanie, opätovné zasielanie poškodených paketov atď.) a voľnú kapacitu využíva na vlastný dátový prenos. Čiže jednotlivé vrstvy referenčného modelu TCP/IP nerobia presne to isté, čo príslušné vrstvy modelu OSI.

**"V skratke"**

**ISO/OSI referenčný model definuje 7 vrstiev**, cez ktoré musia dáta prejsť pri ceste z jedného uzla na druhý

1. **fyzická** – prenos a príjem bitov
2. **linková** (spojová) – prenos rámcov, detekcia chýb + ich oprava, pridáva hlavičku, adresa je fyzická (MAC), každý uzol vidí len susedov
3. **sieťová** – prenos paketov konečnému adresátovi, smerovanie, používa logickú adresu (IP)
4. **transportná** – komunikácia medzi procesmi – nielen medzi uzlami, detekcia a/alebo oprava chýb
5. **relačná** – bezpečnosť - šifrovanie, synchronizácia, podpora transakcií, určenie spôsobu komunikácie, ukončenie prenosu, RPC – protokoly umožňujúce počítačom prenášať dáta alebo požiadať o služby iné počítače
6. **prezentačná** – rovnaké dáta interpretovať rovnako
7. **aplikačná** – jednotné rozhranie medzi programom a sieťou – el. pošta, www,...

**TCP/IP iba 4 vrstvy**

1. **vrstva sieťového rozhrania** (fyzická a linková) – nie je v TCP/IP presne definovaná - ISDN,
GSM, el. rozvody, satelit prenos, káblová TV,...
2. **sieťová** 1. vrstva je rôznorodá - nutnosť jednotného adresovania – logické adresy (URL)
3. **transportná** – komunikácia koncových účastníkov, využíva nespojovaný a nespoľahlivý prenos. Ponúka:
    - **TCP** - spojovaný a spoľahlivý prenos
    - **UDP** (User Datagram Protocol) - nespojovaný a nespoľahlivý prenos, využíva napr. DNS
4. **aplikačná** - el. pošta, prenos súborov,...

