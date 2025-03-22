  
# 🧠 Webentwicklung von Null bis zur Website – Kursstruktur & Setup

**Beschreibung:**  
Dieser Kurs führt Schritt für Schritt durch die Grundlagen moderner Webentwicklung – von der ersten HTML-Seite bis zur vollständigen Website mit JavaScript, Datenbank, Docker und Versionskontrolle. Ideal für Einsteiger mit Interesse an praxisnaher Webentwicklung.

**Inhalte:**

- HTML, CSS, JavaScript
- Git & GitHub
- Jira & agile Projektplanung
- Express.js & API-Entwicklung
- SQL & Datenbankanbindung
- Docker & Containerisierung
- Abschlussprojekt mit echtem Deployment

**Ziel:**  
Am Ende besitzt du eine eigene, funktionierende Website mit API-Anbindung, entwickelst im Team, planst in Jira und nutzt moderne Tools wie Git und Docker.

---

## ✅ Setup-Checkliste: Webentwicklung von Null bis zur Website

### 🔧 Grund-Setup (lokal installieren)
- [ ] **VS Code** installieren 👉 https://code.visualstudio.com/
- [ ] **Windows Subsystem for Linux (WSL)**  
  _Powershell/Terminal command_  
```sh
	wsl --install
```
- [ ] **Node.js + npm** installieren 👉 https://nodejs.org/  
  _Mindestversion: Node 18+_
- [ ] **Git** installieren 👉 https://git-scm.com/
- [ ] **Docker Desktop** installieren 👉 https://www.docker.com/products/docker-desktop/  
  _Für Linux: Docker Engine + Docker Compose_
- [ ] **Postman** installieren (API testen) 👉 https://www.postman.com/downloads/
- [ ] **Sourcetree** (Git-Client) 👉 https://www.sourcetreeapp.com/
- [ ] **SQLiteStudio** (für SQL-Datenbanken, ab Woche 7)  👉 https://sqlitestudio.pl/

---
## 🔑 **Online-Accounts** anlegen

- [ ] **Google Account** 👉 https://accounts.google.com/signup
- [ ] **GitHub Account** 👉 https://github.com/join
- [ ] **Jira (Atlassian) Account** 👉 https://id.atlassian.com/signup  
  _Tipp: Neues Projekt mit Scrum oder Kanban starten_
- [ ] **Docker Hub Account** 👉 https://hub.docker.com/signup

---
### 🧩 VS Code Extensions (empfohlen)

- [ ] Live Server  
- [ ] Prettier – Code formatter  
- [ ] GitLens – Git supercharged  
- [ ] REST Client – HTTP Requests direkt in VS Code  
- [ ] Docker – Container-Verwaltung in VS Code  

---
## 📅 **Kursplan**
---
### **📅 Woche 1–2: Hello World & Git**

- Was ist Webentwicklung? (nur **Frontend**)
- Setup + Accounts
- VS Code & Browser DevTools
- **Git Einführung**
  - Git installieren, `init`, `add`, `commit`, `log`
  - Branches & Merge
  - GitHub: Repository anlegen, push/pull
- Template NodeJs Projekt

 **Ziel:** Hello World Web Page mit Git-Versionierung

---
### **📅 Woche 3–4: HTML & CSS & Jira**

- **HTML-Grundlagen**: Struktur, Tags
- **CSS-Grundlagen**
  - Farben, Schriften, Layout, Box-Modell
  - Flexbox und Grid
- Einführung in agile Entwicklung (Scrum/Kanban)
- Jira-Boards, Epics, Stories, Tasks
- Workflow von Planung bis Entwicklung
- Task board in Jira

**Ziel**: Web-Single-Page App (statisch)

---
### **📅 Woche 5–7: JavaScript Basics & Erste API & JSON**

- Variablen, Funktionen, Arrays, DOM
- Events (Klick, Hover, Input)
- Formulare interaktiv machen
- JSON verstehen
- Eigene kleine API simulieren (z. B. mit JSON Server oder Express.js)
- Frontend-Integration mit realen Daten
- Daten anzeigen, filtern, sortieren

- **Ziel**: Interaktives Formular mit Validierung  

---

### **📅 Woche 8–10: Backend-Kommunikation & SQL & Docker**

- **Client-Server-Prinzip**
- HTTP-Grundlagen (GET, POST)
- Fetch API in JavaScript
- **Datenbank Basics (SQL)**
  - Tabellen, SELECT, INSERT, UPDATE
  - Einfache SQLite- oder PostgreSQL-Datenbank (lokal oder gehostet)

- **Zwischen-Ziel:** Formular sendet Daten an Backend & speichert sie

- **Was ist Docker?**
  - Container vs. virtuelle Maschinen
  - Docker installieren
  - Einfache Container starten (`nginx`, `postgres`, `node`)
  - Dockerfile erstellen & bauen

- **Ziel:** Web-App + Datenbank in Containern laufen lassen 

---

### **📅 Woche 11–12: Abschlussprojekt**

- **Planung mit Jira:**
  - Backlog, Sprint, Task-Aufteilung
- **Projektarbeit:**
  - Eigene mehrseitige Website mit echter Datenanbindung (API + DB)
  - Responsives Design
  - Git-Versionierung, ggf. GitHub-Projektseite
  - Deployment mit Docker

- **Präsentation/Review**