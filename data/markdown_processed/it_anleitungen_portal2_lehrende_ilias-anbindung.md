---
title: Anleitung zur Einrichtung und Nutzung der ILIAS E-Learning Plattform
source_url_de: None
source_url_en: https://www.uni-mannheim.de/en/
category: Benutzung
tags: ['ILIAS', 'E-Learning', 'Portal²', 'Kursanleitung', 'Veranstaltung', 'Admin', 'Teilnehmende']
language: de
---

# ILIAS E-Learning Plattform: Leitfaden für Lehrende und Administratoren

Diese Seite dient als technische Anleitung für die Arbeit mit dem [E-Learning System ILIAS](http://ilias.uni-mannheim.de), das im Rahmen der Universität Mannheim eingesetzt wird. Für inhaltliche Ressourcen zu digitaler Lehre und die Verwendung von ILIAS zur Unterstützung dieser, besuchen Sie bitte die ILIAS-Kurse „Matilde – Wiki zum digitalen Lehren und Lernen“ und „Digitalisierung der Lehre“.

## 🧭 Übersicht und Dashboard

Beim Einloggen in ILIAS wird das Dashboard automatisch geladen oder über den Button „Dashboard“ im linken Menü oben erreicht. Hier werden alle ILIAS-Mitgliedschaften in Kursen und Gruppen angezeigt, sowohl aus dem aktuellen als auch aus vergangenen Semestern.

Neben dem Kurs- bzw. Gruppennamen befindet sich ein Aktionsfeld mit Befehlen, die auch nach Anklicken des Namens gewählt werden können. Um ein Kurs- oder Gruppenmanagement durchzuführen, muss zunächst auf den Namen geklickt werden.

## ⚙️ ILIAS-Kurs für eine Veranstaltung anlegen (Verknüpfung)

Um einen ILIAS-Kurs anzulegen, muss vorab eine Portal² Veranstaltung angelegt sein. Anschließend wird die E-Learning (ILIAS) Anbindung über Portal² aktiviert.

### Voraussetzungen und Zugänge

Die notwendigen Rechte hängen von Ihrer Rolle ab:

- **Department-Admin:** E-Learning-Einstellungen finden Sie unter „Lehrorganisation" > „Veranstaltungen meiner Einrichtung“.
  - *Hilfe zur Nutzung der Übersichtsseite:* [Hier](https://www.uni-mannheim.de/it/anleitungen/portal2/admins-und-verwaltung/department-admins-und-studienkoordination/veranstaltungsmanagement/)
- **Lehrperson:** E-Learning-Einstellungen finden Sie unter „Lehrorganisation" > „Meine Veranstaltungen“.
  - *Hilfe zur Nutzung der Übersichtsseite:* [Hier](https://www.uni-mannheim.de/it/anleitungen/portal2/admins-und-verwaltung/department-admins-und-studienkoordination/veranstaltungsmanagement/)

### Aktivierung der ILIAS-Verknüpfung

1. Navigieren Sie zur Bearbeitungsseite der gewünschten semesterabhängigen Veranstaltung (Parallelgruppe).
1. Klicken Sie auf den Reiter „E-Learning“, um die Einstellungen zu öffnen.

**Mögliche Szenarien:**

- **Keine Zuordnung:** Wird der Hinweis „Es existiert keine Zuordnung zu externen Systemen“ angezeigt, ist ILIAS noch nicht aktiviert. Klicken Sie auf **„Mit E-Learning-System (ILIAS) verknüpfen“**.
- **Bereits aktiviert:** Ist bereits ein Eintrag vorhanden (Option, Kurstitel, Lehrpersonen etc.), ist ILIAS aktiv.
- **Änderung der Zuordnungsart:** Um die Art der Zuordnung zu ändern (z.B. von Option 1 zu Option 2), müssen Sie zuerst die bestehende ILIAS-Verknüpfung deaktivieren und anschließend neu verknüpfen.

**Im Verknüpfungsfenster:**

1. Wählen Sie im ersten Feld **„ILIAS“**.

1. Wählen Sie im zweiten Feld die gewünschte Option:

   - **Option 1: „jede Parallelgruppe als separaten, eigenständigen Kurs“**
     Diese Option eignet sich für Parallelgruppen, die unabhängig von anderen Gruppen sind oder keine weiteren Parallelgruppen in der Veranstaltung gibt. Es wird ein separater ILIAS-Kurs für jede Parallelgruppe erstellt.
   - **Option 2: „alle Parallelgruppen als Gruppen eines gemeinsamen Kurses“**
     Es wird ein zentraler ILIAS-Kurs für die semesterunabhängige Veranstaltung erstellt, und für jede aktivierte Parallelgruppe wird eine zugehörige ILIAS-Gruppe angelegt. Die Namen werden dabei übernommen.

> **⚠️ Wichtig: Umgang mit Optionenwechsel**
> Wenn Sie von Option 2 zu Option 1 wechseln (oder umgekehrt), wird der bereits erstellte Kurs archiviert und ein neuer Kurs wird erstellt. Sie können nicht auf beide Kurse gleichzeitig zugreifen, da immer einer im Archiv ist.

**Link zum ILIAS-Kurs:**
Der direkte Link zur ILIAS-Gruppe finden Sie auf der Detailansicht unter dem Tab „Parallelgruppen / Termine“ neben „Details einblenden“. Beachten Sie, dass die Aktivierung bis zu 5 Minuten dauern kann.

## 🧑‍🎓 Teilnehmende auf Inhalte zugreifen lassen (Synchronisation)

Damit zugelassene Teilnehmende (Mitglieder) auf die ILIAS-Inhalte zugreifen können, müssen diese freigeschaltet werden. Dies erfolgt direkt in ILIAS über den Link **„Portal²-Mitglieder“** (als ILIAS-Admin in der Navigation rechts).

**Wichtige Hinweise zur Synchronisation:**

- **Zeitpunkt der Übernahme:** Übernehmen Sie die Teilnehmenden **erst dann**, wenn die Ergebnisse einer eventuellen Verteilung/Zulassung auf der Portal²-Seite für die Studierenden freigegeben sind.
- **Aktivierung:**
  - **„Aktiviert“:** Alle zugelassenen Teilnehmenden aus Portal² werden übernommen. Auch später zugelassene Teilnehmer werden automatisch hinzugefügt.
  - **„Deaktiviert“:** Alle zu diesem Zeitpunkt aufgenommenen Teilnehmer bleiben erhalten, es werden jedoch keine nachträglich zugelassenen Teilnehmer mehr hinzugefügt.
- **Kein Zulassungsverfahren:** Bei Veranstaltungen ohne Zulassungsverfahren oder wenn Sie den Beitritt zusätzlich einschränken möchten, nutzen Sie bitte das Beitrittsverfahren direkt in ILIAS.

**Sammelbearbeitung:**
Wenn mehrere Parallelgruppen existieren und Sie Admin-Rechte in allen Gruppen haben, bearbeiten Sie die Freischaltung über den übergeordneten Kurs unter „Portal²-Mitglieder“, um alle Gruppen gleichzeitig zu verwalten.

## 👤 Zusätzliche Lehrpersonen und Admins hinzufügen

**Standardzuordnung:**
Sowohl die durchführende als auch die verantwortliche Lehrperson werden automatisch als Administrator des Kurses und der zugehörigen ILIAS-Gruppe eingetragen (basierend auf der Portal²-Zuordnung).

**Hinzufügen zusätzlicher Admins:**
Sie können zusätzliche Personen (z.B. Department-Admins) hinzufügen, die neben den Dozent\*innen auch Admin für den ILIAS-Kurs und die zugehörige ILIAS-Gruppe sein sollen.

1. Klicken Sie auf das **Person-mit-Stern-Symbol** rechts neben der ILIAS-Gruppe (bei der Veranstaltung als übergeordneter Kurs und der PG als untergeordneter Gruppe).
1. Suchen Sie die gewünschten Mitarbeiter*innen (Tutor*innen, Sekretär\*innen etc.).
1. Wählen Sie die Personen aus und bestätigen Sie.

> **Hinweis zum Zugriff:** Personen, die Admin des ILIAS-Kurses sind, können nicht automatisch auf alle untergeordneten Gruppen zugreifen. Der Zugriff ist nur auf die ILIAS-Gruppe möglich, zu der die Person in Portal² zugeordnet wurde.

## 📚 Weitere Informationen

Für allgemeine Informationen zu ILIAS-Grundlagen und zur Definition eines Beitrittsverfahrens empfiehlt sich der Besuch unserer allgemeinen ILIAS-Grundlagen-Seite.

Tiefergehende Informationen zu ILIAS und E-Learning finden Sie direkt in ILIAS selbst unter dem Kurs: [„Digitalisierung in der Lehre“](http://ilias.uni-mannheim.de/goto.php?target=crs_980882&client_id=ILIAS).
