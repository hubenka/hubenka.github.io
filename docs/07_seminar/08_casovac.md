---
title: Časovač
publish: true
---

## Demonštrácia

- [Učebnica - Časovač](https://python2016-sphinx.readthedocs.io/sk/latest/10.html#casovac)

## Úloha pre 3.ročník

Cieľ: Programovo ovládať herné a neherné postavy v 2D grafike

- Rozpohybovať svoje postavičky (Spraviť funkciu pre kreslenie postavičky bolu na DÚ)
    - Herná postava bude reagovať na stlačenie kláves na klávesnici
    - NPC (nehrateľné postavičky) sa budú samovoľne pohybovať medzi určenými bodmi


## Úlohy pre 4.ročník

Mentor môže použiť časti z nasledujúcich úloh na vysvetlenie udalostí v grafickej ploche a časovača.

### č.1

Vytvorte hru (program), ktorá bude v pravidelných časových intervaloch (1000 ms) vykresľovať na náhodnom mieste na grafickej ploche (600x600 bodov) zelený štvorec
s dĺžkou strany 50 bodov, do ktorého má hráč kliknúť. Ak sa v časovom intervale trafí do štvorca má bod, ak nie, tak bod stratí. V hornej časti gr. plochy hrač vidí vypísaný bodový stav.

Na začiatku hry má hráč bonus 2 body. Hra končí, ak hráč získa 10 bodov (vypíšte oznam, že vyhral) alebo má -5 bodov (hráč prehral).

### č.2

Do grafickej plochy nakresli kružnicu (napr. pre r, x0, y0 = 100, 150, 120). Potom naprogramuj časovač, ktorý bude rovnomerne posúvať červenú bodku (napr. kruh s polomerom 5) na obvode tejto kružnice (napr. po každom tiknutí časovača posunie jeho pozíciu o uhol na kružnici o 10 stupňov). Posúvanie kruhu budeš robiť pomocou canvas.coords()

### č.3

Urobte program, ktorý bude simulovať preteky dvoch vozíkov. Preteky spustíme stlačením tlačidla ŠTART alebo kliknutím myšou na zelený kruh s polomerom 20
bodov v hornej časti grafickej plochy. Po skončení pretekov sa na obrazovku vypíše, ktorý vozík vyhral.



