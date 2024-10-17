
# Introduksjon til datatyper og lister i JavaScript

Når vi programmerer, må vi ofte holde styr på forskjellige typer informasjon. I JavaScript finnes det flere **datatyper** som lar oss jobbe med tall, tekst og mer. Å forstå disse typene er viktig for å kunne lage god kode. 

## 1. Primitive datatyper
JavaScript har seks primitive datatyper:

- **Number**: Brukes for tall, enten de er heltall (som 5) eller desimaltall (som 3.14).
  ```javascript
  let age = 30;
  let pi = 3.14;
  ```

- **String**: Brukes for tekst. Teksten må være inni anførselstegn (enten `""` eller `''`)
  ```javascript
  let name = "Ola Nordmann";
  ```

- **Boolean**: Brukes for verdier som er enten `true` (sant) eller `false` (usant).
  ```javascript
  let isStudent = true;
  ```

- **Null**: Representerer en tom eller ikke-eksisterende verdi.
  ```javascript
  let emptyValue = null;
  ```

- **Undefined**: Brukes når en variabel er deklarert, men ikke tildelt noen verdi ennå.
  ```javascript
  let notAssigned;
  ```

- **Symbol**: En spesiell, unik datatype som brukes sjeldnere.

## 2. Arrays (Lister)
En **array** er en samling av flere verdier i én variabel. Dette gjør det letter å jobbe med flere verdier på én gang. Arrays kan inneholde alle typer data, inkludert andre arrays.

```javascript
let fruits = ["Eple", "Banan", "Appelsin"];
```

### Tilgang til elementer i en array
For å hente ut et element fra en array, bruker vi dets **indeks** (posisjon). Indeksering starter alltid på 0.

```javascript
console.log(fruits[0]);  // Henter ut "Eple" som er det første elementet
console.log(fruits[2]);  // Henter ut "Appelsin" som er det tredje elementet
```

### Legge til elementer i en array
For å legge til nye elementer på slutten av en array, bruker vi `push()`-metoden.

```javascript
fruits.push("Mango");  // Legger til "Mango" på slutten
console.log(fruits);  
```

### Fjerne elementer
For å fjerne det siste elementet i en array, bruker vi pop()-metoden.

```javascript
fruits.pop();  // Fjerner "Mango"
console.log(fruits);
```

### Lengden på en array
For å finne ut hvor mange elementer det er i en array, bruker vi length-egenskapen.

```javascript
console.log(fruits.length);  // Viser antall elementer i arrayen
```

---

## Oppgaver

### Oppgave 1: Primitive datatyper
Lag variabler som representerer følgende:
- Din alder som et tall
- Navnet ditt som en tekstreng
- Om du er student eller ikke som en boolean

Skriv disse variablene ut i konsollen.

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
Lag en array som inneholder tre av dine favorittfrukter. Skriv ut den første og den siste frukten i arrayen.

```javascript
// Oppgave 2
let fruits = ["Eple", "Banan", "Appelsin"];

console.log(fruits[0]);  // Første frukt
console.log(fruits[fruits.length - 1]);  // Siste frukt
```

### Oppgave 3: Legge til og fjerne elementer i en array
Bruk push() til å legge til en ny frukt til arrayen. Bruk deretter pop() til å fjerne den siste frukten. Skriv ut arrayen etter begge operasjonene.

```javascript
// Oppgave 3
let fruits = ["Eple", "Banan", "Appelsin"];

fruits.push("Mango");  // Legger til Mango
console.log(fruits);

fruits.pop();  // Fjerner Mango
console.log(fruits);
```

### Oppgave 4: Kombinere datatyper i en array
Lag en array som inneholder forskjellige datatyper (f.eks. et tall, en streng, og en boolean). Bruk en for-løkke til å skrive ut hvert element i arrayen.

```javascript
// Oppgave 4
let mixedArray = [25, "Ola Nordmann", true];

for (let i = 0; i < mixedArray.length; i++) {
  console.log(mixedArray[i]);
}
```

---

Disse oppgavene gir deg en god forståelse av hvordan ulike datatyper og arrays fungerer i JavaScript. Arrays er en kraftig måte å holde styr på flere verdier på én gang, og når du kombinerer dem med de primitive datatypene, kan du lage mer komplekse og dynamiske programmer.