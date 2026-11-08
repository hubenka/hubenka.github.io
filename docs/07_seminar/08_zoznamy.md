---
title: Zoznamy
slug: zoznamy
publish: true
---

## Úvod

alebo aj jednorozmerné polia

- polia majú vždy prvky len rovnakého typu (homogénne)
- zoznamy môžu mať prvky rôzného typu (heterogénne)

## Učebnica

- [Polia (list)](https://python2016-sphinx.readthedocs.io/sk/latest/09.html)

## Práca so zoznamami

- Vytváranie: `veci = []`
- Zisťovanie dĺžky: `len(veci)`
- Indexovanie (prístup k prvkom zoznamu): `veci[0]`
- Iterovanie (prechádzanie prvkov zoznamu):

```
for i in range(len(veci)):
    print(veci[i])
```

```
for vec in veci:
    print(vec)
```

- Mazanie: 
    - Podľa pozície: `veci.pop(0)`
    - Podľa obsahu: `veci.remove(10)`
    
    
### Úlohy

# Číslo 1

Naprogramuj súťaž loptičiek. Loptičky padajú z hornej časti obrazovky smerom dolu.

- Na začiatku hry nastavte štartovaciu pozíciu pre 10 loptičiek. Pre každú loptičku vygenerujte náhodnú farbu.
- Zabezpečte, aby sa každá loptička náhodne posunula smerom dolu.
- Po dosiahnutí dolnej časti obrazovky nech počítač vypíše číslo lopty, ktorá vyhrala. Nech výpis je tou farbou ako lopta, ktorá vyhrala.

## Číslo 2

Zaznamenané sú body na trase, v ktorých sa mení sklon terénu (prudšie stúpa, začína klesať a pod.).
- V X[0] sú súradnice začiatku a platí x[0] = 0. V X[i] je posun v smere osi x oproti predchádzajúcemu stanovisku. V Y[i] je nadmorská výška i-teho bodu na trase. Úsek i má na osi x krajné body X[i-1] a X[i]. Údaje sú v metroch.

Vytvorte program, ktorý:

- vypočíta a vypíše dĺžku turistickej trasy,
- vypíše počet úsekov, na ktorých nadmorská výška neklesá,
- vypíše hodnotu najväčšieho rozdielu nadmorských výšok na jednom úseku a jeho poradie na trase


## Číslo 3

Napíšte program na výpočet priemernej výšky žiakov vo vašej triede. Vytvorte textový súbor vyska.txt a naplňte ho náhodne vygenerovanými 25 výškami žiakov z intervalu ⟨150, 200⟩. Vypíšte výšku najvyššieho a najnižšieho žiaka, priemernú výšku a počet žiakov vyšších ako priemerná výška.
