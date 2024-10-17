
# Introduksjon til funksjoner i JavaScript

Funksjoner i JavaScript lar deg organisere og gjenbruke kode ved å definere et sett med instruksjoner som kan kjøres senere. Funksjoner gjør det lettere å strukturere koden og gjøre den mer lesbar og vedlikeholdbar.

> Funksjoner i JavaScript er som små oppskrifter. Du skriver en oppskrift én gang, og så kan du bruke den igjen og igjen, akkurat når du trenger den. 

## 1. Definere en funksjon

For å lage en funksjon bruker vi nøkkelordet `function`, etterfulgt av et navn vi gir funksjonen. Inni funksjonen skriver vi det vi vil at den skal gjøre.

```javascript
function greet() {
  console.log("Hei, verden!");
}
```

I dette eksempelet heter funksjonen `greet`. Hver gang vi kaller på `greet`, vil den skrive ut "Hei, verden!" i konsollen.

## 2. Kalle en funksjon
For å bruke en funksjon, må vi kalle den ved å skrive funksjonsnavnet etterfulgt av parenteser ().

```javascript
greet();  // Kaller funksjonen og den skriver "Hei, verden!"
```

## 3. Funksjoner med parametere
Funksjoner kan ta inn parametere, som er verdier som sendes inn i funksjonen når den kalles. Parametere gir funksjoner mulighet til å utføre handlinger basert på data de mottar.

```javascript
function greetPerson(name) {
  console.log("Hei, " + name + "!");
}

greetPerson("Ola");  // Output: "Hei, Ola!"
```

Her tar funksjonen `greetPerson` et parameter kalt `name`, og den skriver ut en personlig melding basert på hva vi sender inn. Når vi kaller funksjonen med "Ola", skriver den ut "Hei, Ola!".

## 4. Returnere verdier
Funksjoner kan også *returnere* (gi tilbake) en verdi. Dette er nyttig hvis vi vil bruke resultatet av funksjonen til noe senere i koden.

```javascript
function add(a, b) {
  return a + b;
}

let sum = add(5, 3);  // Funksjonen returnerer 8, som vi lagrer i variabelen `sum`
console.log(sum);  // Output: 8
```

## 5. Funksjonsuttrykk
En funksjon kan også lagres i en variabel. Dette kalles et funksjonsuttrykk.

```javascript
let greet = function() {
  console.log("Hei, verden!");
};

greet();  // Kaller funksjonen
```
I dette eksempelet er funksjonen lagret i variabelen `greet`, og vi kan bruke den på samme måte som andre funksjoner.

---

## Oppgaver

### Oppgave 1: En enkel funksjon
Lag en funksjon `sayHello`, som skriver ut "Hei, verden!" når den kalles. Kall funksjonen for å se resultatet.

```javascript
// Oppgave 1
function sayHello() {
  console.log("Hei, verden!");
}

sayHello();  // Kall funksjonen
```

### Oppgave 2: Funksjoner med parametere
Lag en funksjon `greetPerson`, som tar et navn som parameter og skriver ut "Hei, [navn]!". Kall funksjonen med ditt eget navn.

```javascript
// Oppgave 2
function greetPerson(name) {
  console.log("Hei, " + name + "!");
}

greetPerson("Ola");  // Kall funksjonen med ditt navn
```

### Oppgave 3: Funksjoner som returnerer verdier
Skriv en funksjon `multiply` som tar to tall som parametere og returnerer produktet av dem. Kall funksjonen og skriv ut resultatet.

```javascript
// Oppgave 3
function multiply(a, b) {
  return a * b;
}

let result = multiply(4, 5);
console.log(result);  // Output: 20
```

### Oppgave 4: Funksjonsuttrykk
Skriv en funksjon som lagres i en variabel `sayGoodbye`, som skriver ut "Ha det bra!" når den kalles.

```javascript
// Oppgave 4
let sayGoodbye = function() {
  console.log("Ha det bra!");
};

sayGoodbye();  // Kall funksjonen
```

---

Disse oppgavene vil hjelpe deg å forstå hvordan funksjoner fungerer i JavaScript. Ved å bruke funksjoner kan du gjenbruke kode og gjøre programmene dine mer effektive og ryddige.