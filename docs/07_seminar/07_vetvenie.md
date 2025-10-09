---
title: Vetvenie
publish: true
---


## Demonštrácia

- [Učebnica AbcPython - 16. hodina - Vetvenie](https://abcpython.input.sk/p16.html)

## Ukážka

Vytvor kruh na náhodne generovaných súradniciach, tak aby sa celý nachádzal v grafickom okne. Kruh bude mať farbu výplne podľa [kvadrantu](https://cs.wikipedia.org/wiki/Kvadrant_(geometrie) grafického okna. Od 1. po 4. kvadrantu sa postupne vystriedajú farby z palety CMYK. S pomocou viacerých volaní funkcie na vytvorenie kruhu nakreslite aspoň 4 kruhy.

## Cvičenie

**Každá dvojica** mentor/mentee v triede bude riešiť **len jednu úlohu** na vetvenie. Dohodnite sa dvojice medzi sebou o prerozdelení úloh (učiteľ do spôsobu prerozdelenia nezasahuje). 

Vo dvojici vyriešte spoločne úlohu, forma spolupráce mentor/mentee je na rozhodnutí dvojice. Po dokončení úloh všetkými dvojicami príde k prezentácii vášho riešenia ostatným dvojiciach. Preto ak skončíte skôr ako ostatní, premyslite si ako v skratke (max. 4 minúty) opíšete svoj program.


## Úlohy na prerozdelenie

### č.1

Z mnohých firiem nosia na poštu veľa listov. Podľa pravidiel pošty môže byť hmotnosť listov najviac jeden kilogram. Pracovníčka pošty položí list na váhu, označí cieľ: Slovensko (s), Európska únia (e) alebo Inde (i) a druh zásielky obyčajne (o) alebo doporučene (d). 

Prepravné tarify sú takéto:

- Základ – pre list do 200 gramov
    - obyčajne: Slovensko 0,33 €, Európska únia: 0,50 €, Inde: 0,75€
    - doporučene: Slovensko 0,50 €, Európska únia: 1 €, Inde: 1,20 €
- Poštovné za každý list ťažší ako 200 gramov sa zvyšuje o 20 percent.

Napíšte program, ktorý na základe vstupných údajov : hmotnosť, cieľ a druh zásielky vypočíta a vypíše:

1. Pre jeden list na základe jeho načítanej hmotnosti napísať OK LIST, ak je ľahší alebo rovný 1000 gramom a vypísať POŠLITE AKO BALIK, ak je ťažší ako 1000 gramov.
2. Pre jeden list základe zadaného cieľa, spôsobu dopravy a hmotnosti vypísať cenu za prepravu

- Vstup
```
e o 20
s d 250
i d 1020
i o 300
```
- Výstup
```
0.50
0.60
POSLITE AKO BALIK
0.90
```

### č.2

Na postupne zadávaných riadkoch na klávesnici máme zapísané hmotnosti a výšky žiakov triedy. V jednom riadku je informácia o jednom žiakovi v tvare: hmotnosť v kg a výška v m. Napíšte program, ktorý vypočíta BMI index každého žiaka. BMI je telesný hmotnostný index, ktorý sa vypočíta ako podiel hmotnosti v kilogramoch a výšky v metroch na druhú.

- BMI < 18,5 -  podváha,
- 18.5 <= BMI < 25 - normálna hmotnosť,
- 25 <= BMI < 30 - nadváha,
- BMI > 30 -  obezita.

Vytvorte program, ktorý

- Pre každého žiaka vypočíta a vypíše jeho BMI index
- Zistite, koľko žiakov má podváhu a koľko percent žiakov je obéznych
- Vhodným grafom vyjadrite pomer jednotlivých kategórií BMI indexu

### č.3

Simulujte hádzanie troma kockami. Na obrazovku vykreslite kocky (štvorce) s "hodenými" číslami.

Ak sú všetky tri hodnoty rovnaké vypíše sa správa BOMBA! , ak sú dva z nich rovnaké, vypíše sa správa SUPER!, inak sa vypíše SMOLA.

### č.4

Vytvorte program pre učiteľa, na vyhodnotenie opravenej písomnej práce. Počet žiakov a známky sú postupne zadávané na riadkoch na klávesnici.

- Po načítaní výsledkov písomných prác počítač vypočíta, koľko bolo jednotiek, dvojok, trojok, štvoriek a pätiek z písomnej práce a aká bola priemerná známka.
- V grafickej ploche vytvorte vhodný graf počtu jednotlivých známok
