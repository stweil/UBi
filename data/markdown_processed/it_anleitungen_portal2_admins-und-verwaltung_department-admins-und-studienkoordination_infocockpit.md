---
title: InfoCockpit Konfiguration und Nutzung im Portal²
source_url_de: https://www.uni-mannheim.de/it/anleitungen/portal2/admins-und-verwaltung/department-admins-und-studienkoordination/infocockpit/
source_url_en: https://www.uni-mannheim.de/en/
category: Benutzung
tags: ['InfoCockpit', 'Portal²', 'Konfiguration', 'Studieninformation', 'Erstsemester', 'Studierende', 'Administration']
language: de
---

# InfoCockpit: Verwaltung und Konfiguration im Portal²

Das InfoCockpit dient dazu, Studierenden zielgruppenspezifische Informationen auf der Startseite des Portal² bereitzustellen. Die Inhalte können von der Zulassungsstelle, den Studienbüros, dem Studiengangsmanagement und dem Akademischen Auslandsamt gepflegt werden.

## 1. Überblick und Hintergrund

Auf der Portal²-Startseite werden Informationen für verschiedene Zielgruppen (z. B. Erstsemester oder spezifische Studiengangskohorten) angezeigt. Die Pflege dieser Inhalte erfolgt über das „InfoCockpit“.

**Mögliche Inhalte:**

- Orientierung an der Universität
- Aktuelle Hinweise
- Veranstaltungen und Prüfungen
- Fristen

Das InfoCockpit ermöglicht die Pflege verschiedener Gestaltungselemente, die in diesem Leitfaden detailliert beschrieben werden.

## 2. Gestaltungselemente des InfoCockpits

Je nach Zielgruppe werden unterschiedliche Elemente zur Darstellung von Informationen genutzt:

### 2.1 Informationen für Erstsemester

Es stehen vier Anzeigeoptionen zur Verfügung:

- **Obere Kachel:** Wird für studiengangsspezifische Informationen genutzt (Titel, Text, Verlinkung).
- **Mittlere Kachel (Teaser Box TYPO3):** Geeignet für Einführungsveranstaltungen und wichtige ToDos.
- **Untere Kachel (Teaser Box TYPO3):** Wird für allgemeine Informationen genutzt.
- **Verlinkung in der rechten Spalte:** Dient für allgemeine und studiengangsspezifische Informationen (Titel, Text, Verlinkung).

### 2.2 Informationen für Studierende

Aktuell werden drei Hauptoptionen genutzt:

- **News-Kachel:** Wird zentral für alle gepflegt und erlaubt keine Differenzierung.
- **Untere Kachel (Teaser Box TYPO3):** Für allgemeine Informationen.
- **Verlinkung in der rechten Spalte:** Für allgemeine und studiengangsspezifische Informationen.

**Weitere Optionen:**

- **Obere Kachel:** Für studiengangsspezifische Informationen.
- **Mittlere Kachel (Teaser Box TYPO3):** Für allgemeine Informationen.

### 2.3 Differenzierungsmöglichkeiten

Die angezeigten Informationen (mit Ausnahme der News-Kachel) können anhand folgender Kriterien zielgruppenspezifisch unterschieden werden:

- Bewerber/Studierender
- Abschluss (Bachelor/Master)
- Studienfach
- Bildungsinländer/-ausländer
- Fachsemester

### 2.4 Darstellung der Inhalte

Die Inhalte werden in TYPO3 angelegt und können auf zwei Arten im Portal angezeigt werden:

- Inhalte der TYPO3-Seite im Portal anzeigen.
- Komplette TYPO3-Seite in neuem Fenster öffnen.

## 3. Konfiguration des InfoCockpits

Die Konfiguration erfolgt im Portal² über den Pfad: **Administration –> InfoCockpit –> Konfigurieren**. Hier kann ein neuer oder ein bestehender Eintrag gesucht und bearbeitet werden.

### 3.1 Anlegen neuer Inhaltselemente

Zur Definition eines Inhaltselements müssen verschiedene Parameter ausgefüllt werden:

