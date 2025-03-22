
# 📚 Woche 5–7: JavaScript Basics, API & JSON

## 🎯 Ziele
- JavaScript-Grundlagen verstehen
- Mit DOM-Elementen interagieren
- Formulare und Events nutzen
- JSON verstehen & API-Daten verarbeiten
- Erste kleine REST-API simulieren

---

## ✨ JavaScript Grundlagen

### Variablen & Datentypen

```javascript
let name = "Anna";
const alter = 28;
let istAktiv = true;
```

### Bedingungen & Schleifen

```javascript
if (alter > 18) {
  console.log("Volljährig");
}

for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

### Funktionen

```javascript
function begruessen(name) {
  return "Hallo " + name;
}
```

🔗 [MDN JavaScript-Grundlagen](https://developer.mozilla.org/de/docs/Web/JavaScript/Guide)

---

## 🧠 Der DOM & Events

### Elemente auswählen und manipulieren:

```javascript
const btn = document.querySelector("button");
btn.textContent = "Klick mich!";
```

### Event Listener:

```javascript
btn.addEventListener("click", function () {
  alert("Button wurde geklickt!");
});
```

🔗 [MDN – DOM Events](https://developer.mozilla.org/en-US/docs/Web/API/Event)

---

## 📝 Formulare & Validierung

```html
<form id="kontaktForm">
  <input type="text" id="name" required />
  <button type="submit">Senden</button>
</form>
```

```javascript
document.getElementById("kontaktForm").addEventListener("submit", function (e) {
  e.preventDefault();
  let name = document.getElementById("name").value;
  alert("Hallo, " + name);
});
```

---

## 📦 JSON & APIs

### Was ist JSON?

```json
{
  "name": "Lisa",
  "alter": 25
}
```

### Daten holen (Fetch API):

```javascript
fetch("https://jsonplaceholder.typicode.com/users")
  .then(response => response.json())
  .then(data => console.log(data));
```

🔗 [JSON Einführung](https://developer.mozilla.org/de/docs/Learn/JavaScript/Objects/JSON)

---

## 🧪 Aufgaben & Übungen

### 🔹 Aufgabe 1: Interaktives Formular
- Name und E-Mail als Eingabefelder
- Bei Absenden:
  - Eingaben prüfen
  - In der Konsole ausgeben
  - Leere Felder farblich markieren

### 🔹 Aufgabe 2: Farbwechsler
- Button erzeugt Zufallsfarbe für den Hintergrund

### 🔹 Aufgabe 3: API-Daten anzeigen
- Hole Benutzerdaten von https://jsonplaceholder.typicode.com/users
- Zeige Namen und E-Mails in einer Liste an

### 🔹 Aufgabe 4: Mini-API mit JSON Server
1. Installiere JSON Server:
```bash
npm install -g json-server
```
2. Erstelle eine Datei `db.json`:

```json
{
  "nachrichten": [
    { "id": 1, "text": "Hallo Welt" }
  ]
}
```

3. Starte den Server:
```bash
json-server --watch db.json
```

4. Teste mit `fetch()`:
```javascript
fetch("http://localhost:3000/nachrichten")
  .then(res => res.json())
  .then(data => console.log(data));
```

---

## ✅ Mini-Projekt: Gästebuch

### Ziel:
Ein einfaches Gästebuch mit:
- Formular für Name und Nachricht
- Nachrichten werden per Fetch an API gesendet (POST)
- Alle Einträge werden automatisch angezeigt (GET)

**Extra:**
- Fehlermeldungen bei leeren Feldern
- Visuelles Feedback nach dem Absenden
