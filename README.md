# assistr — Handbuch für neue Coaches

**Dein digitaler Assistant Coach**

`davidinho2303.github.io/wiesel2-dashboard/Drill.html`

-----

## Überblick

assistr ist eine digitale Coaching-Plattform — läuft im Browser, keine Installation nötig. Einfach URL aufrufen und loslegen.

|Feature           |Beschreibung                                              |
|------------------|----------------------------------------------------------|
|📚 Drill-Bibliothek|70+ Drills, filterbar, mit Beschreibung & Coaching-Punkten|
|📋 Trainingsplanung|Pläne aus Blöcken bauen, Drills zuweisen, exportieren     |
|📅 Saisonplanung   |Phasen mit Zeitraum, Ziel & Tracking                      |
|📊 Tracking        |Drill-Einsatz über die Saison auswerten                   |
|🤖 KI Drill-Import |Drills per Freitext oder Foto automatisch importieren     |
|👥 Multi-User      |Eigenes Kürzel, geteilte und private Inhalte              |

-----

## Erste Schritte

### App öffnen

URL im Browser aufrufen:

```
davidinho2303.github.io/wiesel2-dashboard/Drill.html
```

> 💡 **Mobil:** Über “Teilen” → “Zum Home-Bildschirm hinzufügen” lässt sich die App wie eine native App auf dem Homescreen ablegen — direkter Zugriff, kein Browser nötig.

### Einloggen

Beim ersten Start erscheint ein Login-Screen. Kürzel eingeben (z.B. “max”, “anna”) und Speichern tippen.

- Nur Kleinbuchstaben und Zahlen — wird automatisch erzwungen
- Kürzel merken — solange kein Google Login existiert ist es der einzige Zugang
- Falls das Kürzel schon vergeben ist, kommt eine Warnung mit der Option trotzdem fortzufahren

-----

## Navigation

Auf Mobile: Bottom-Navigation mit 5 Tabs. Auf Desktop: Sidebar links.

|Tab|Name     |Inhalt                                                 |
|---|---------|-------------------------------------------------------|
|📚  |Drills   |Drill-Bibliothek — alle Drills suchen, filtern, ansehen|
|📋  |Plan     |Aktuellen Trainingsplan bearbeiten                     |
|📊  |Tracking |Drill-Einsatz-Statistiken                              |
|📦  |Übersicht|Alle gespeicherten Pläne                               |
|📅  |Saison   |Saisonphasen & Kalender                                |

-----

## 📚 Drill-Bibliothek

Alle Drills — filterbar nach allen relevanten Dimensionen.

### Filtern & Suchen

- Freitextsuche nach Drill-Name
- Kategorie: Passing, Ballhandling, Shooting, Defense, Offense, …
- Trainingsphase: Warmup / Hauptteil
- Spielphase: Technik, SO (Set Offense), OT, DT, SD
- Intensität: niedrig / mittel / hoch
- Min. Spieler: filtert Drills die mit weniger Spielern funktionieren
- Ersteller: Alle / Nur meine

### Drill-Detail

Drill antippen → Detail-Modal mit Beschreibung, Variationen, Coaching-Punkten, Bild/Video. Von hier direkt zum Trainingsplan hinzufügen.

### Neuer Drill

- Button “+ Neuer Drill” → Formular ausfüllen → Speichern
- Sichtbarkeit: “Geteilt” = alle Coaches sehen ihn / “Nur ich” = privat

> 💡 Schneller: KI Drill-Import nutzen — Freitext oder Foto, Claude füllt alle Felder automatisch aus.

-----

## 🤖 KI Drill-Import

Das Kernfeature von assistr. Drills per Freitext oder Foto importieren — Claude erkennt automatisch Name, Kategorie, Phase, Intensität und alle anderen Metadaten.

### So geht’s

1. “🤖 KI-Import” in der Drill-Bibliothek antippen
1. Tab wählen: Text oder Bild
1. “Analysieren” tippen — Claude erkennt alle Drills im Input
1. Erkannte Drills prüfen und bei Bedarf anpassen
1. “Ausgewählte speichern” → fertig, Drills sind sofort in der Bibliothek

### Text-Modus

Drills frei beschreiben — ein oder mehrere, kein festes Format nötig:

```
Shell Drill: 4-on-4 Defense, Halbfeld, 8 Spieler, Defense live, kompetitiv, Abschluss
Leiter Dribbling — Warmup, 1 Spieler, niedrige Intensität
```

### Bild-Modus

- Foto von Whiteboard, Drill-Sheet oder handgeschriebenem Zettel
- Direkt aufnehmen oder aus der Galerie wählen
- Claude liest alle erkennbaren Drills aus dem Bild

