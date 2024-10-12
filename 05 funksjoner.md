
# Introduksjon til funksjoner i JavaScript

Funksjoner i JavaScript lar deg organisere og gjenbruke kode ved å definere et sett med instruksjoner som kan kjøres senere. Funksjoner gjør det lettere å strukturere koden og gjøre den mer lesbar og vedlikeholdbar.

## 1. Definere en funksjon
En funksjon defineres ved hjelp av nøkkelordet `function`, etterfulgt av et navn, en liste med parametere (valgfritt), og en blokk med kode som skal utføres når funksjonen kalles.

```javascript
function greet() {
  console.log("Hei, verden!");
}
```

Her er `greet` funksjonens navn, og når funksjonen kalles, vil den skrive "Hei, verden!" i konsollen.

## 2. Kalle en funksjon
For å kjøre koden i en funksjon må den kalles ved hjelp av funksjonsnavnet etterfulgt av parenteser.

```javascript
greet();  // Kaller funksjonen
```

## 3. Funksjoner med parametere
Funksjoner kan ta inn parametere, som er verdier som sendes inn i funksjonen når den kalles. Parametere gir funksjoner mulighet til å utføre handlinger basert på data de mottar.

```javascript
function greetPerson(name) {
  console.log("Hei, " + name + "!");
}

greetPerson("Ola");  // Output: "Hei, Ola!"
```

I dette eksempelet tar funksjonen `greetPerson` et parameter, `name`, og bruker det til å tilpasse meldingen som skrives ut.

## 4. Returnere verdier
En funksjon kan returnere en verdi ved hjelp av `return`-nøkkelordet. Når funksjonen returnerer en verdi, kan den brukes senere i koden.

```javascript
function add(a, b) {
  return a + b;
}

let sum = add(5, 3);  // sum får verdien 8
console.log(sum);  // Output: 8
```

## 5. Funksjonsuttrykk
I JavaScript kan funksjoner også lagres i variabler. Dette kalles funksjonsuttrykk.

```javascript
let greet = function() {
  console.log("Hei, verden!");
};

greet();  // Kaller funksjonen
```

---

## Oppgaver

### Oppgave 1: En enkel funksjon
Lag en funksjon `sayHello` som skriver ut "Hei, verden!" når den kalles. Kall funksjonen for å se resultatet.

```javascript
// Oppgave 1
function sayHello() {
  console.log("Hei, verden!");
}

sayHello();  // Kall funksjonen
```

### Oppgave 2: Funksjoner med parametere
Lag en funksjon `greetPerson` som tar et navn som parameter og skriver ut "Hei, [navn]!". Kall funksjonen med ditt eget navn.

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
Skriv en funksjon som lagres i en variabel `sayGoodbye`, og som skriver ut "Ha det bra!" når den kalles.

```javascript
// Oppgave 4
let sayGoodbye = function() {
  console.log("Ha det bra!");
};

sayGoodbye();  // Kall funksjonen
```

---

Disse oppgavene vil hjelpe deg å forstå hvordan funksjoner fungerer i JavaScript. Funksjoner gjør det enklere å gjenbruke kode og strukturere programmet på en måte som gjør det mer vedlikeholdbart.
