
# Introduksjon til DOM og `getElementById` i JavaScript

## Hva er DOM?

**DOM** står for **Document Object Model** og er en representasjon av HTML-dokumentet som JavaScript kan interagere med. DOM gir deg muligheten til å manipulere innholdet på nettsiden dynamisk, som for eksempel å endre tekst, stiler, legge til eller fjerne elementer, og mer.

Når nettleseren laster en nettside, skaper den et DOM-tre basert på HTML-dokumentet. Hvert element på nettsiden, som `div`, `p`, `h1`, eller `input`, blir representert som et "node" (en node) i DOM-treet.

### Eksempel på enkel HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DOM Interaksjon</title>
</head>
<body>
    <h1 id="header">Hei, verden!</h1>
    <p id="description">Dette er et eksempel på DOM-manipulering.</p>
    <button id="changeTextButton">Endre tekst</button>
    <script src="script.js"></script>
</body>
</html>
```

I dette eksempelet har vi et `h1`-element, et avsnitt, og en knapp.

## `getElementById`

Metoden `getElementById` er en av de vanligste måtene å få tilgang til elementer i DOM-en på. Denne metoden returnerer et referanse til et HTML-element basert på dets `id`-attributt.

```javascript
// Få tilgang til h1-elementet med id="header"
let header = document.getElementById("header");

// Skriv ut innholdet (teksten) i h1-elementet
console.log(header.textContent);
```

I koden ovenfor finner vi `h1`-elementet ved hjelp av `getElementById` og skriver ut teksten i konsollen.

### Endre innhold med JavaScript

Nå som vi har tilgang til et element, kan vi endre dets innhold eller andre egenskaper.

```javascript
// Endre innholdet i h1-elementet
header.textContent = "Velkommen til DOM-manipulering!";
```

Dette vil endre teksten fra "Hei, verden!" til "Velkommen til DOM-manipulering!".

## Interaksjon med knapper

Vi kan også bruke DOM for å gjøre nettsiden mer interaktiv. La oss for eksempel endre teksten i avsnittet når knappen blir klikket.

### JavaScript for å endre tekst når knappen klikkes

```javascript
// Få tilgang til knappen og avsnittet
let button = document.getElementById("changeTextButton");
let description = document.getElementById("description");

// Legg til en funksjon som kjøres når knappen klikkes
button.addEventListener("click", function() {
    description.textContent = "Teksten har blitt endret!";
});
```

I dette eksempelet legger vi til en `click`-hendelse på knappen. Når knappen trykkes, endrer vi teksten i avsnittet.

---

## Oppgaver

### Oppgave 1: Endre overskrift med knappetrykk
Lag et HTML-dokument med en overskrift (`h1`) og en knapp. Bruk JavaScript til å endre teksten i overskriften når knappen klikkes.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Endre overskrift</title>
</head>
<body>
    <h1 id="header">Original overskrift</h1>
    <button id="changeHeaderButton">Endre overskrift</button>

    <script>
        let button = document.getElementById("changeHeaderButton");
        let header = document.getElementById("header");

        button.addEventListener("click", function() {
            header.textContent = "Ny overskrift!";
        });
    </script>
</body>
</html>
```

### Oppgave 2: Endre farge på et element
Legg til et element med tekst og bruk JavaScript til å endre fargen på teksten når en knapp trykkes.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Endre farge</title>
</head>
<body>
    <p id="text">Denne teksten skal endre farge.</p>
    <button id="changeColorButton">Endre farge</button>

    <script>
        let button = document.getElementById("changeColorButton");
        let text = document.getElementById("text");

        button.addEventListener("click", function() {
            text.style.color = "red";
        });
    </script>
</body>
</html>
```

---

Disse oppgavene gir deg grunnleggende innsikt i hvordan du kan manipulere DOM og bruke `getElementById` for å interagere med nettsiden. Dette er viktige konsepter når du begynner å lage dynamiske nettsider.