> 💡 Auch Screenshots aus anderen Coaching-Apps oder PDFs funktionieren — einfach Screenshot machen und importieren.

-----

## 📋 Trainingsplanung

Pläne aus Zeitblöcken aufbauen, Drills zuweisen, exportieren.

### Plan erstellen

- Tab “Plan” öffnen
- Template laden (falls vorhanden) oder “+ Leerer Plan”
- Datum wählen → Name wird automatisch auf “Datum — Ort” gesetzt
- Gegner / Thema eintragen (optional)
- Gesamtzeit setzen (Standard: 90 Min)

### Drills zuweisen

- In jedem Block “+ Drill auswählen” tippen
- Drill suchen oder filtern, antippen zum Hinzufügen
- Minuten pro Drill anpassen
- Reihenfolge per Pfeil-Buttons ändern, Drills per × entfernen

### Blöcke verwalten

- **Warmup & Stretching:** fix vorgegeben, Dauer anpassbar, kein Löschen
- **Hauptteil:** frei bespielbar, verschiebbar, löschbar
- **Abschluss (Ausdehnen):** fix vorgegeben
- **Eigene Blöcke:** “+ Block hinzufügen” erstellt einen neuen freien Block

### Speichern & Teilen

- “💾 Speichern” → Plan ist in der Cloud, sofort auf allen Geräten sichtbar
- Schloss-Icon: Plan sperren (kein versehentliches Überschreiben)
- Export: Word (.htm), PDF/Drucken, JSON, CSV, WhatsApp-Text

> 💡 Als Template speichern: “📋 Tpl.” Button. Templates erscheinen oben im Plan-Tab für schnellen Zugriff.

-----

## 📅 Saisonplanung

Überblick über die gesamte Saison — Phasen definieren, Trainingsdichte tracken.

### Phase anlegen

- “+ Phase” tippen
- Name, Zeitraum (Start/Ende), Farbe, Wochenziel eingeben
- Ziele (Freitext) optional
- Schwerpunkte: Kategorien mit optionalem %-Ziel
- Speichern → Phase erscheint im Kalender als farbiger Balken

### Kalender

- Phasen als farbige Balken über den Tagen
- Trainingspunkte (●) zeigen Tage mit gespeicherten Plänen
- Tag antippen → Popup mit Phasen und Plänen des Tages
- Kalender-Monat wechseln per ‹ / ›
- “☰ Liste” / “📅 Kalender” umschalten

### Tracking pro Phase

- **IST / SOLL:** Trainings gezählt vs. Wochenziel
- **Kategorien-Balken:** welche Drill-Kategorien wurden wie oft eingesetzt
- **Trainings dieser Phase:** alle gespeicherten Pläne aufgelistet, direkt öffenbar

-----

## 📊 Tracking

Auswertung welche Drills wie oft in Trainingsplänen eingesetzt wurden.

- Datumsfilter: beliebigen Zeitraum wählen
- Übersicht: Gesamtanzahl, Drill-Minuten, aktive Pläne
- Drill-Rangliste: sortiert nach Einsatz-Häufigkeit
- Kategorie-Auswertung: welche Bereiche dominieren das Training

> 💡 Tracking zählt nur gespeicherte Pläne — nicht den aktuell offenen Plan.

-----

## 👥 Multi-User & Berechtigungen

### Kürzel & Rollen

- Jeder Coach hat ein eigenes Kürzel (z.B. “anna”, “max”)
- **Admin:** kann alle Inhalte bearbeiten und löschen, unabhängig vom Ersteller
- **Coach:** kann eigene Inhalte und geteilte Inhalte bearbeiten

### Sichtbarkeit

|Inhalt         |Sehen   |Bearbeiten       |Löschen          |
|---------------|--------|-----------------|-----------------|
|Geteilte Drills|Alle    |Ersteller + Admin|Ersteller + Admin|
|Eigene Drills  |Nur ich |Nur ich          |Nur ich          |
|Geteilte Pläne |Alle    |Alle             |Ersteller + Admin|
|Eigene Pläne   |Nur ich |Nur ich          |Nur ich          |
|Plan-Templates |Je Scope|Ersteller + Admin|Ersteller + Admin|

-----

## Mobile Tipps

- **Home-Bildschirm:** “Teilen” → “Zum Home-Bildschirm” — App verhält sich wie nativ, kein Browser-Chrome
- **Erster Start:** kurz warten bis alle Drills aus der Cloud geladen sind
- **Exportieren:** Teilen-Button → “In Dateien sichern” oder “Drucken” → Als PDF speichern
- **Kein Netz:** Bereits geladene Inhalte bleiben im Cache — Speichern und Sync benötigen Verbindung

-----

*assistr · Saison 2025/2026*