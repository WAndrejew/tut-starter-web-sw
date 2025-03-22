# 📚 Woche 1–2: Einstieg in Webentwicklung & Git

## 🎯 Ziele

- Grundverständnis: Was ist Webentwicklung?
- Erste eigene HTML-Seite erstellen
- Git & GitHub verstehen und nutzen
- VS Code und Browser DevTools kennenlernen

TIip
Verwenden nur Open Source Tools und Free Account!!! Verwende https://www.deepl.com/de/translator als Übersetzer oder https://chatgpt.com/ (mein täglicher Helfer). Wenn du fragen hast, fragt zuerst Google oder ChatGPT. Du bist nicht der erster und findest zur der Grundfragen auch bestimmt Lösung (investiere etwas Zeit wenn es nicht out of box funktioniert).
 
---

## 🌐 Was ist Webentwicklung?


Webentwicklung umfasst das Erstellen und Pflegen von Webseiten und Webanwendungen. Es gibt zwei Hauptbereiche:

- **Frontend**: Alles, was im Browser sichtbar ist (HTML, CSS, JavaScript)
- **Backend**: Serverseitige Logik, APIs, Datenbanken (z. B. Node.js) 

📖 Mehr dazu:

- [MDN Web Docs – Introduction to web development](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web)

---
## 🛠️ Tools installieren & vorbereiten

- **VS Code**: Code-Editor → https://code.visualstudio.com/
- **Browser (Chrome/Firefox)**: Für Vorschau und DevTools
- **Git**: Versionskontrolle → https://git-scm.com/
- **GitHub**: Online-Plattform für Git-Repositories → https://github.com/ 

---
## 🧱 HTML-Grundlagen

HTML (HyperText Markup Language) ist das Grundgerüst jeder Website.  

Beispiel:  

```html

<!DOCTYPE html>

<html>

  <head>

    <title>Meine erste Seite</title>

  </head>

  <body>

    <h1>Hello World!</h1>

    <p>Das ist meine erste Webseite.</p>

  </body>

</html>

```

🔗 Mehr lernen:

- [HTML Einsteigerkurs auf MDN](https://developer.mozilla.org/de/docs/Web/HTML)
- [W3Schools HTML Tutorial](https://www.w3schools.com/html/)

---
## 🔧 DevTools verwenden

Mit **F12** oder Rechtsklick → „Untersuchen“ kannst du im Browser:

- Seitenstruktur (DOM) inspizieren
- CSS live ändern
- JavaScript-Fehler sehen 

📖 [MDN – Introduction to browser developer tools](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_are_browser_developer_tools)

---
## 🌱 Git Basics

Mit Git kannst du Codeänderungen versionieren und rückgängig machen.
### Grundbefehle im Terminal:  

```bash

git init            # Neues Git-Repository

git add .           # Änderungen zum Commit vormerken

git commit -m "Erster Commit"

git status          # Status anzeigen

git log             # Verlauf anzeigen

```

### GitHub verbinden:
  

```bash

git remote add origin https://github.com/benutzername/repo.git

git push -u origin main

```

  

🔗 Mehr lernen:
- [Git Dokumentation](https://git-scm.com/doc)
- [GitHub Learning Lab](https://lab.github.com/)

---
## ✅ Mini-Projekt: Hello World Website mit Git

1. Erstelle eine HTML-Datei (`index.html`) mit einer Überschrift und einem Absatz.
2. Initialisiere ein Git-Repo in diesem Ordner.
3. Mache deinen ersten Commit.
4. Lege ein GitHub-Repository an und pushe dein Projekt online.

🎯 Ziel: Deine erste versionierte Website auf GitHub!