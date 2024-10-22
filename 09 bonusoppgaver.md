# Bonusoppgaver i JavaScript

Her er tre bonusoppgaver du kan velge mellom, alle på omtrent samme vanskelighetsgrad som å lage en todo-list-app. Du kan velge hvilken oppgave du vil jobbe med, eller prøve deg på alle tre!

---

## Oppgave 1: Lag en "Todo-list"-app

**Beskrivelse:**  
Lag en enkel "todo-list"-applikasjon der brukeren kan legge til, fjerne og merke av oppgaver som fullført. Dette er en fin måte å øve på dynamisk håndtering av DOM-elementer i JavaScript.

**Krav til funksjonalitet:**
- Brukeren skal kunne skrive inn en oppgave i et tekstfelt og legge til denne i en liste når de klikker på en "Legg til"-knapp.
- Hver oppgave skal vises som et eget element i listen med mulighet for å markere den som "fullført".
- Det skal være en knapp for å slette en oppgave.
- Oppgavene skal lagres i `localStorage`, slik at listen ikke blir tom når siden lastes inn på nytt.

**Tips:**
- Bruk event listeners for å håndtere klikk på knapper.
- Sørg for å bruke funksjoner for å holde koden ryddig og lett å forstå.

---

## Oppgave 2: Lag en "Terningsimulator"

**Beskrivelse:**  
Lag en applikasjon der brukeren kan simulere å kaste en terning. Terningen skal kunne ha mellom 4 og 20 sider, og resultatet fra hvert kast skal vises i en liste. 

**Krav til funksjonalitet:**
- Brukeren skal kunne velge hvor mange sider terningen har (4, 6, 8, 10, 12, 20).
- Brukeren skal kunne klikke på en "Kast terning"-knapp for å simulere et kast, og resultatet skal vises under knappen.
- Hver gang brukeren kaster terningen, skal resultatet legges til i en liste med alle tidligere kast.
- Legg til en knapp for å slette alle kast og starte på nytt.

**Tips:**
- Bruk `Math.random()` for å generere et tilfeldig tall.
- Sørg for at brukeren kan velge antall sider på terningen før de kaster den.

---

## Oppgave 3: Lag en "Enkel kalkulator"

**Beskrivelse:**  
Lag en enkel kalkulator der brukeren kan legge inn to tall og velge en operasjon (addisjon, subtraksjon, multiplikasjon eller divisjon). Resultatet skal vises når brukeren trykker på "Beregn"-knappen.

**Krav til funksjonalitet:**
- Brukeren skal kunne legge inn to tall i hver sitt tekstfelt.
- Brukeren skal kunne velge hvilken operasjon de vil utføre (addere, subtrahere, multiplisere eller dividere) ved hjelp av en dropdown-meny.
- Resultatet av operasjonen skal vises på skjermen etter at brukeren klikker på "Beregn".
- Lag en knapp for å resette kalkulatoren og fjerne tidligere resultat.

**Tips:**
- Bruk `parseInt()` eller `parseFloat()` for å konvertere input-feltene til tall.
- Lag en funksjon for hver operasjon (addisjon, subtraksjon, osv.) for å gjøre koden din mer oversiktlig.

---

Alle oppgavene gir deg en god mulighet til å øve på grunnleggende JavaScript, inkludert DOM-manipulering, lagring i `localStorage`, bruk av event listeners, og modulær koding. Hvilken oppgave vil du ta fatt på først?
