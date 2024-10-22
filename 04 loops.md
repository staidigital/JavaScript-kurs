
# Introduksjon til løkker i JavaScript

Løkker lar deg gjenta den samme koden flere ganger uten å skrive den flere ganger manuelt. Dette er nyttig når du vil gjøre noe mange ganger, som å gå gjennom en liste med ting eller telle opp til et bestemt tall.

## 1. For-løkker (for-loops)
For-løkker brukes mest når du vet hvor mange ganger du vil at en handling skal gjentas. Det er tre ting som kontrollerer en for-løkke: startverdien, når den skal stoppe, og hvordan den teller opp.

```javascript
for (let i = 0; i < 5; i++) {
  console.log("Dette er iterasjon nummer " + i);
}
```
Her er hva som skjer:
- `let i = 0`: Vi starter med at variabelen `i` gis verdien 0.
- `i < 5`: Løkken kjører så lenge `i` er mindre enn 5.
- `i++`: For hver gang løkken kjører (for hver *iterasjon*), økes `i` med 1. 

Så denne løkken vil skrive ut "Dette er iterasjon nummer 0", "Dette er iterasjon nummer 1", osv., helt opp til 4.

## 2. While-løkker (while-loops)
En **while-løkke** fortsetter å kjøre så lenge en betingelse er sann. Denne typen løkke er bra når du ikke vet på forhånd hvor mange ganger du trenger å gjenta noe.

```javascript
let i = 0;
while (i < 5) {
  console.log("Dette er iterasjon nummer " + i);
  i++;
}
```

Her vil løkken kjøre så lenge `i` er mindre enn 5, akkurat som i for-løkken. Forskjellen er at med en while-løkke, skriver du oppdateringen (`i++`) selv inne i løkken, og løkken vil fortsette å kjøre så lenge betingelsen `i<5` er sann.

## 3. Do-while-løkker
En **do-while-løkke** er litt spesiell. Den kjører alltid **minst én gang**, selv om betingelsen er falsk fra starten. Etter første gang den kjører, sjekker den om betingelsen fortsatt er sann.

```javascript
let i = 0;
do {
  console.log("Dette er iterasjon nummer " + i);
  i++;
} while (i < 5);
```

I dette eksempelet vil løkken også kjøre så lenge i er mindre enn 5, men den kjører alltid minst én gang før den sjekker betingelsen.

---

## Oppgaver

### Oppgave 1: Tell opp fra 1 til 10
Bruk en for-løkke til å skrive ut tallene fra 1 til 10 i konsollen.


### Oppgave 2: Finn summen av tallene fra 1 til 100
Skriv et program som bruker en while-løkke for å finne summen av alle tallene fra 1 til 100.


### Oppgave 3: Skriv ut et array
Lag et array med noen bynavn. Bruk en for-løkke til å skrive ut hvert bynavn i konsollen.


### Oppgave 4: Finn det største tallet
Lag et array med tall. Bruk en for-løkke til å finne det største tallet i arrayet.


---

Disse oppgavene hjelper deg å forstå hvordan løkker fungerer i JavaScript. Løkker er et kraftig verktøy for å gjøre ting om igjen uten å skrive samme kode flere ganger.