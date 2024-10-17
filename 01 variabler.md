
# Introduksjon til variabler i JavaScript

En variabel i JavaScript brukes til å lagre verdier som kan gjenbrukes senere i koden din. Det finnes flere måter å definere variabler på i JavaScript: `var`, `let`, og `const`.

## 1. `var`:
- Dette er den eldste måten å definere variabler på i JavaScript.
- En variabel deklarert med `var` kan endres (reassignes) senere.
- `var` har **funksjonsscope**, noe som betyr at den er tilgjengelig innenfor hele funksjonen den er deklarert i.

```javascript
var name = "John";
console.log(name);  // Output: John
name = "Jane";
console.log(name);  // Output: Jane
```

## 2. `let`:
- `let` ble introdusert i nyere versjoner av JavaScript (ES6/ES2015).
- Variabler deklarert med `let` kan endres (reassignes) senere, men har **blokkscope**, noe som betyr at de bare er tilgjengelige innenfor blokken de er definert i.

```javascript
let age = 30;
console.log(age);  // Output: 30
age = 31;
console.log(age);  // Output: 31
```

## 3. `const`:
- `const` brukes når du vil definere en konstant, det vil si en variabel som ikke kan endres.
- `const` har også **blokkscope**, akkurat som `let`.
- Selv om verdien ikke kan endres, kan objekter eller arrayer deklarert med `const` få endret innholdet sitt.

```javascript
const country = "Norway";
console.log(country);  // Output: Norway
// country = "Sweden";  // Dette vil gi en feil, siden const ikke kan reassignes.
```

---

## Oppgaver

### Oppgave 1: Enkel variabelbruk
Definer tre variabler: `firstName`, `lastName`, og `age`. Gi dem verdier og skriv dem ut i konsollen.


### Oppgave 2: Endre variabler
Lag en variabel `favoriteColor` med `let`. Gi den en verdi og skriv den ut. Endre så verdien av variabelen og skriv ut den nye verdien.


### Oppgave 3: Bruk av `const`
Definer en konstant `PI` med verdien 3.14. Prøv deretter å endre verdien og observer hva som skjer.


### Oppgave 4: Variabelscope
Skriv et program som definerer en variabel med `let` innenfor en blokk (for eksempel en `if`-setning) og prøv å bruke variabelen utenfor blokken. Hva skjer?


### Oppgave 5: Bonusoppgave – Enkel kalkulator
Lag to variabler, `num1` og `num2`, med tallverdier. Lag variabler for summen, differansen, produktet, og kvotienten av disse tallene. Skriv resultatene ut i konsollen.


---

Disse oppgavene gir en god start for å forstå hvordan variabler fungerer i JavaScript. Variabler er en viktig del av all programmering, så det er viktig å øve seg på å bruke dem på riktig måte!
