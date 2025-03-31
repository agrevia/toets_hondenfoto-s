## 📝 **Toetsopdracht JavaScript – Hondengenerator **

### 📦 Wat krijg je?

Je krijgt een **HTML- en CSS-bestand** waarin:

- de knoppen al aanwezig zijn
- het `<img>`-element en `#foto-zone` al voorzien zijn
- de juiste `id`’s aan alle knoppen staan

Je taak is om het **JavaScript-bestand (`script.js`)** volledig zelf te schrijven volgens de onderstaande richtlijnen.

------

### 🎯 **Leerdoelen**

Je toont aan dat je:

- met de DOM kan werken via `document.querySelector`
- knoppen correct koppelt via `addEventListener`
- functies met parameters schrijft
- een API-aanroep uitvoert met `fetch` en `async/await`

------

### 🔧 **Opdracht: schrijf het script**

#### 1. Begin met een `DOMContentLoaded`-event

- Maak een `init()`-functie waarin je alle knoppen koppelt
- Roep deze `init()` aan **wanneer de DOM geladen is**

------

#### 2. Laad een willekeurige hondenfoto

- Gebruik de API: `https://dog.ceo/api/breeds/image/random`
- Schrijf een functie `fetchDog()` die:
  - een API-aanroep doet met `fetch`
  - het resultaat toont in het `<img id="hondenfoto">`-element
- Roep deze functie op:
  - bij het laden van de pagina
  - én bij een klik op de knop met `id="nieuwe-hond"`

> ✅ *Tip: gebruik `async/await` + `try...catch` om fouten netjes op te vangen.*

------

#### 3. Verander de achtergrondkleur van `#foto-zone`

- De knoppen zijn al voorzien met `id="kleur-blauw"`, `kleur-geel`, `kleur-wit`
- Schrijf voor elk van deze knoppen een aparte `addEventListener`
- Maak één functie `veranderAchtergrondkleur(kleur)` die de `backgroundColor` aanpast

#### 4. Verander de randstijl van `#foto-zone`

- De knoppen zijn al voorzien met `id="rand-solid"`, `rand-dashed`, `rand-none`
- Schrijf voor elk van deze knoppen een aparte `addEventListener`
- Maak één functie `veranderRandstijl(stijl)` die de `borderStyle` aanpast
