
# 📚 Woche 8–10: Backend-Kommunikation, SQL & Docker

## 🎯 Ziele
- HTTP & Fetch API verstehen
- Daten an ein Backend senden
- Einführung in SQL & SQLite
- Daten in Datenbanken speichern und abrufen
- Erste Nutzung von Docker zur Containerisierung

---

## 🌐 HTTP & Fetch API

### Was ist HTTP?

- **GET**: Daten abrufen
- **POST**: Daten senden
- **PUT/PATCH**: Daten ändern
- **DELETE**: Daten löschen

### Beispiel mit Fetch:

```javascript
// GET
fetch("http://localhost:3000/nutzer")
  .then(res => res.json())
  .then(data => console.log(data));

// POST
fetch("http://localhost:3000/nutzer", {
  method: "POST",
  headers: { "Content-Type": "application/json" },
  body: JSON.stringify({ name: "Anna" })
});
```

📖 [MDN Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)

---

## 💾 SQL & SQLite

SQL (Structured Query Language) ist die Sprache für Datenbanken.

### Grundbefehle

```sql
CREATE TABLE benutzer (
  id INTEGER PRIMARY KEY,
  name TEXT,
  email TEXT
);

INSERT INTO benutzer (name, email) VALUES ('Max', 'max@example.com');

SELECT * FROM benutzer;

UPDATE benutzer SET name = 'Anna' WHERE id = 1;

DELETE FROM benutzer WHERE id = 1;
```

🔗 [SQL-Tutorial auf sqlitetutorial.net](https://www.sqlitetutorial.net/)

### Tools:
- SQLiteStudio → https://sqlitestudio.pl/
- DBeaver → https://dbeaver.io/

---

## 🐳 Einführung in Docker

### Was ist Docker?
- Tool zur Verpackung von Anwendungen in Containern
- Container = Mini-Linux-System mit deiner App

### Grundbegriffe:
- **Dockerfile**: beschreibt, wie ein Container gebaut wird
- **Image**: Vorlage für Container
- **Container**: laufendes Image

### Beispiel Dockerfile:

```dockerfile
FROM node:18
WORKDIR /app
COPY . .
RUN npm install
CMD ["node", "server.js"]
```

### Docker-Befehle:

```bash
docker build -t meine-app .
docker run -p 3000:3000 meine-app
```

📖 [Docker Einstieg (offiziell)](https://docs.docker.com/get-started/)

---

## ✅ Aufgaben & Übungen

### 🔹 Aufgabe 1: Formular + Backend
- Erstelle ein HTML-Formular (Name, E-Mail)
- Sende die Daten via `fetch()` an eine Express.js API
- Speichere sie in einer SQLite-Datenbank

### 🔹 Aufgabe 2: SQL testen
- Starte SQLiteStudio
- Lege eine Tabelle an
- Füge Testdaten ein und rufe sie ab

### 🔹 Aufgabe 3: Docker verstehen
- Installiere Docker Desktop
- Starte einen Beispiel-Container:
  ```bash
  docker run -d -p 8080:80 nginx
  ```
- Öffne `http://localhost:8080`

---

## 🎯 Mini-Projekt: Feedback-API mit Docker

### Ziel:
Eine Fullstack-Anwendung bestehend aus:
- HTML-Formular zur Eingabe von Feedback
- Express.js API mit SQLite zur Speicherung
- Docker-Container für das Backend

**Optional:** Docker Compose zum Kombinieren von API + DB

🔗 Beispielprojekt-Setup auf Wunsch verfügbar!
