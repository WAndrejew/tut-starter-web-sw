
# 📚 Woche 11–12: Abschlussprojekt & Deployment

## 🎯 Ziele
- Ein eigenes Fullstack-Webprojekt umsetzen
- Jira für Planung und Aufgaben nutzen
- Projektversionierung mit Git
- Deployment mit Docker oder Netlify

---

## 🗂️ Projektplanung mit Jira

### Schritte:

1. **Projekt definieren**
   - Ziel: z. B. Portfolio, Gästebuch, Blog, Mini-Tool

2. **Backlog anlegen**
   - Features (Startseite, Formular, DB, etc.)
   - In Epics, Stories & Tasks aufteilen

3. **Sprint starten**
   - Tasks in „To Do“, „In Progress“, „Done“

🔗 [Jira Getting Started Guide](https://www.atlassian.com/de/software/jira/guides)

---

## 🧠 Tipps zur Projektstruktur

```
myproject/
├── frontend/        # HTML/CSS/JS
├── backend/         # Express.js + SQLite
├── docker/
│   ├── Dockerfile
│   └── docker-compose.yml
├── README.md
└── .gitignore
```

- Trenne Frontend und Backend sauber
- Nutze Git-Branches für neue Features

---

## 🚀 Deployment-Optionen

### Variante A: Netlify (nur Frontend)

1. Projekt auf GitHub pushen
2. Mit Netlify verbinden: https://app.netlify.com/
3. Deploy direkt aus Repository

### Variante B: Docker Compose (Fullstack)

```yaml
# docker-compose.yml
version: "3"
services:
  web:
    build: ./backend
    ports:
      - "3000:3000"
  db:
    image: sqlite3
```

### Alternativen:
- Render.com (kostenloses Fullstack-Hosting)
- Railway, Vercel, Fly.io

---

## ✅ Abschlussprojekt: Eigene Website

### Anforderungen:

- **Mindestens 3 Seiten** (z. B. Home, Info, Kontakt)
- **Interaktives Feature** mit JavaScript
- **API-Anbindung** (z. B. Nachrichten, Formulare)
- **Datenbankanbindung** mit SQLite
- **Git + GitHub** für Versionierung
- **Jira-Board** für Planung

### Optional:
- Responsives Design
- Deployment mit Docker

---

## 📌 Bonusideen

- Portfolio-Website mit Eintragungsformular
- Mini-Blog mit SQLite & Markdown
- Aufgabenliste mit Backend-Speicherung
- Notizen-Tool mit API & Login (optional)

---

## 🏁 Projektabschluss

- Projekt dokumentieren (`README.md`)
- Code aufräumen & kommentieren
- Optional: Präsentation mit kurzen Slides oder GitHub Demo

🎉 Glückwunsch – du hast dein erstes Fullstack-Projekt gebaut!
