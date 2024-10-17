
# Introduksjon til variabler i JavaScript
I JavaScript (og i programmering generelt) bruker vi **variabler** for å lagre informasjon som vi kan bruke senere. Det kan være et tall, et ord eller andre typer data.

Vi kan definere variabler på tre hovedmåter i JavaScript: `var`, `let` og `const`. 

## 1. `var` - den gamle måten
-  `var` er den eldste måten å deklarere variabler på i JavaScript og ble brukt mye før rundt 2015.
- En variabel deklarert med `var` kan endres (reassignes) senere.
- `var` har **funksjonsscope**, noe som betyr at den kan brukes overalt innenfor funksjonen den er deklarert i. 

```javascript
var name = "John";
console.log(name);  // Output: John
name = "Jane";
console.log(name);  // Output: Jane
```

## 2. `let` - den moderne måten
- `let` ble introdusert i en nyere versjon av JavaScript (ES6/ES2015).
- En variabel deklarert med `let` kan også endres, men den kan bare brukes i den spesifikke blokken (f.eks. en `if`-setning) den er laget i. Dette kalles **blokkscope**.
- `let` er den **anbefalte** måten å deklarere variabler på i moderne JavaScript.

```javascript
let age = 30;
console.log(age);  // Output: 30
age = 31;
console.log(age);  // Output: 31
```

## 3. `const` - for noe som ikke skal endres
- `const` er perfekt når du vil lage en variabel som ikke skal endres.
- Når du har definert en konstant, kan du ikke endre verdien senere.
- `const` har også **blokkscope**, akkurat som `let`.

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
Lag en variabel `favoriteColor` med `let`. Gi den en verdi og skriv den ut. ndre så verdien av variabelen og skriv ut den nye verdien.


### Oppgave 3: Bruk av `const`
Definer en konstant `PI` med verdien 3.14. Prøv å endre verdien (spoiler: det vil ikke fungere!). Hva skjer?


### Oppgave 4: Variabelscope
Definer en variabel med `let` inne i en `if`-setning. Forsøk å bruke den utenfor `if`-setningen. Hva skjer?


### Oppgave 5: Bonusoppgave – Lag en kalkulator
Lag to variabler, `num1` og `num2`, og gjør noen enkle berekninger med dem. Skriv ut summen, differansen, produktet og kvotienten i konsollen. 


---

Disse oppgavene hjelper deg å forstå hvordan variabler fungerer i JavaScript. Husk at variabler er en av de viktigste delene av programmering, så det er viktig å øve på dem på riktig måte. Lykke til! 🚀

