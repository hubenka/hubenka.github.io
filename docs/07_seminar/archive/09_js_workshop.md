---
title: Workshop Javascript
slug: js-workshop
publish: false
---

## Kompletné riešenie

- Vyskúšaj si interaktívne: [Klikni sem](/seminar/js-complete.html)

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Redakčný systém časopisu</title>
        <meta charset="utf-8" />
        <style>
            body {
                display: flex;
                flex-direction: row;
                justify-content: center;
                align-items: center;
                font-family: 'Open Sans', 'Arial', 'sans';
                font-size: 12pt;
                background-color: lightblue;
            }

            main {
                width: 60%;
                margin-top: 4rem;
                background-color: white;
                padding: 4rem 6rem;
                border-radius: 10px;
            }

            h1 {
                text-align: center;
                margin-bottom: 3rem;
            }

            p {
                text-align: justify;
                line-height: 2;
            }

            #ponuka {
                display: flex;
                flex-direction: row;
                justify-content: right;
            }

            button {
                border: 1px solid gray;
                background-color: lightgreen;
                width: 8rem;
                padding: 1rem;
                cursor: pointer;
                font-weight: bold;
            }

            input {
                display: block;
                width: 100%;
                margin-top: 1rem;
                margin-bottom: 1rem;
                padding: 0.5rem;
                box-sizing: border-box;
                font-family: 'Open Sans', 'Arial', 'sans';
                font-size: 12pt;
            }

            textarea {
                width: 100%;
                height: 20rem;
                padding: 0.5rem;
                box-sizing: border-box;
                font-family: 'Open Sans', 'Arial', 'sans';
                font-size: 12pt;
            }
        </style>
    </head>
    <body>
        <main>
            <div id="ponuka">
                <button id="tlacidlo">Upraviť</button>
            </div>
            <div id="editor">
                <h1 id="nadpis">Čo je to školský parlament?</h1>
                <p id="clanok">Školský parlament je nezávislý a nestranný orgán, ktorý zastupuje záujmy voči vedeniu školy,
školskej rade a organizuje akcie. Zasadá každý mesiac. Poplatok pre žiakov na činnosť školského
parlamentu je jedno euro. Členom školského parlamentu sa môže stať každý žiak, ktorý na začiatku
školského roka bude zvolený za predsedu triedy. Pokiaľ majú žiaci nejaké výhrady, nápady alebo sťažnosti,
môžu sa obrátiť na školský parlament cez predsedu svojej triedy, koordinátora školského parlamentu,
predsedu školského parlamentu, podpredsedu školského parlamentu alebo anonymne, vhodením podnetu do urny 
umiestnenej vo vestibule školy. Školský parlament má organizačnú a odporúčaciu právomoc, ale nemá rozhodovaciu právomoc.
                </p>
            </div>
        </main>
    </body>
    <script>
        let tlacidlo = document.querySelector("#tlacidlo");

        // načítaj z nadpis a clanok local storage
        window.addEventListener("load", function() {
            let nadpis = document.querySelector("#nadpis");
            let nadpisText = localStorage.getItem("nadpis");
            if (nadpisText && nadpisText != "null") {
                nadpis.textContent = nadpisText;
            } else {
                localStorage.setItem("nadpis", nadpisText);
            }

            let clanok = document.querySelector("#clanok");
            let clanokText = localStorage.getItem("clanok");
            if (nadpisText && clanokText != "null") {
                clanok.textContent = clanokText;
            } else {
                localStorage.setItem("clanok", clanokText);
            }
        });

        // Akcia pri kliknutí na tlačidlo
        tlacidlo.addEventListener("click", function() {

            // Zmeň tlačidlo medzi upraviť a uložiť
            let btn = document.querySelector("#tlacidlo");
            if (btn.textContent == "Upraviť") {
                btn.textContent = "Uložiť";

                // Nahraď #nadpis za input
                let nadpis = document.querySelector("#nadpis");
                let nadpisEdit = document.createElement("input");
                nadpisEdit.id = "nadpis";
                nadpisEdit.type = "text";
                nadpisEdit.value = nadpis.textContent;

                // Nahraď #clanok za textarea
                let clanok = document.querySelector("#clanok");
                let clanokEdit = document.createElement("textarea");
                clanokEdit.id = "clanok";
                clanokEdit.textContent = clanok.textContent;

                // zmaž pôvodné html elementy
                nadpis.remove();
                clanok.remove();

                // vytvor nové html elementy
                let editor = document.querySelector("#editor");
                editor.appendChild(nadpisEdit);
                editor.appendChild(clanokEdit);

            } else {  // Uložiť
                btn.textContent = "Upraviť";

                // Ulož nadpis a článok do local storage
                let nadpisEdit = document.querySelector("#nadpis");
                localStorage.setItem("nadpis", nadpisEdit.value);

                let clanokEdit = document.querySelector("#clanok");
                localStorage.setItem("clanok", clanokEdit.value);

                // Namiesto nahradenia môžeme znovu načítať stránku
                // location.reload();

                // Nahraď #nadpis za h1
                let nadpis = document.createElement("h1");
                nadpis.id = "nadpis";
                nadpis.textContent = nadpisEdit.value;

                // Nahraď #clanok za p
                let clanok = document.createElement("p");
                clanok.id = "clanok";
                clanok.textContent = clanokEdit.value;

                // zmaž pôvodné html elementy
                nadpisEdit.remove();
                clanokEdit.remove();

                // vytvor nové html elementy
                let editor = document.querySelector("#editor");
                editor.appendChild(nadpis);
                editor.appendChild(clanok);
            }
        });
    </script>
