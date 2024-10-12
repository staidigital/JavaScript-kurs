
# Introduksjon til if-setninger i JavaScript

Når du har lært om variabler, er det neste steget å forstå hvordan man kan ta beslutninger i koden ved hjelp av if-setninger. If-setninger brukes til å utføre kode kun hvis en betingelse er oppfylt.

## Grunnleggende if-setning:
En enkel if-setning sjekker om en betingelse er sann. Hvis den er det, kjøres koden innenfor klammeparentesene.

```javascript
let age = 18;

if (age >= 18) {
  console.log("Du er myndig.");
}
```

I dette eksempelet sjekker if-setningen om `age` er større enn eller lik 18. Hvis det er sant, skriver den "Du er myndig." i konsollen.

## If-else-setning:
Hvis du ønsker å utføre en annen handling når betingelsen ikke er oppfylt, kan du bruke en if-else-setning.

```javascript
let age = 16;

if (age >= 18) {
  console.log("Du er myndig.");
} else {
  console.log("Du er ikke myndig.");
}
```

Her sjekker if-setningen om `age` er større enn eller lik 18. Hvis det ikke er sant, skriver den "Du er ikke myndig." i stedet.

## If-else if-else-setning:
Noen ganger trenger du å sjekke flere betingelser. Dette kan gjøres med en if-else if-else-struktur.

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

Her sjekkes først om `score` er 90 eller høyere. Hvis ikke, sjekker den om `score` er 80 eller høyere. Hvis ingen av betingelsene er sanne, skriver den "Du fikk en C eller lavere."

---

## Oppgaver

### Oppgave 1: Sjekk tall
Skriv en if-setning som sjekker om en variabel `number` er større enn 10. Hvis den er det, skal "Større enn 10" skrives ut, hvis ikke skal "10 eller mindre" skrives ut.

```javascript
// Oppgave 1
let number = 12;

// Skriv if-setning her
```

### Oppgave 2: Kategori basert på alder
Lag et program som sjekker en persons alder. Hvis personen er under 13, skal programmet skrive "Barn". Hvis personen er mellom 13 og 19, skal det skrive "Tenåring". Hvis personen er 20 eller eldre, skal det skrive "Voksen".

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
Lag et program som tar en variabel `poeng` som verdi og gir en karakter basert på følgende betingelser:
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

Disse oppgavene vil hjelpe deg å forstå hvordan if-setninger kan brukes til å ta beslutninger i koden din, basert på variablenes verdier.
