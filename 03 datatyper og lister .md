
# Introduksjon til datatyper og lister i JavaScript

JavaScript har forskjellige datatyper som lar deg jobbe med ulike typer informasjon. For å bli komfortabel med JavaScript-programmering er det viktig å forstå disse datatypene og hvordan de brukes.

## 1. Primitive datatyper
JavaScript har seks primitive datatyper:

- **Number**: Representerer tall, både heltall og desimaltall.
  ```javascript
  let age = 30;
  let pi = 3.14;
  ```

- **String**: Brukes til å representere tekst.
  ```javascript
  let name = "Ola Nordmann";
  ```

- **Boolean**: Har bare to mulige verdier: `true` eller `false`.
  ```javascript
  let isStudent = true;
  ```

- **Null**: Representerer en tom eller ikke-eksisterende verdi.
  ```javascript
  let emptyValue = null;
  ```

- **Undefined**: En variabel som er deklarert, men ikke tildelt noen verdi, har verdien `undefined`.
  ```javascript
  let notAssigned;
  ```

- **Symbol**: En spesiell, unik datatype som brukes sjeldnere.

## 2. Arrays (Lister)
En array er en samling av flere verdier i én variabel. Dette gjør det lettere å lagre og jobbe med flere relaterte verdier samtidig. Arrays kan inneholde alle typer data, inkludert andre arrays.

```javascript
let fruits = ["Eple", "Banan", "Appelsin"];
```

### Tilgang til elementer
Du kan få tilgang til elementene i en array ved å bruke deres indeks (posisjon). Indeksering starter på 0 i JavaScript.

```javascript
console.log(fruits[0]);  // "Eple"
console.log(fruits[2]);  // "Appelsin"
```

### Legge til elementer
Du kan legge til nye elementer i en array ved å bruke metoder som `push()`.

```javascript
fruits.push("Mango");  // Legger til "Mango" på slutten
```

### Fjerne elementer
For å fjerne det siste elementet i en array, kan du bruke `pop()`.

```javascript
fruits.pop();  // Fjerner "Mango"
```

### Lengde på array
`length`-egenskapen gir deg antall elementer i en array.

```javascript
console.log(fruits.length);  // Antall elementer i arrayen
```

---

## Oppgaver

### Oppgave 1: Primitive datatyper
Lag variabler for følgende:
- Et tall som representerer alderen din.
- En streng som representerer navnet ditt.
- En boolean som representerer om du er student eller ikke.
Skriv dem ut i konsollen.

```javascript
// Oppgave 1
let age = 25;
let name = "Ola Nordmann";
let isStudent = true;

console.log(age);
console.log(name);
console.log(isStudent);
```

### Oppgave 2: Enkle array-operasjoner
Lag en array med tre av dine favorittfrukter. Skriv ut den første og den siste frukten i arrayen.

```javascript
// Oppgave 2
let fruits = ["Eple", "Banan", "Appelsin"];

console.log(fruits[0]);  // Første frukt
console.log(fruits[fruits.length - 1]);  // Siste frukt
```

### Oppgave 3: Legge til og fjerne elementer i en array
Bruk `push()` til å legge til en ny frukt i arrayen. Bruk deretter `pop()` til å fjerne den siste frukten. Skriv ut arrayen etter begge operasjoner.

```javascript
// Oppgave 3
let fruits = ["Eple", "Banan", "Appelsin"];

fruits.push("Mango");  // Legger til Mango
console.log(fruits);

fruits.pop();  // Fjerner Mango
console.log(fruits);
```

### Oppgave 4: Bruk av forskjellige datatyper
Lag en array som inneholder ulike datatyper (for eksempel et tall, en streng, og en boolean). Skriv ut hvert element i arrayen ved å bruke en for-løkke.

```javascript
// Oppgave 4
let mixedArray = [25, "Ola Nordmann", true];

for (let i = 0; i < mixedArray.length; i++) {
  console.log(mixedArray[i]);
}
```

---

Disse oppgavene vil hjelpe deg å forstå hvordan datatyper og arrays fungerer i JavaScript. Arrays er et kraftig verktøy som lar deg jobbe med flere verdier samtidig, og ved å kombinere dem med primitive datatyper kan du lage mer dynamisk kode.