| Feld | Beschreibung | Auswahlmöglichkeiten / Hinweise |
| :--- | :--- | :--- |
| **Abschluss und Studienfach**\* | Definiert, für welchen Studiengang das Element sichtbar ist. | Kombination von Abschluss und Studienfach (Mehrfachauswahl möglich). *Hinweis: „(nur studiengangsunabhängige Informationen anzeigen)“ darf nicht gleichzeitig mit anderen Kombinationen ausgewählt werden.* |
| **Fakultät** | Definition des Corporate Design für das Inhaltselement. | Auswahl über Dropdown Menü. |
| **Rolle**\* | Definiert die Zielgruppe: Bewerber\*in, Student\*in (vorläufig), Student\*in oder eine Kombination. | Auswahl über Anklicken der Kästchen (Mehrfachauswahl möglich). *Hinweis: Hinter „Student\*in (vorläufig)“ verbergen sich die aus Mobility-Online (MO) übertragenen Incoming-Bewerber.* |
| **Semester** | Nur für die Rolle Student\*in: Definiert das Fachsemester. | Eintragen als Ganzzahl. Bei mehreren Semestern durch Komma trennen (z.B. 2,4,6). Unterstützte Zahlen: 1..99. |
| **Hochschulzugangs-berechtigung**\* | Definiert die Berechtigungsgruppe. | Auswahl über Anklicken der Kästchen (Mehrfachauswahl möglich). Optionen: nicht EU-Ausländer/in ohne dt. HZB (A), Ausländer/in mit dt. HZB (B), dt. Staatsbürger/in (D), EU-Ausländer/in ohne dt. HZB (E), Keine Angabe (–). |
| **Gültigkeit**\* | Definiert den Zeitraum, in dem das Element angezeigt werden soll. | Auswahl über Kalender. |
| **Art des Inhaltselements und Anzeigemodus**\* | Definiert das Layout und die Platzierung. | Auswahl über Dropdown Menü. Kombination aus Elementart (Link rechte Spalte, Obere Kachel, etc.) und Anzeigemodus (Innerhalb des Portal² oder In neuem Fenster). |
| **Priorität** | Definiert die Reihenfolge der Elemente. | Eintragen als Zahl. Je höher die Zahl, desto weiter vorne wird das Element angezeigt. |
| **URL für die Verlinkung des Inhaltselementes**\* | Die zu verlinkende Quelle. | Angabe einer (TYPO3-)URL. |
| **URL für die Verlinkung des Inhaltselementes EN**\* | Die englische Übersetzung der Verlinkung. | Angabe einer (TYPO3-)URL. Falls keine Übersetzung vorhanden, die deutsche URL erneut eingeben. |
| **URL für den Teaser des Inhaltselementes** | Nur für „mittlere Kachel“ und „untere Kachel“. | Angabe der TYPO3-URL für die Teaserbox. |
| **URL für den Teaser des Inhaltselementes EN** | Nur für „mittlere Kachel“ und „untere Kachel“. | Angabe der TYPO3-URL für die englische Teaserbox. |
| **Titel des Inhaltselementes** | Nur für „obere Kachel“ und „Link rechte Spalte“. | Eingabe des Titels. |
| **Titel des Inhaltselementes EN** | Nur für „obere Kachel“ und „Link rechte Spalte“. | Eingabe des englischen Titels. Falls nicht vorhanden, den deutschen Titel eingeben. |
| **Text des Inhaltselementes** | Nur für „obere Kachel“ und „Link rechte Spalte“. | Eingabe des Textes (kurz, ohne Formatierung). |
| **Text des Inhaltselementes EN** | Nur für „obere Kachel“ und „Link rechte Spalte“. | Eingabe des englischen Textes. Falls nicht vorhanden, den deutschen Text eingeben. |
| **Schlüsselwort** | Optionales Schlüsselwort zur besseren Auffindbarkeit. | Freie Eingabe. |

### 3.2 Suchen von Inhaltselementen

Über die Suchmaske können die verschiedenen Parameter definiert werden (z.B. alle Elemente der Philosophischen Fakultät). Die Ergebnisse werden tabellarisch angezeigt und können dort ausgewählt und bearbeitet werden.

### 3.3 Tipps zur Konfigurationsmaske

- **Schlüsselwörter:** Die Vergabe von Schlüsselwörtern erleichtert die Suche nach bestehenden Links.
- **Ergebnistabelle:** Die Ergebnisse können personalisiert werden, um relevante Informationen zuerst zu sehen.
- **Standardabfragen:** Häufige Suchanfragen können als Standardabfrage gespeichert werden.
- **PDF vs. TYPO3:** Für Inhalte wie Begrüßungsschreiben kann alternativ eine TYPO3-Seite erstellt werden, die im Portal angezeigt wird, anstatt ein PDF zu verwenden.

## 4. Vorschau und Statistik-Download

### 4.1 Vorschau der Inhalte

Vor dem Veröffentlichen können die Inhalte im Vorschau-Modus geprüft werden:
**Administration –> InfoCockpit –> Vorschau**
Hier können Parameter wie Abschluss, Studienfach, Rolle, HZB, Fachsemester und Gültigkeit definiert werden. Alternativ kann die Matrikelnummer oder Uni-ID zur Prüfung eines spezifischen Nutzers verwendet werden (durch Umschalten der Suchmaske).

### 4.2 Download der Statistik

Die InfoCockpit-Statistik kann über den Menüpunkt **Administration –> InfoCockpit –> Download Statistik** heruntergeladen werden. Die betroffenen Gruppen sind Bewerber\*innen und Studierende.

**Erläuterung der Statistik-Tabelle:**

- **Datum:** Tag der statistischen Erfassung.
- **Abschluss/Studienfach:** Bezeichnet den Abschluss bzw. das Studienfach des Benutzers.
- **Rolle:** Codes wie `65` (Bewerber\*in), `6` (Student\*in (vorläufig)) oder `5` (Student\*in).
- **Fachsemester:** Wird nur bei Studierenden geprüft. Bei Bewerbern wird immer NULL gespeichert.
- **HZB:** Bezeichnet die Hochschulzugangsberechtigung (A, B, D, E).
- **Aufgerufener Inhalt:** `home` bezieht sich auf die Startseite. Eine Zahl ist die ID des geöffneten InfoCockpit-Inhaltselementes.
- **Aufrufhäufigkeit:** Wie oft der entsprechende Inhalt aufgerufen wurde.

______________________________________________________________________

## Kontakt bei Fragen oder Problemen mit dem InfoCockpit

Für Rückfragen steht Ihnen Alexandra Theobalt zur Verfügung:

**Alexandra Theobalt**
Leitung Koordinationsstelle Studieninformationen

- **Adresse:** Universität Mannheim, Dezernat II – Studienangelegenheiten, L 1, 1 – Raum 115, 68161 Mannheim
- **Telefon:** +49 621 181-3157
- **E-Mail:** [alexandra.theobalt@uni-mannheim.de](mailto:alexandra.theobalt@uni-mannheim.de)
- **Web:** [Informationen zur Studienwahl](/studium/vor-dem-studium/)
