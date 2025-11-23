---
title: Kolízie a zoznamy
publish: true
---

## Návod - Detekcia kolízie medzi obdĺžníkmi

Obdĺžník r1 má kolíziu s obdĺžníkom r2 ak súčasne platí:

- Je PRAVÝ okraj r1 doprava od ĽAVÉHO okraja r2?
    - `r1x + r1w >= r2x`
- Je ĽAVÝ okraj r1 doľava od ĽAVÉHO okraja r2?
    - `r1x <= r2x + r2w`
- JE SPODNÝ okraj r1 pod VRCHNÝM okrajom r2?
    - `r1y + r1h >= r2y`
- JE VRCHNÝ okraj r1 nad SPODNÝM okrajom r2?
    - `r1y <= r2y + r2h`

---

## Scenár ukážky od učiteľa

### Detekcia kolízie
Pozri: [Collsion detection](https://jeffreythompson.org/collision-detection/rect-rect.php)

- V grafickej ploche je na pevnom mieste nakreslený zelený štvorec.
- Modrý štvorec pohybujeme po ploche myšou pomocou udalosti `<Motion>`
- Ak nastane kolízia štvorcov, oba zafarbíme na červeno.

### Zoznamy
- Počítadlá počtu osôb v učebniach v našej škole
- Štatistika počtu: priemerný, najmenší, najväčší počet osôb v učebni

---

## Úlohy

### 3.ročník

- **Čo už máš hotové:**
    - Herná postavička sa pohybuje podľa stlačených kláves od hráča
    - Neherné postavičky (NPC) sa pohybujú samostatne po predpísaných cestách
    
- **Čo robiť na dnes na seminári:**
    - Zapracovať detekciu kolízie do svojho projektu (s pomocou mentora)

- **Čo si dohodni s učiteľom:**
    - Ako bude učiteľ čiastkovo hodnotiť tvoj postup práce na projekte k 1.12.2025
    - Nižšie sú príkazy, ktoré máš využiť v svojom programe. Rozmysli kde sú jednotlivé body v tvojom zadaní projektu.
    - Max. 10 bodov a požaduje sa mať:
        - Jednofarebné pozadie alebo scénu ako vložený obrázok
        - Kreslenie obrázkov z geometrických útvarov v grafickom okne 
        - Udalosti klávesnice s nakreslenými obrázkami
        - Časovač (animácia) nehráčskych obrazcov
        - Kolízie medzi dvoma predmetmi
        - Počítanie skóre na základe úspešnej akcie
        - Predstavu čo postupne treba ďalej dokončiť (napr. v číslovaných odrážkach)
        
---

### 4.ročník

1. **Zrážky**: táto úloha má dva varianty (1.hodina zo semináru):
    - Si mentor tretiaka: Nájdi s spolu s menteem miesto v jeho projekte, kde ukážeš ako naprogramovať detekciu kolízie. Napr. zákaz pohybu cez prekážku, príchod k predmetu ho zoberie/vykoná inú akciu.
    - Si mentor štvrtáka: Vytvor pong s jednom raketou. Obdĺžník (tenisovú raketu) pri jednej strane okna budeš môcť šípkami hore a dole. Kruh (loptička) sa bude odrážať od všetkých stien okrem steny s raketou. Tam sa odrazí iba od rakety.
2. **Padajúci sneh** (2.hodina zo semináru)
    - Vytvor zoznam so súradnicami aspoň 10 vločiek, ktoré začnú padať od zhora nadol.
    - Každá vločka padá inou náhodnou rýchlosťou.
    - Pridaj "vietor", ktorý bude všetky vločky posúvať postupne vpravo.
    - **Dobrovoľný bonus za známku** (možné dokončiť najneskôr do 8.12.): Paralax efekt padania snehu s vlastnou funckiou na kreslenie vločky. Ukážka v 24:30 [https://thecodingtrain.com/tracks/snowflakes/88-snowfall](https://thecodingtrain.com/tracks/snowflakes/88-snowfall)
    
3. **Budúci týždeň písomka!:** udalosti, časovač, zoznamy