</html>
```


## Zadanie úlohy
Predloha pre stránku, do ktorej pridáme úpravu textu a ponechanie zmeneného textu po obnovení stránky

- Vyskúšaj si interaktívne: [Klikni sem](/seminar/js-assignment.html)

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Redakčný systém časopisu</title>
        <meta charset="utf-8" />
        <style>
            body {
                display: flex;
                flex-direction: row;
                justify-content: center;
                align-items: center;
                font-family: 'Open Sans', 'Arial', 'sans';
                font-size: 12pt;
                background-color: lightblue;
            }

            main {
                width: 60%;
                margin-top: 4rem;
                background-color: white;
                padding: 4rem 6rem;
                border-radius: 10px;
            }

            h1 {
                text-align: center;
                margin-bottom: 3rem;
            }

            p {
                text-align: justify;
                line-height: 2;
            }

            #ponuka {
                display: flex;
                flex-direction: row;
                justify-content: right;
            }

            button {
                border: 1px solid gray;
                background-color: lightgreen;
                width: 8rem;
                padding: 1rem;
                cursor: pointer;
                font-weight: bold;
            }

            input {
                display: block;
                width: 100%;
                margin-top: 1rem;
                margin-bottom: 1rem;
                padding: 0.5rem;
                box-sizing: border-box;
                font-family: 'Open Sans', 'Arial', 'sans';
                font-size: 12pt;
            }

            textarea {
                width: 100%;
                height: 20rem;
                padding: 0.5rem;
                box-sizing: border-box;
                font-family: 'Open Sans', 'Arial', 'sans';
                font-size: 12pt;
            }
        </style>
    </head>
    <body>
        <main>
            <div id="ponuka">
                <button id="tlacidlo">Upraviť</button>
            </div>
            <div id="editor">
                <h1 id="nadpis">Čo je to školský parlament?</h1>
                <p id="clanok">Školský parlament je nezávislý a nestranný orgán, ktorý zastupuje záujmy voči vedeniu školy,
školskej rade a organizuje akcie. Zasadá každý mesiac. Poplatok pre žiakov na činnosť školského
parlamentu je jedno euro. Členom školského parlamentu sa môže stať každý žiak, ktorý na začiatku
školského roka bude zvolený za predsedu triedy. Pokiaľ majú žiaci nejaké výhrady, nápady alebo sťažnosti,
môžu sa obrátiť na školský parlament cez predsedu svojej triedy, koordinátora školského parlamentu,
predsedu školského parlamentu, podpredsedu školského parlamentu alebo anonymne, vhodením podnetu do urny
umiestnenej vo vestibule školy. Školský parlament má organizačnú a odporúčaciu právomoc, ale nemá rozhodovaciu právomoc.
                </p>
            </div>
        </main>
    </body>
</html>
```
