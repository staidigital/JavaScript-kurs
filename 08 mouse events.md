
# Introduksjon til Mouse Events og Musekoordinater i JavaScript

I JavaScript kan vi bruke ulike **mouse events** for å interagere med nettsider på en dynamisk måte. Vanlige hendelser som kan fanges opp er for eksempel når brukeren klikker, holder musen over et element, eller beveger musen. I tillegg kan vi hente musekoordinatene for å lage mer interaktivt innhold.

## 1. Mouse Events
### Hva er en Mouse Event?
> En mouse event er en hendelse som skjer når brukeren gjør noe med musen, som å klikke eller bevege den over et element.

### `click`-hendelsen
`click`-hendelsen oppstår når brukeren klikker på et element.

```javascript
let button = document.getElementById("myButton");
button.addEventListener("click", function() {
    console.log("Knappen ble klikket!");
});
```

`getElementById("myButton")` finner knappen på siden med id-en `myButton`.
`addEventListener("click", ...)` legger til en funksjon som kjører når knappen klikkes.

Når brukeren klikker på knappen (`myButton`), skrives "Knappen ble klikket!" i konsollen.

### `mouseover` og `mouseout`

`mouseover`: Når musen flyttes over et element.
`mouseout`: Når musen flyttes ut av elementet.

```javascript
let box = document.getElementById("myBox");

box.addEventListener("mouseover", function() {
    box.style.backgroundColor = "lightblue";
});

box.addEventListener("mouseout", function() {
    box.style.backgroundColor = "white";
});
```
`mouseover`: Når musen er over elementet, endres bakgrunnsfargen til lys blå.
`mouseout`: Når musen forlater elementet, settes bakgrunnsfargen tilbake til hvit.

## 2. Musekoordinater

Når musen beveger seg over nettsiden, kan vi hente posisjonen til musen med koordinatene `clientX` og `clientY`. Disse gir deg x- og y-posisjonene til musepekeren i forhold til nettsidens synlige område.

```javascript
document.addEventListener("mousemove", function(event) {
    console.log("X-koordinat: " + event.clientX + ", Y-koordinat: " + event.clientY);
});
```
`clientX` gir x-posisjonen (horisontal).
`clientY` gir y-posisjonen (vertikal).

Når brukeren beveger musen over nettsiden, vil musekoordinatene skrives ut i konsollen.

## 3. Kombinere musehendelser og musekoordinater

La oss lage et eksempel der vi viser musekoordinatene i sanntid mens brukeren beveger musen over et element.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mouse Events</title>
    <style>
        #mouseArea {
            width: 300px;
            height: 300px;
            background-color: lightgray;
            text-align: center;
            line-height: 300px;
        }
    </style>
</head>
<body>
    <div id="mouseArea">Flytt musen her</div>
    <p id="coordinates">X: 0, Y: 0</p>

    <script>
        let mouseArea = document.getElementById("mouseArea");
        let coordinates = document.getElementById("coordinates");

        mouseArea.addEventListener("mousemove", function(event) {
            let x = event.clientX;
            let y = event.clientY;
            coordinates.textContent = "X: " + x + ", Y: " + y;
        });
    </script>
</body>
</html>
```

Her vises musekoordinatene i en `p`-tag når brukeren beveger musen over det grå feltet (`mouseArea`).

---

## Oppgaver

### Oppgave 1: Vis musekoordinater
Lag en nettside der du viser musekoordinatene når brukeren beveger musen over hele vinduet.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Musekoordinater</title>
</head>
<body>
    <h1>Musekoordinater</h1>
    <p id="mouseCoordinates">X: 0, Y: 0</p>

    <script>
        document.addEventListener("mousemove", function(event) {
            let x = event.clientX;
            let y = event.clientY;
            let coordinates = document.getElementById("mouseCoordinates");
            coordinates.textContent = "X: " + x + ", Y: " + y;
        });
    </script>
</body>
</html>
```

### Oppgave 2: Endre farge ved museklikk
Lag en nettside med et område (`div`) der bakgrunnsfargen endres hver gang brukeren klikker på området.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Klikk for å endre farge</title>
    <style>
        #colorBox {
            width: 200px;
            height: 200px;
            background-color: lightgreen;
        }
    </style>
</head>
<body>
    <div id="colorBox"></div>

    <script>
        let box = document.getElementById("colorBox");

        box.addEventListener("click", function() {
            let randomColor = "#" + Math.floor(Math.random()*16777215).toString(16);
            box.style.backgroundColor = randomColor;
        });
    </script>
</body>
</html>
```

---

Disse oppgavene gir deg grunnleggende forståelse for hvordan du kan bruke mouse events og musekoordinater i JavaScript for å skape interaktivitet på nettsiden din.