# Narrentreffen 2027 – Planungs-App
**Binkerzunft Boll e.V. · Sauldorf-Boll · 5.–7. Februar 2027**

🌐 **Live:** https://wistefa.github.io/narrentreffen-2027/

---

## Was ist das?

Eine vollständig interaktive **Planungs-App** für das Narrentreffen als einzelne HTML-Datei.  
Kein Server, keine Installation, kein Internet nötig (außer für Chart.js-Diagramme).

Alle Inhalte sind **direkt im Browser editierbar** – Klick auf einen Wert, tippen, fertig.  
Alles wird automatisch im Browser gespeichert (localStorage) und überlebt einen Reload.

---

## Tabs im Überblick

| Tab | Inhalt |
|-----|--------|
| 📊 **Dashboard** | Gesamtstatus, Fortschrittsbalken, T-Minus Zeitplan |
| 📋 **Zunftanmeldung** | 50 NVH-B Zünfte, Anmeldestatus, Aufstellungsplan |
| 🎭 **Umzug** | Reihenfolge, Positionsnummern, 2,2 km Strecke |
| 📅 **Programm** | Detailprogramm Fr–So mit allen Veranstaltungen |
| 🏨 **Unterkunft** | Quartierplan, Belegung, Anfahrt |
| 🎟 **Tickets** | Verkaufsübersicht, Preiskategorien, Auslastung |
| 🎰 **Tombola** | Losverkauf, Preisübersicht, Verlosungsplan |
| 💶 **Finanzen** | Budget, Einnahmen/Ausgaben, Rücklagen |
| 🙋 **Helfer** | Schichtplanung, Drag & Drop, Helfer-Karten, CSV-Export |
| 🚌 **Logistik** | Parkplätze, Shuttle, Infrastruktur, Sicherheit |
| 🍺 **Narrenstände** | Standliste, WC/Müll-Punkte |
| 📨 **Kommunikation** | Briefvorlagen, E-Mail-Status, Pressemitteilungen |
| 📞 **Kontakte** | Telefonlisten, Suche, Gruppen-Filter |
| 🏟 **Reithalle Setup** | Aufbauplan, Ausstattungslisten, Zeitplan, Budget |
| 🏅 **ZM-Empfang** | Saalplan Gemeindehalle, Bewirtungsplan, Programm |
| 💛 **Sponsoren** | Sponsorenpakete, CRUD-Liste, Leistungsmatrix, Budget |

---

## Editierbarkeit

**Alles ist editierbar** – einfach draufklicken:

- Alle Tabellen: Zellen direkt bearbeiten, Zeilen löschen (✕), neue Zeilen hinzufügen (➕)
- Tabellen mit Drag & Drop: Reihenfolge per ⠿-Handle verschieben
- Alle Texte, Kennzahlen-Karten, Alerts und Info-Boxen per Klick bearbeitbar
- Aufbau-Zeitpläne und Offene-Punkte-Boxen sind freie Textbereiche
- **Sponsorenliste:** Stufe und Status als Dropdown-Menü auswählbar

Änderungen werden sofort in `localStorage` gespeichert. Kein Speichern-Button nötig.

---

## Daten sichern & teilen

| Aktion | Wo |
|--------|-----|
| **Backup exportieren** | Dashboard → „Daten exportieren" → JSON-Datei |
| **Backup importieren** | Dashboard → „Importieren" → JSON-Datei auswählen |
| **Reset** | Dashboard → „Alle Daten zurücksetzen" |

Beim Import werden nur Schlüssel mit dem Präfix `nt27_` oder `sp_` akzeptiert.

Für gemeinsames Arbeiten: nach Änderungen JSON-Backup exportieren und an Kollegen schicken.

---

## Was sind Echtdaten, was Platzhalter?

| Bereich | Status |
|---------|--------|
| 50 Zünfte (NVH-B) | ✅ echte Namen und Landschaften |
| Veranstaltungsorte | ✅ Reithalle, Zelt, Gemeindehalle |
| Umzugsstrecke | ✅ 2.200 m mit WC- und Müllpunkten |
| Sponsorenliste | ⚠ Demo-Daten, bitte ersetzen |
| Helfer-Stammdaten | ⚠ Demo-Daten, bitte ersetzen |
| Finanzzahlen | ⚠ Schätzwerte, bitte aktualisieren |
| Kontaktdaten | ⚠ Beispieldaten, bitte ergänzen |

---

## Technisches

- **Single File:** ~400 KB, alles in einer `index.html`
- **Browser:** Chrome, Firefox, Edge, Safari (Chrome empfohlen)
- **Persistenz:** localStorage im jeweiligen Browser
- **Kein Internet** nötig (Chart.js wird von CDN geladen – offline: keine Diagramme)
- **CSP:** Content-Security-Policy Meta-Tag aktiv (`object-src 'none'`, `base-uri 'self'`)
- **Plattform:** Windows, Mac, Linux

---

## Deployment

GitHub Pages: Push nach `main` → live unter https://wistefa.github.io/narrentreffen-2027/

```bash
# Lokales Deploy-Script (Python, kein git nötig):
python3 deploy.py   # nutzt macOS Keychain für GitHub-Token
```

---

*Erstellt für Binkerzunft Boll e.V. · Stand: Juni 2026 · BIEN-STICH! 🐝*
