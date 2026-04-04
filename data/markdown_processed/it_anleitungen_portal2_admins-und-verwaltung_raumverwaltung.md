---
title: Leitfaden zur Raumverwaltung in Portal2 für Raum-Manager*innen
source_url_de: https://www.uni-mannheim.de/it/anleitungen/portal2/admins-und-verwaltung/raumverwaltung/
source_url_en: https://www.uni-mannheim.de/en/
category: Services
tags: ['Raumverwaltung', 'Portal2', 'Raumanfragen', 'Buchung', 'Admin', 'Dozent', 'Filter']
language: de
---

# Anleitungen für Raum-Manager\*innen

Als Raum-Manager\*in sind Sie für die Verwaltung einer oder mehrerer Gruppen von Räumen zuständig. Wenn ein Dozent oder Sekretariat eine Nutzung dieser Räume anfragt, werden Sie benachrichtigt. Die Benachrichtigung erfolgt zunächst per E-Mail. Danach erhalten Sie keine weiteren E-Mails vom System, bis Sie sich im Portal2 eingeloggt haben. Erst danach werden Sie bei neuen Meldungen erneut per E-Mail benachrichtigt.

## Wege zur Raumverwaltung

Es gibt mehrere Wege, um die Raumanfragen zu bearbeiten:

1. **Über die Startseite:** Neue Raumanfragen werden als Portalnachricht auf der Startseite angezeigt. Ein Klick auf die Nachricht leitet zur Maske für die Raumverwaltung. Die Nachrichten bleiben sichtbar, bis sie manuell gelöscht werden.
1. **Über das Menü:** Alternativ erreichen Sie die Bearbeitung über den Pfad: `Organisation` > `Räume und Gebäude` > `Raumanfragemanagement` > `Raumanfragen verwalten`.
1. **Über die Suche:** Sie können auch direkt in der Menü-Suche nach „Raumanfragen verwalten“ suchen.

## Konfiguration der Filtermaske

Unabhängig vom gewählten Zugang gelangen Sie zur Übersichtsseite der Raumverwaltung. Im oberen Bereich finden Sie die Konfigurationseinstellungen, mit denen Sie die angezeigten Anfragen filtern, gruppieren und sortieren können.

### 1. Filteroptionen (Anzeige und Filterung)

Sie können festlegen, ob offene, zurückgestellte oder bearbeitete Raumanfragen angezeigt werden sollen. Darüber hinaus können Sie direkt nach folgenden Kriterien filtern:

- Semester
- Startdatum
- Enddatum
- Rhythmus
- Wochentag

**Erweiterte Filterkriterien:**
Wenn die Standardfilter nicht ausreichen, können Sie detaillierter filtern und sortieren nach folgenden Dimensionen:

- **Anfragebezogen:** Anfragestatus (offen, zurückgestellt, erfüllt, erfüllt durch alternativen Raum, abgelehnt), Konflikte (konfliktfrei, Anfragekonflikt, Terminkonflikt, Raumsperrkonflikt), Terminabweichungen (Ausweichtermine, Zeitslotsabweichungen), Anfrageart (nur spezifische/nur unspezifische Raumanfragen), Raumzuordnungsgruppe.
- **Terminbezogen:** Datum, Uhrzeit, Wochentag, Rhythmus, Teilnehmerzahl.
- **Veranstaltungsbezogen:** Veranstaltungsart (Vorlesung, Seminar, Übung etc.), Einrichtung.
- **Personenbezogen:** Bestimmte/r Anfragesteller/-in, bestimmte/r Dozent/-in.

Diese Filterkriterien können gespeichert werden, um sie später über die Dropdownbox auszuwählen.

### 2. Gruppierung und Sortierung

Sie können die angezeigten Raumanfragen wie folgt gruppieren:

