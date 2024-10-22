
# Introduksjon til DOM og `getElementById` i JavaScript

## Hva er DOM?

**DOM** står for **Document Object Model** og er en måte for å "se" og "interagere" med HTML-dokumentet. Med DOM får du muligheten til å endre ting på nettsiden dynamisk, som å endre tekst, farger, legge til eller fjerne elementer.

Når nettleseren laster en nettside, lager den et DOM-tre basert på HTML-en. Hvert element på nettsiden (som `div`, `p`, `h1`) blir en "node" i dette treet, som JavaScript kan endre.

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

I dette eksempelet har vi en overskrift (`h1`), et avsnitt (`p`), og en knapp (`button`). 

## Hva gjør `getElementById`

Metoden `getElementById` lar oss få tak i et bestemt HTML-element ved å bruke dets id-attributt. Når vi har fått tak i elementet, kan vi gjøre hva vi vil med det, som å endre tekst, farger eller andre stiler.

```javascript
// Få tilgang til h1-elementet med id="header"
let header = document.getElementById("header");

// Skriv ut innholdet (teksten) i h1-elementet
console.log(header.textContent);
```

Her får vi tak i overskriften (h1) ved hjelp av getElementById og skriver ut teksten som er inni overskriften.

### Endre innhold med JavaScript

Nå som vi har tilgang til et element, kan vi endre dets innhold eller stil.

```javascript
// Endre innholdet i h1-elementet
header.textContent = "Velkommen til DOM-manipulering!";
```

Dette vil endre teksten fra "Hei, verden!" til "Velkommen til DOM-manipulering!".

## Interaksjon med knapper

Vi kan også bruke DOM for å gjøre nettsiden mer interaktiv. For eksempel kan vi endre tekst når en knapp trykkes.

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

I dette eksempelet legger vi til en `click`-hendelse på knappen. Når knappen trykkes, endrer vi teksten i avsnittet til "Teksten har blitt endret!".

---

## Oppgaver

### Oppgave 1: Endre overskrift med knappetrykk
Lag et HTML-dokument med en overskrift (`h1`) og en knapp. Bruk JavaScript til å endre teksten i overskriften når knappen klikkes.


### Oppgave 2: Endre farge på et element
Legg til et element med tekst og bruk JavaScript til å endre fargen på teksten når en knapp trykkes.

---

Disse oppgavene gir deg grunnleggende innsikt i hvordan du kan manipulere DOM og bruke `getElementById` for å interagere med nettsiden. Dette er viktige konsepter når du begynner å lage dynamiske nettsider.
