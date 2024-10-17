
# Introduksjon til if-setninger i JavaScript

Nå som du har lært om variabler, er det tid for å lære hvordan vi kan få koden til å ta beslutninger. Dette gjør vi med `if`-setninger. `if`-setninger hjelper datamaskinen med å gjøre noe kun når en bestemt betingelse er oppfylt, som om vi sier "hvis dette skjer, gjør dette". 

## Grunnleggende if-setning:
En if-setning sjekker om noe er sant. Hvis det er sant, kjører den koden inne i klammeparentesene `{}`.

```javascript
let age = 18;

if (age >= 18) {
  console.log("Du er myndig.");
}
```

I dette eksempelet sjekker if-setningen om `age` er større enn eller lik 18. Hvis det er sant, vil den skrive ut "Du er myndig."

## If-else-setning:

Noen ganger vil vi gjøre noe annet hvis betingelsen ikke er sann. Da bruker vi en `else`-setning, som betyr "ellers". 

```javascript
let age = 16;

if (age >= 18) {
  console.log("Du er myndig.");
} else {
  console.log("Du er ikke myndig.");
}
```

Her sjekker vi om `age` er større enn eller lik 18. Hvis det er **sant** skriver den ut "Du er myndig". Hvis det er **usant** skriver den ut "Du er ikke myndig." i stedet.

## If-else if-else-setning:
Noen ganger har vi flere ting vi vil sjekke. Da kan vi bruke en kombinasjon av `if`, `else if` og `else` for å sjekke flere betingelser. 

```javascript
let score = 85;

if (score >= 90) {
  console.log("Du fikk en A.");
} else if (score >= 80) {
  console.log("Du fikk en B.");
} else {
  console.log("Du fikk en C eller lavere.");
}
```
I dette eksemplet sjekker vi flere ting:
* Først sjekker vi om `score` er 90 eller mer. 
* Hvis det ikke er sant, sjekker vi om `score` er 80 eller mer.
* Hvis ingen av de to betingelsene er sanne, skriver den "Du fikk en C eller lavere.

---

## Oppgaver

### Oppgave 1: Sjekk tall
Skriv en if-setning som sjekker om en variabel `number` er større enn 10. Hvis den er større, skriv ut "Større enn 10", ellers skriv ut "10 eller mindre".

```javascript
// Oppgave 1
let number = 12;

// Skriv if-setning her
```

### Oppgave 2: Kategori basert på alder
Lag et program som sjekker alderen til en person. Hvis personen er under 13, skal programmet skrive "Barn". Hvis personen er mellom 13 og 19, skal det skrive "Tenåring". Hvis personen er 20 eller eldre, skal det skrive "Voksen".

```javascript
// Oppgave 2
let age = 17;

// Skriv if-else if-else-setning her
```

### Oppgave 3: Enkel login-simulering
Skriv et program som sjekker om et brukernavn og passord er riktig. Hvis brukernavnet er "admin" og passordet er "1234", skal programmet skrive "Velkommen!". Hvis ikke, skal det skrive "Feil brukernavn eller passord".

```javascript
// Oppgave 3
let username = "admin";
let password = "1234";

// Skriv if-else-setning her
```

### Oppgave 4: Bonus – Graderingssystem
Lag et program som tar en variabel `poeng` og gir en karakter basert på poengene:
- 90 eller mer: A
- 80 eller mer: B
- 70 eller mer: C
- 60 eller mer: D
- Mindre enn 60: F

```javascript
// Oppgave 4
let poeng = 85;

// Skriv if-else if-else-setning her
```

---

Disse oppgavene vil gi deg en god forståelse av hvordan du kan bruke `if`-setninger for å ta beslutninger i JavaScript. Det er viktig for å lage dynamiske og responsive nettsider. 🚀
