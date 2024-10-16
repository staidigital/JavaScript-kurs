
# Flere Selectors og Manipulering av CSS med JavaScript

I JavaScript finnes det mange måter å hente ut elementer fra HTML-en. Vi kan bruke ulike selectors (velgere) for å få tak i elementene vi vil jobbe med, og deretter kan vi dynamisk endre stilene deres ved hjelp av JavaScript.

## 1. Flere Selectors

### `getElementsByClassName`
Denne metoden returnerer en samling av alle elementer som har en gitt klasse. Siden den returnerer en samling (HTMLCollection), må du bruke en løkke for å endre stil på hvert enkelt element.

```javascript
let elements = document.getElementsByClassName("myClass");

for (let i = 0; i < elements.length; i++) {
  elements[i].style.color = "blue";
}
```

### `getElementsByTagName`
Denne metoden returnerer en samling av alle elementer med et bestemt HTML-tag. For eksempel kan du velge alle `p`-elementene på en side.

```javascript
let paragraphs = document.getElementsByTagName("p");

for (let i = 0; i < paragraphs.length; i++) {
  paragraphs[i].style.fontSize = "18px";
}
```

### `querySelector` og `querySelectorAll`
`querySelector` returnerer det **første** elementet som samsvarer med en gitt CSS-selektor, mens `querySelectorAll` returnerer **alle** elementene som samsvarer med selektoren som en NodeList.


```javascript
// Velg det første elementet med klassen "myClass"
let element = document.querySelector(".myClass");
element.style.backgroundColor = "yellow";

// Velg alle elementer med klassen "myClass"
let allElements = document.querySelectorAll(".myClass");

allElements.forEach(function(el) {
  el.style.border = "2px solid red";
});
```

## 2. Manipulering av CSS med JavaScript

### Endre CSS med `style`-egenskapen
Vi kan bruke `style`-egenskapen i JavaScript til å direkte endre CSS-stiler på et element, som for eksempel farge, størrelse, marginer, eller bakgrunn.


```javascript
let element = document.getElementById("myElement");
element.style.color = "green";
element.style.backgroundColor = "lightgrey";
```

### Legge til og fjerne klasser med `classList`
`classList` lar deg legge til, fjerne eller toggle (veksle) mellom CSS-klasser på et element. Dette er spesielt nyttig hvis du har forhåndsdefinerte CSS-klasser du ønsker å aktivere eller deaktivere.

```javascript
let element = document.getElementById("myElement");

// Legg til en klasse
element.classList.add("highlight");

// Fjern en klasse
element.classList.remove("highlight");

// Veksle en klasse
element.classList.toggle("highlight");
```

## Oppgaver

### Oppgave 1: Endre stil på flere elementer
Bruk `getElementsByClassName` for å velge alle elementer med en bestemt klasse, og endre fargen på teksten deres.


### Oppgave 2: Bruk `querySelectorAll` til å velge elementer
Bruk `querySelectorAll` for å velge alle `div`-elementer, og legg til en rød kant rundt dem når en knapp trykkes.


### Oppgave 3: Endre klasser med `classList`
Bruk `classList` til å veksle en klasse som endrer bakgrunnsfargen på et element.


---

Disse oppgavene vil hjelpe deg å forstå hvordan du kan bruke forskjellige selectors for å hente ut elementer fra DOM, samt hvordan du kan endre stiler dynamisk ved hjelp av JavaScript. Dette er viktige ferdigheter for å lage interaktive nettsider.