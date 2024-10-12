
# Introduksjon til løkker i JavaScript

Løkker lar deg kjøre samme kode flere ganger uten å skrive den flere ganger manuelt. Dette er veldig nyttig når du ønsker å utføre en handling gjentatte ganger, for eksempel iterere gjennom elementer i et array eller telle opp til et visst tall.

## 1. For-løkker (for-loops)
For-løkker brukes ofte når du vet hvor mange ganger du vil at en handling skal gjentas. Løkken består av tre deler: en startverdi, en betingelse, og en oppdatering.

```javascript
for (let i = 0; i < 5; i++) {
  console.log("Dette er iterasjon nummer " + i);
}
```

I dette eksempelet:
- `let i = 0` setter startverdien til variabelen `i`.
- `i < 5` er betingelsen som kontrollerer når løkken skal stoppe. Så lenge `i` er mindre enn 5, vil koden kjøre.
- `i++` oppdaterer variabelen `i` med 1 for hver iterasjon.

## 2. While-løkker (while-loops)
En while-løkke kjører så lenge en betingelse er sann. Denne typen løkke brukes når du ikke nødvendigvis vet hvor mange ganger løkken skal kjøre på forhånd.

```javascript
let i = 0;
while (i < 5) {
  console.log("Dette er iterasjon nummer " + i);
  i++;
}
```

I dette eksempelet vil løkken kjøre så lenge `i` er mindre enn 5. Hver gang løkken kjører, økes `i` med 1.

## 3. Do-while-løkker
En do-while-løkke ligner på en while-løkke, men med én stor forskjell: koden vil alltid kjøre minst én gang, selv om betingelsen ikke er oppfylt.

```javascript
let i = 0;
do {
  console.log("Dette er iterasjon nummer " + i);
  i++;
} while (i < 5);
```

Her vil løkken kjøre minst én gang før betingelsen sjekkes.

---

## Oppgaver

### Oppgave 1: Tell opp fra 1 til 10
Bruk en for-løkke til å skrive ut tallene fra 1 til 10 i konsollen.

```javascript
// Oppgave 1
for (let i = 1; i <= 10; i++) {
  console.log(i);
}
```

### Oppgave 2: Finn summen av tallene fra 1 til 100
Skriv et program som bruker en while-løkke for å finne summen av alle tall fra 1 til 100.

```javascript
// Oppgave 2
let sum = 0;
let i = 1;
while (i <= 100) {
  sum += i;
  i++;
}
console.log("Summen av tallene fra 1 til 100 er: " + sum);
```

### Oppgave 3: Skriv ut et array
Lag et array med navnene på noen byer. Bruk en for-løkke til å skrive ut hver by i konsollen.

```javascript
// Oppgave 3
let cities = ["Oslo", "Bergen", "Trondheim", "Stavanger"];
for (let i = 0; i < cities.length; i++) {
  console.log(cities[i]);
}
```

### Oppgave 4: Finn det største tallet
Lag et array med tall. Bruk en for-løkke til å finne det største tallet i arrayet.

```javascript
// Oppgave 4
let numbers = [5, 12, 8, 20, 3];
let largest = numbers[0];
for (let i = 1; i < numbers.length; i++) {
  if (numbers[i] > largest) {
    largest = numbers[i];
  }
}
console.log("Det største tallet er: " + largest);
```

---

Disse oppgavene vil hjelpe deg å forstå hvordan løkker fungerer i JavaScript. Øving på bruk av for-løkker, while-løkker og do-while-løkker vil gjøre deg tryggere på hvordan du kan automatisere gjentatte oppgaver i koden din.
