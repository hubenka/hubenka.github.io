---
title: Cvičenia
publish: true
---

1. Nájdite na internete dve počítačové zostavy (2xPC/2xNotebook) do 500 eur, ktoré porovnáte a vypíšte najdôležitejšie parametre pre jednotlivé komponenty (Cena PC, Obrázok PC, CPU, RAM, GPU, Externý disk, Konektory). Písomne zdôvodnite, ktorý z nich je lepší a ktorý by ste si kúpili vy osobne a prečo. Úlohu odovzdajte ako odt/docx/pdf z Wordu.

2. Vytvorte prezentáciu ohľadom určitej oblasti alebo éry z histórie počítačov alebo o konkrétnom harvéri. Presná téma je na vás podľa toho čo vás najviac zaujalo. Min. rozsah je 5 - 8 slidov samotného obsahu. Odovzadajte v jednom z formátov: ppt/pptx/odp/pdf.

3. Vytvorte prezentáciu o okruhu z histórie počítačov, ktorý vás najviac zaujal. Rozsah 5 - 8 slidov. Odovzdajte v pdf/ppt/pptx/odp.

4. Premyslite si okolnosti do pozvánky pre fiktívne vianočné podujatie (večierok, akadémia, kapustnica, trhy, ...).

5. Do dokumentu vo worde vložte tabuľky kalórií, ktoré ste si pripravili v exceli. V takto prepojenej tabuľke vypočítajte súčet kalórií za každý deň zvlášť, zvýraznite hlavičky podfarbením a tučným písmom. Vyberte jednotný rez a veľkosť písma.

6. Z vášho mena a priezviska (bez diakritiky a prechyľovania) si vytvorte 2 čísla v desiatkovej sústave, sčítaním poradia týchto písmen v abecede. Premente čísla do binárnej a hexadecimálnej sústavy. Do riešenia úlohy napíšte meno, priezvisko, ktoré ste premieňali a všetky vypočítané čísla.

7. Rozvrhnite a naformátujte vo Worde tabuľku podľa predlohy "predaj zeleninára".

8. V súbore laboratorna-praca.docx nahraďte text, ktorý vyzerá ako rovnica, vložením word-ovských vzorcov alebo rovníc.

9. Pozri https://opendata.bratislava.sk. Vyber si odtiaľ vhodnú tabuľku a v MS Excel z nej vytvor kontingenčnú tabuľku. A k nej jednoduchý graf.

10. Nakreslite korytnačkou v Pythone 10 domčekov vedľa seba. Každý domček má inú náhodnú farbu. Použite for cyklus.
Prehľad príkazov: https://www.stechies.com/turtle-graphics-python/

11. Vytvor program v Pythone s Turtle na nakreslenie hracej dosky Človeče. Využi for cyklus.

12. Napíš program, ktorý bude v animácii posúvať po obrazovke predmet zložený z viacerých geometrických útvarov (postavička). Predmet sa posúva po obrazovke zľava doprava a keď príde za pravý okraj obrazovky objaví sa znova z ľavého okraja obrazovky.

13. Napíš program v Pythone (s tkinter), ktorý po kliknutí myšou na dve miesta na obrazovke (príkaz bind_all na "Button-1") nakreslí medzi týmito bodmi obdĺžnik. Umožnite kreslenie ľubovoľného počtu obdĺžnikov (keď skončím kreslenie jedného, môžem vyznačiť body pre druhý). Skúste vytváraný obdĺžnik aj priebežne prekreslovať pomocou príkazu delete("all") a udalosti "Motion". Postup:
    - Po kliknutí na prvú pozíciu si zapíšem súradnice kliknutia: event.x, event.y (vo funkcii treba použiť: global x, y)
    - Po kliknutí na druhú pozíciu nakreslím obdĺžnik medzi aktuálnymi súradnicami kliknutia: event.x, event.y a zapísanými x, y. Sledovať, či ide o prvú alebo druhú pozíciu môžem napr. logickou premennou: kreslenie = False, kreslenie = True.

14. Pridajte do programu z hodiny kreslenie pohybu postavičky namiesto kruhu. Zároveň nakreslite do grafickej plochy obdĺžnik (napr. krabica). Zabezpečte, aby postavička nemohla prejsť cez obdĺžnik (collision detection)