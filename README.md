# Narrentreffen 2027 – Planungs-Mockup
**Binkerzunft Boll e.V. · Sauldorf-Boll · 5.–7. Februar 2027**

---

## Was ist das?

Eine interaktive Planungshilfe für das Narrentreffen als **einzelne HTML-Datei** – kein Server, keine Installation, kein Internet nötig.

Die Datei kann einfach per E-Mail, WhatsApp oder USB-Stick weitergegeben werden.

---

## Starten

Datei `Narrentreffen-2027-Mockup.html` im Browser öffnen (Chrome oder Firefox empfohlen).

---

## Bereiche im Überblick

| Tab | Inhalt |
|-----|--------|
| 📊 **Dashboard** | Gesamtstatus, Fortschrittsbalken, Zeitplan T-Minus |
| 📋 **Zunftanmeldung** | Liste der 50 NVH-B Zünfte, Anmeldestatus, Filter nach Landschaft |
| 🎭 **Umzug** | Aufstellungsreihenfolge der Zünfte, Positionsnummern, Streckenlänge 2,2 km |
| 📅 **Programm** | Detailprogramm Fr–So mit allen Veranstaltungen |
| 🏨 **Unterkunft** | Quartierplan, Belegung, Anfahrt |
| 🎟 **Tickets** | Verkaufsübersicht, Preiskategorien, Auslastung |
| 🎰 **Tombola** | Losverkauf, Preisübersicht, Verlosungsplan |
| 💶 **Finanzen** | Budget, Einnahmen/Ausgaben, Rücklagen |
| 🙋 **Helfer** | Schichtplanung (s. unten), Bereichsübersicht, Anmeldung |
| 🚌 **Logistik** | Parkplätze, Shuttle, Infrastruktur, Sicherheit |
| 🍺 **Narrenstände** | Standliste entlang der Umzugsstrecke, WC/Müll-Punkte |
| 📨 **Kommunikation** | Briefvorlagen, E-Mail-Status, Pressemitteilungen |
| 📞 **Kontakte** | Telefonliste aller Ansprechpartner, Export als CSV |
| 🏟 **Reithalle Setup** | Aufbauplan, Ausstattungslisten, Timeline, Budget 24.190 € |
| 🏅 **ZM-Empfang** | Saalplan Gemeindehalle, Bewirtungsplan, Programm-Ablauf |

---

## Helfer-Schichtplanung

Der **🙋 Helfer**-Tab ist in 5 Unter-Bereiche gegliedert:

### 📋 Übersicht
Aktuelle Besetzungsstatistik mit der Schichtmatrix (12 Bereiche × 3 Tage) und Bereichssteckbriefen.

### 📊 Schicht-Planer ← **das Herzstück**
Interaktive Einteilung per **Drag & Drop**:
- Links: Helfer-Pool mit allen verfügbaren Personen
- Rechts: Grid aus 12 Bereichen × 8 Schichten
- Helfer einfach von links in eine Zelle ziehen
- Farbcode: 🔴 Unterbesetzt · 🟡 Teilbesetzt · 🟢 Vollbesetzt
- **⚡ Auto-Assign**: füllt alle offenen Stellen automatisch nach Verfügbarkeit
- **⬇ CSV-Export**: komplette Einteilung als Excel-Datei
- Einteilung wird automatisch im Browser gespeichert (bleibt beim Neuladen erhalten)

### 👤 Helfer-Karten
Persönliche Übersicht pro Helfer: zugewiesene Schichten, Einsatzbereiche, Gesamtstunden. Jede Karte kann einzeln ausgedruckt werden.

### 📈 Statistik
Besetzungsgrad nach Bereich und nach Schicht, Stundenübersicht aller Helfer.

### ➕ Anmeldung
Formular zur Helfer-Neuanmeldung + Liste der bereits registrierten Helfer.

---

## Was sind Echtdaten, was Platzhalter?

| Bereich | Status |
|---------|--------|
| 50 Zünfte (NVH-B) | ✅ echte Namen und Landschaften |
| Veranstaltungsorte | ✅ Reithalle (3.000 P.), Zelt (1.500 P.), Gemeindehalle (250 P.) |
| Umzugsstrecke | ✅ 2.200 m mit WC- und Müllpunkten |
| Helfer-Stammdaten (38 Personen) | ⚠ Demo-Daten, bitte ersetzen |
| Finanzzahlen | ⚠ Schätzwerte, bitte aktualisieren |
| Kontaktdaten | ⚠ Beispieldaten, bitte ergänzen |

---

## Daten speichern

Die Datei selbst speichert **nichts dauerhaft** – sie hat keinen Server im Hintergrund.

- **Schichteinteilungen** (Drag & Drop) werden im Browser-Speicher (localStorage) des jeweiligen Computers gesichert
- Alle anderen Eingaben (Formulare, Checkboxen) gehen beim Schließen verloren
- Empfehlung: Änderungen per **CSV-Export** sichern

Für gemeinsames Arbeiten muss die Datei nach Änderungen immer neu weitergegeben werden.

---

## Teilen

Die HTML-Datei ist vollständig eigenständig – einfach die Datei `Narrentreffen-2027-Mockup.html` verschicken. Keine weiteren Dateien notwendig.

---

## Technisches

- Läuft lokal im Browser (Chrome, Firefox, Edge, Safari)
- Kein Internet erforderlich (Chart.js wird einmalig von CDN geladen – falls offline, erscheinen keine Diagramme)
- Funktioniert auf Windows, Mac und Linux
- Datei ist ca. 600 KB groß

---

*Erstellt für Binkerzunft Boll e.V. · Stand: Juni 2026 · Schlachtruf: BIEN-STICH!* 🐝
