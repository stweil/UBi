---
title: Verwaltung von Veranstaltungsbelegungen und -verteilungen im Portal
source_url_de: https://www.uni-mannheim.de/it/anleitungen/portal2/admins-und-verwaltung/department-admins-und-studienkoordination/zeitraeume-anhaengen/
source_url_en: https://www.uni-mannheim.de/en/
category: Services
tags: ['Belegungsverfahren', 'Verteilungsverfahren', 'Zeitraumzuordnung', 'Veranstaltung', 'Studienkoordination', 'Portal2']
language: de
---

# Verwaltung von Veranstaltungsbelegungen und -verteilungen

Diese Anleitung beschreibt die notwendigen Schritte und Verfahren zur Einrichtung von Belegungen und Verteilungen für Veranstaltungen im Portal.

> **Hinweis:** Eine allgemeine Erklärung zu Belegungen und zu den Einstellungen, die nötig sind, um Belegungen durch Studierende zu ermöglichen, finden Sie [in unserer Dokumentation zur Veranstaltungsbelegung](https://www.uni-mannheim.de/it/anleitungen/portal2/lehrende/veranstaltungsbelegung/).

## 📚 Grundlagen: Zeitraumarten und Verfahren

Um eine Veranstaltungsbelegung zu ermöglichen, müssen jeder Veranstaltung Zeiträume zugeordnet werden. Diese Zeiträume definieren, wer und wann an einer Veranstaltung teilnehmen kann.

- **Belegungsverfahren:** Definiert, wie sich Studierende für die Veranstaltungen anmelden können.
- **Verteilungsverfahren:** Bestimmt, wie die Studierenden den Kursen zugeordnet werden.

### ⏱️ Zeitraumarten

(Keine spezifischen Details im Originaltext, aber der Abschnitt dient der Einleitung.)

## ⚙️ Belegungsverfahren (Enrollment Procedures)

Die Wahl des Belegungsverfahrens bestimmt die Art der Anmeldung der Studierenden.

### Überblick der Verfahren

- **Gruppenpriorität:** Studierende ordnen Alternativen in einer Rangfolge. Wird verwendet, wenn eine Veranstaltung aus mehreren inhaltlich gleichen Parallelgruppen besteht.
- **Modulpriorität:** Studierende vergeben Alternativen auf Modulebene, wenn die Inhalte der Veranstaltungen voneinander abweichen (z.B. bei Hauptseminaren).
- **Echtzeitbelegung:** Geeignet für Vorlesungen mit ausreichender Kapazität. Anmeldungen werden direkt zugelassen, da keine Auswahl der Studierenden notwendig ist.
  - *Sonderfall:* Eine Echtzeitbelegung kann mit anschließender Verteilung eingerichtet werden, bei der alle Angemeldeten per Losverfahren zugelassen werden. Dies erfordert die Kontaktaufnahme mit dem zuständigen Studiengangsmanager oder dem Portal-Team.

### Detaillierte Verfahrensübersicht

| Bezeichnung | Eigenschaften | Auswirkungen |
| :--- | :--- | :--- |
| **Echtzeitbelegung ZU** | Belegung und automatische Zulassung (TN sind ZU) | Keine TN-Begrenzung |
| **Echtzeitbelegung ZU FCFS** | Belegung und automatische Zulassung bis max. TN (TN sind ZU) | First-come-first-serve! |
| **Echtzeitbelegung AN** | Belegung (TN sind AN) | Ein Verteilverfahren muss durchgeführt werden |
| **Echtzeitbelegung Stg. ZU/AN** | Belegung und automatische Zulassung für Studierende mit dieser Veranstaltung in PO (TN sind ZU, andere TN sind AN) | Ein Verteilverfahren muss durchgeführt werden |
| **Gruppenpriorität ALLE** | Verpflichtende Priorisierung aller Parallelgruppen; Prioritäten sind vorbelegt; TN sind AN | Ein Verteilverfahren ist notwendig |
| **Gruppenpriorität mit 2 Alternativen (= 3 Prioritäten)** | Eine Gruppe bevorzugt (Prio 1); Alternativen dürfen mehrfach vergeben werden (Prio 2/3) | Ein Verteilverfahren ist notwendig; Psychologischer Effekt |
| **Modulpriorität ALLE** | Verpflichtende Priorisierung aller Veranstaltungen; Prioritäten sind vorbelegt; TN sind AN | Ein Verteilverfahren ist notwendig |
| **Modulpriorität mit 2 Alternativen (= 3 Prioritäten)** | Eine Veranstaltung bevorzugt (Prio 1); Alternativen dürfen mehrfach vergeben werden (Prio 2/3) | Ein Verteilverfahren ist notwendig; Psychologischer Effekt |

## 📊 Verteilungsverfahren (Distribution Procedures)

Die Wahl des Verteilungsverfahrens erfolgt je nach Art der Belegungsverfahren.

### Für Echtzeit- und Gruppenpriorität

| Bezeichnung | Eigenschaften |
| :--- | :--- |
| **Losverfahren** | Vergabe von Losnummern; Zufällige Verteilung nach Losnummer |
| **Sortiertes Verfahren** | Sortierung nach: Studiengang (Studiengänge der Veranstaltung zuerst) und Fachsemester (hohe Semester zuerst); Vergabe von Losnummern; Zufällige Verteilung nach Gruppenprioritäten |
| **Sortiertes Verfahren mit Konfliktknüpfung** | Zusätzliche Überprüfung auf Konflikte mit anderer Zulassung; Falls Konflikt, Auswertung der nächsten abgegebenen Priorität |
| **Rücknahme der Verteilung** | (Keine Details angegeben) |

### Für Modulpriorität

| Bezeichnung | Eigenschaften |
| :--- | :--- |
| **Modulverteilung** | Vergabe von Losnummern; Zufällige Verteilung nach Modulprioritäten |
| **Modulverteilung mit Sortierung** | Sortierung nach Studiengang und Fachsemester; Vergabe von Losnummern; Zufällige Verteilung nach Modulprioritäten |
| **Rücknahme der Verteilung** | (Keine Details angegeben) |

## 🔗 Zeitraum zuordnen

Um eine Belegung zu ermöglichen, muss jeder im Portal² belegbare Veranstaltung mindestens einen Belegungszeitraum zugeordnet bekommen.

**Vorgehen:**

1. Öffnen Sie die Bearbeitungsansicht der Veranstaltung (z.B. mit der Rolle „Department-Admin“).
1. Navigieren Sie zum Reiter „Zeiträume“. Hier werden alle Zeitraumgruppen angezeigt, die der Veranstaltung angehängt wurden.
1. **Verknüpfung:** Zeitraumgruppen müssen nur einmalig verknüpft werden, da sie semesterunabhängig sind. Die spezifischen Laufzeiten müssen anschließend vom Studiengangsmanagement beim Portal² Team angefordert werden.
1. **Zuordnung:** Klicken Sie auf „Zeitraumgruppe zuordnen“. Setzen oder entfernen Sie dort einen Haken bei der gewünschten Zeitraumgruppe und bestätigen Sie mit „Zuordnungen aktualisieren“.

> **Wichtig:** Achten Sie darauf, dass sich mehrere Belegungsverfahren für dieselbe Rolle (meist Student\*in) nicht zeitlich überschneiden dürfen. Andernfalls kann das System kein eindeutiges Belegungsverfahren feststellen und die Belegung wird blockiert.

## ⚠️ Wichtige Hinweise für einen reibungslosen Ablauf

Um einen reibungslosen Ablauf der Belegung und Verteilung zu gewährleisten, beachten Sie folgende Zeitrahmen und Einschränkungen:

### Zeitliche Planung

- Die Konfiguration der Veranstaltungsbelegung (inkl. Zeitraum, Belegverfahren, Zuordnungen) sollte **mindestens 1 Woche** vor Beginn der Studierenden-Belegung erfolgen.
- Zwischen dem Ende der Belegungsphase und der Bekanntgabe der Verteilung sollten **3 Werktage** eingeplant werden.
- Zwischen der Bekanntgabe der Verteilung und dem Start der Veranstaltung sollten **2 Werktage** eingeplant werden.

### Verbotene Änderungen während der Belegungsphase

Während der Belegungsphase dürfen folgende Änderungen an Veranstaltungen **NICHT** vorgenommen werden:

- Hinzufügen oder Löschen von Parallelgruppen.
- „Fällt aus“-Setzen von Parallelgruppen.
- Hinzufügen oder Löschen von Veranstaltungen in zu belegenden Modulen bei „Belegung mit Modulpriorität“.
- Hinzufügen oder Löschen von (Teil-)Modulen im Prüfungsordnungsbaum.
- Bearbeiten von Regeln an Modulen.
- Ändern der Zeitraumgruppen der zu belegenden Veranstaltungen.
- Manuelle Platzvergabe (Zulassung, Änderung) einzelner Studierender.

## 📥 Support und Dokumentation

- **Fehlender Zeitraum:** Sollte kein passender Zeitraum in der Liste zu finden sein, wenden Sie sich bitte mit folgendem ausgefüllten Formular an das Portal-Team: [Download Formular (DOCX)](https://portal2.uni-mannheim.de/portal2/download/help/Formular_Zeitraumgruppe.docx).
- **Weitere Details zur Platzvergabe:** Für detaillierte Informationen zur Verteilung und Platzvergabe lesen Sie bitte unsere [Anleitungen zur Verteilung und Platzvergabe](https://www.uni-mannheim.de/it/anleitungen/portal2/admins-und-verwaltung/department-admins-und-studienkoordination/verteilung-und-platzvergabe-fuer-veranstaltungen/).
