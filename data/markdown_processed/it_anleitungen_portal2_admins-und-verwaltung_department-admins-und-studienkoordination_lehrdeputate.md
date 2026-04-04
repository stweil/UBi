---
title: Verwaltung von Lehrdeputaten und Stundenkonten in Portal²
source_url_de: https://www.uni-mannheim.de/it/anleitungen/portal2/admins-und-verwaltung/department-admins-und-studienkoordination/lehrdeputate/
source_url_en: https://www.uni-mannheim.de/en/
category: Services
tags: ['Lehrdeputat', 'Portal²', 'Verwaltung', 'Stunden', 'Credits', 'Lehrpersonen', 'Soll', 'Ist']
language: de
---

# Verwaltung von Lehrdeputaten in Portal²

Dieser Leitfaden beschreibt die Verwaltung von Lehrdeputaten (Lehrstundenkonten) innerhalb des Portals² für Administratoren und Studienkoordinatoren. Die Funktionen gliedern sich in die Übersicht, die Verwaltung der Soll-Deputate (geplante Stunden) und die Verwaltung der Ist-Deputate (tatsächlich geleistete Stunden).

## 1. Übersicht: Deputate meiner Einrichtung

Dieser Bereich dient als zentrale Übersicht über das Lehrdeputats-Soll, die geleisteten Ist-Stunden und mögliche Minderungen für die Lehrpersonen der Einrichtung.

**Funktionalität:**

1. **Suche:** Über eine Suchmaske können Personen nach Name oder Funktion (z.B. Lehrperson) gefiltert werden.
1. **Anzeige:** Nach der Suche werden die Daten tabellarisch aufgelistet und zeigen für das aktuelle Semester folgende Informationen:
   - Lehrdeputats-Soll
   - Übertrag aus dem Vorsemester
   - Summe der Minderungen
   - Summe der angerechneten SWS
   - Übertrag in das Folgesemester
1. **Semesterwechsel:** Es ist möglich, das angezeigte Semester zu wechseln, um Überträge aus früheren Perioden zu prüfen.

**Aktionsmöglichkeiten:**

- **Lehrdeputatserklärung für Einrichtung:** Erzeugt eine Excel-Datei mit den Lehrdeputatserklärungen für alle gefundenen Personen.
- **Übertrag übernehmen:** Übernimmt alle eingetragenen Überträge in das Folgesemester.
- **Einzelübertrag übernehmen:** Übernimmt den Übertrag für eine spezifische Person mit einem Klick.
- **Detailansicht:** Zeigt die Übersichtsseite für eine einzelne Person, welche alle Veranstaltungen und Minderungen listet und von wo aus eine individuelle Lehrdeputatserklärung erstellt werden kann.

## 2. Soll-Deputate tabellarisch bearbeiten (Geplante Stunden)

In diesem Modul wird das geplante Lehrdeputat (Soll-Deputat) der Lehrpersonen verwaltet.

**Funktionalität:**

1. **Suche:** Mittels einer Suchmaske können Personen identifiziert werden (Name, Funktion = Lehrperson).
1. **Anzeige:** Die Ergebnisse zeigen tabellarisch folgende Daten für das aktuelle Semester:
   - Übertrag aus dem Vorsemester
   - Lehrdeputats-Soll
   - Optionaler Vermerk
   - Eventuelle Minderungen
1. **Bearbeitungsmöglichkeiten:**
   - **Übertrag anpassen:** Der automatisch ausgefüllte Übertrag aus dem Vorsemester kann manuell korrigiert werden.
   - **Soll-Stunden eintragen:** Das geplante Soll-Deputat kann direkt eingegeben werden.
   - **Vermerk verfassen:** Hinzufügen von erklärenden Vermerken.
   - **Minderungen verwalten:** Neue Minderungen können hinzugefügt werden (Angabe des Minderungsgrunds, geminderte SWS, optionaler Vermerk). Bestehende Minderungen können entfernt werden.

## 3. Ist-Deputate tabellarisch bearbeiten (Tatsächlich geleistete Stunden)

Dieses Modul dient zur Verwaltung der Ist-Deputate, die direkt an spezifische Veranstaltungen gebunden sind.

**Funktionalität:**

1. **Suche:** Eine Suchmaske ermöglicht die Eingrenzung auf spezifische Veranstaltungen.
1. **Anzeige:** Die gefundenen Veranstaltungen werden tabellarisch aufgelistet.
1. **Rollenzuweisung:** Ist-Deputate können sowohl an **verantwortliche** als auch an **durchführende** Lehrpersonen vergeben werden.
   - *Hinweis:* In der Übersicht weisen kursiv geschriebene Namen auf die Rolle als durchführende Lehrperson hin, gefolgt von der Anzahl der durchgeführten Einzeltermine in Klammern. Die Namen verantwortlicher Lehrpersonen sind in normaler Schriftart dargestellt.
1. **Berechnung der Ist-Stunden (SWS):** Die SWS einer Veranstaltung werden zur Berechnung der Ist-Stunden für die beteiligten Dozierenden herangezogen:
   - **Nur eine verantwortliche Lehrperson:** Die gesamten SWS werden dieser Person angerechnet.
   - **Mehrere verantwortliche Lehrpersonen:** Die SWS werden gleichmäßig auf diese Personen aufgeteilt.
   - **Durchführende Lehrpersonen:** Die SWS werden entsprechend der durchgeführten Einzeltermine aufgeteilt. Eventuelle verantwortliche Lehrpersonen werden in diesem Fall nicht berücksichtigt.

**Aktionsmöglichkeiten:**

- **Vorschlagswert übernehmen:** Der automatisch berechnete Vorschlagswert wird einer Lehrperson angerechnet. Alternativ kann ein abweichender Wert manuell eingegeben werden.
- **Detailansicht:** Über die Aktionssymbole kann direkt zur Detailansicht oder zur Bearbeitungsmaske der jeweiligen Veranstaltung gesprungen werden.
