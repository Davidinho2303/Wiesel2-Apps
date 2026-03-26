# assistr

**Coaching-Plattform für Basketballtrainer** — Drill-Bibliothek, Trainingsplanung, Saisonplanung, Team-Kollaboration.

🌐 [assistr öffnen](https://davidinho2303.github.io/wiesel2-dashboard/Drill.html)

---

## Was ist assistr?

assistr ist ein web-basiertes Coaching-Tool das Trainer beim Planen und Dokumentieren von Trainings unterstützt. Es läuft vollständig im Browser, funktioniert als iOS PWA und synchronisiert Daten in Echtzeit über Firebase.

---

## Features

### Drill-Bibliothek
- Drills anlegen, bearbeiten, filtern und durchsuchen
- Kategorien, Trainingsphase, Spielphase, Intensität, Spieleranzahl
- Bild und Video pro Drill
- **KI-Import:** Text oder Foto → Claude analysiert → Drills direkt importieren
- **Scopes:** Privat (nur du), Team (dein Team), Public (alle)

### Trainingsplanung
- Trainingsplan mit Zeitblöcken und Drills bauen
- Constraints pro Drill (z.B. "max 3 Dribbles")
- Export als Word, PDF, CSV oder WhatsApp-Text
- Plan-Templates mit Wochentag-Auto-Datum
- Templates auf privat, Team oder public teilen

### Saisonplanung
- Saison-Phasen mit Start/Ende, Farbe, Zielen und Wochenschwerpunkten
- Kalenderansicht mit eigenen Trainings (grün) und Team-Trainings (blau)
- IST/SOLL-Tracking pro Phase
- Kategorie-Verteilung der Drills pro Phase
- Alle Teammitglieder sehen gegenseitige Pläne in der Phasenübersicht

### Team-Kollaboration
- Mehrere User pro Team, mehrere Teams pro User
- Team beitreten per 6-stelligem Join-Code
- Pläne werden automatisch im Team geteilt
- Fremde Pläne sind read-only (kein versehentliches Überschreiben)
- Geteilte Templates und Drills auf Team-Ebene
- Saison-Phasen sind team-weit synchronisiert

---

## Einstieg

1. **assistr öffnen** → [Link](https://davidinho2303.github.io/wiesel2-dashboard/Drill.html)
2. **Kürzel eingeben** (z.B. `david`) — merke es dir, es ist dein einziger Zugangscode
3. **Team beitreten** (Join-Code vom Teamchef) oder neues Team anlegen
4. Loslegen

> **iOS:** "Zum Home-Bildschirm hinzufügen" für die beste Erfahrung als App.

---

## Technischer Stack

| Bereich | Technologie |
|---|---|
| Frontend | Single-File HTML — kein Framework, kein Build-Step |
| Hosting | GitHub Pages |
| Datenbank | Firebase Firestore |
| Medien | Firebase Storage |
| Auth | Anonymous Auth + Kürzel (kein Passwort) |
| KI | Anthropic Claude via Cloudflare Worker Proxy |

---

## Für Entwickler

Die gesamte App steckt in einer einzigen Datei: `Drill.html`. Änderungen werden direkt committet und über GitHub Pages deployed.

Technische Details, Firestore-Struktur, Patterns und bekannte Fallstricke: siehe [assistr_bauplan.md](assistr_bauplan.md).

### Lokale Entwicklung
Keine lokale Umgebung nötig — direkt `Drill.html` im Browser öffnen. Firebase läuft gegen die Produktions-Datenbank.

### Deploy
```
git add Drill.html
git commit -m "..."
git push
```
GitHub Pages deployed automatisch. Cache-Busting: Cmd+Shift+R im Browser.

---

## Roadmap

- **Google Login** — ersetzt das Kürzel-System, schützt Daten zuverlässig
- **Firestore Security Rules** — nach Google Login dichtmachen
- **Drill-Templates** — häufig genutzte Drill-Kombinationen als Template speichern
- **Code-Cleanup** — toten Code entfernen, Duplikate bereinigen

---

## Projekt

Entwickelt für **Weddinger Wiesel 2** (Herren Landesliga B Berlin, Saison 2025/2026).
Gebaut von David Schreiber mit Claude (Anthropic).