- **Veranstaltung/Prüfung:** Gruppierung nach der jeweiligen Veranstaltung oder Prüfung.
- **Raum:** Gruppierung nach dem angefragten Raum.
- **Ohne:** Anzeige aller Anfragen einzeln ohne Gruppierung.

Zusätzlich können Sie die Sortierreihenfolge definieren (z.B. Älteste Raumanfrage zuerst, Beste Raumauslastung zuerst, Neuste Raumanfrage zuerst, etc.) sowie die Anzahl der anzuzeigenden Anfragen festlegen.

## Bearbeiten von Raumanfragen

Unter der Filtermaske sehen Sie die Tabelle der aktuellen Raumanfragen.

**Tabelle und Navigation:**

- **Gruppierung:** Die erste Spalte zeigt je nach Einstellung entweder die Veranstaltung (mit Titel) oder die angefragten Räume (mit Titel).
- **Detailansicht:** Durch Klicken auf den Namen des Raumes gelangen Sie zum jeweiligen Raumplan. Durch Klicken auf den Titel der Veranstaltung gelangen Sie zur [Detailseite](https://www.uni-mannheim.de/it/anleitungen/portal2/allgemein/veranstaltungsdetailseite/).
- **Weitere Spalten:** Diese geben Auskunft über Konflikte, Alternativen, Sitzplatzauslastung, Datum, Uhrzeit, Zeitraum, Dozent/in und Anfragesteller/in.

**Konflikt- und Alternativanzeigen:**

- **Konflikte:** Werden in der Spalte Konflikte angezeigt.
  - *Anfragekonflikt:* Konflikt mit einer anderen offenen Raumanfrage.
  - *Terminkonflikt:* Der Raum ist zum Zeitpunkt bereits vergeben.
  - *Raumsperrkonflikt:* Der Raum ist durch eine Raumsperre belegt.
  - Die Zahl am Konfliktsymbol gibt die Anzahl der Einzeltermine an, an denen der Konflikt besteht. Mit einem Klick auf das Plus können Einzeltermine und deren Konflikte einblendet werden.
- **Alternative Raumanfragen:** Zeigt die Anzahl paralleler Anfragen. Über die Lupe können alle parallel gestellten Anfragen (auch von anderen Verwaltern) in einem Overlay eingesehen werden.

**Aktionen:**
In der Spalte Aktionen sind folgende Optionen verfügbar:

- Raumanfrage erfüllen
- Alternativen Raum zuordnen
- Raumanfrage zurückstellen (später bearbeiten)
- Raumanfrage ablehnen

**Massenbearbeitung:**
Über die Massenbearbeitung können Sie mehrere ausgewählte Anfragen gleichzeitig ablehnen oder zulassen.

> **Hinweis für Raumverwalter:** Sie können nur Alternativräume vergeben/zuweisen, die auch von Ihnen verwaltet werden. Sollte ein Raumwunsch nicht bestätigt werden können, empfehlen wir, sich direkt mit dem/der Anfragesteller/-in in Verbindung zu setzen, damit dieser/diese die Anfrage stornieren und einen alternativen Raum anfragen kann.

## Mehrfach-Raumbuchungen für Department-Admins

Für Department-Admins, die gleichzeitig Raummanager\*innen sind, ist die gleichzeitige Buchung mehrerer Räume möglich.

**Vorgehen:**

1. Rufen Sie die Veranstaltung auf, für die die Mehrfach-Raumbuchung erfolgen soll, und gehen Sie in die **Veranstaltungsbearbeitung**.
1. Navigieren Sie zu **Termine und Räme** und legen Sie einen Termin an.
1. Wenn die Rechte vorhanden sind, erscheint neben dem normalen Buchungssymbol ein zweites Tür-Symbol für die Mehrfach-Raumbuchung.
1. Wählen Sie alle gewünschten Räume mit einem Haken aus und klicken Sie auf **Auswahl hinzufügen**.
1. Das System erstellt automatisch eine eigene Terminserie für jeden gebuchten Raum.
