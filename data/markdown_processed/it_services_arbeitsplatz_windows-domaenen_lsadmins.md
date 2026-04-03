---
title: Leitfaden zur Einrichtung und Verwaltung von Active Directory Strukturen für Lehrstühle
source_url_de: N/A (Inhalt basiert auf IT-Service-Dokumentation)
source_url_en: https://www.uni-mannheim.de/en/
category: Services
tags: ['Active Directory', 'OU', 'Domäne', 'Lehrstuhl', 'Workstation', 'Benutzerprofile', 'IT-Support']
language: de
---

# Leitfaden für Lehrstuhladministrator\*innen: Einrichtung der Domänen-Infrastruktur

Wenn eine größere Anzahl von Arbeitsplätzen einer Lehrstuhladministration in die Domäne integriert werden soll, ist eine umfassende, schrittweise Planung erforderlich. Dieser Leitfaden fasst die notwendigen Schritte zur Organisation der DV-Infrastruktur zusammen.

## 1. Vorbereitung und Organisation der Domänenstruktur

### Beantragung einer Organizational Unit (OU)

OUs dienen der effizienten Organisation der Lehrstuhl- oder zentralen DV-Infrastruktur innerhalb des Domänen-Konzepts von Windows.

- **Wichtig:** OUs sind nicht automatisch vorhanden, nur weil eine Lehrstuhlkennung beantragt wurde.
- **Vorgehen:** OUs müssen von einem Domänen-Admin (Universitäts-IT-Mitarbeiter) angelegt und mit den notwendigen Berechtigungseigenschaften ausgestattet werden.
- **Kontakt:** Bei der Beabsichtigung der Nutzung einer OU wenden Sie sich bitte an den [IT-Support](https://www.uni-mannheim.de/it/support/).

### Einrichtung des Admin-Arbeitsplatzes

Der administrative Arbeitsplatz benötigt spezielle Plugins für den Zugriff auf das Active Directory.

- **Tool:** Die Verwaltung erfolgt über die „Microsoft-Management-Console“ (MMC).
- **Funktionalität:** Für die OU-Administration wird ein spezifisches Snap-In benötigt, um die OU direkt im Active Directory verwalten zu können.

### Definition und Befüllung von Benutzergruppen

Sobald die OU existiert und Sie als OU-Admin eingetragen sind, ist die Definition von Benutzergruppen notwendig, um Nutzungsberechtigungen für Ressourcen festzulegen.

**Namenskonventionen beachten:**

1. **Allgemeine Gruppen:** Beginnen mit dem Namen der **OU** gefolgt von einem Unterstrich (`_`) und dem eigentlichen Gruppennamen.
1. **Gruppen für zentrale Ressourcen:** Folgen dem Muster: `[OU-Name]__` + `[Dienst-Abkürzung]__` + `[Gruppennamen]`.

*Beispiel:* Gruppen mit dem Präfix `lsxyz__FS__` sind für die Regelung der Nutzungsberechtigung des zentralen Fileservice reserviert.

## 2. Integration der Arbeitsplätze in die Domäne

Nachdem die OU eingerichtet und die Gruppen definiert wurden, erfolgt die Aufnahme der physischen Arbeitsplätze. Dieser Prozess besteht aus mehreren Teilaufgaben:

1. **Domänenaufnahme:** Der Rechner muss zunächst mithilfe des Skripts `"join-ad-mit-ou.bat"` in die Domäne aufgenommen werden.
1. **Gruppenmitgliedschaft anpassen:**
   - Das Skript `"group-ad.bat"` muss verwendet werden, um den Domänen-Admin aus der Gruppe „Lokale Administrator\*innen“ zu entfernen.
   - Die OU-Gruppe „Lehrstuhl-Administrator*innen“ muss in die Gruppe „Lokale Administrator*innen“ aufgenommen werden.
   - Schließlich muss sichergestellt werden, dass nur Benutzerkennungen, die Mitglied in der OU-Gruppe „Lehrstuhl_alle“ sind, sich an diesem Rechner anmelden können.
1. **Profile kopieren:** Folgen Sie der Anleitung [Wie kopiere ich Profile?](#wie-kopiere-ich-profile).

## 3. Übertragung lokaler Benutzerprofile auf Domänen-Profile

Dieser letzte Schritt stellt sicher, dass Personen, die bisher mit einer lokalen Benutzerkennung gearbeitet haben, ihre gewohnte Umgebung auch für die Domänen-Kennung nutzen können.

**Grundlagen:**

- Ein lokaler Benutzer und ein Domänenbenutzer sind für Windows unterschiedliche Benutzerkennungen.
- **Voraussetzung:** Der/die Domänen-Benutzer\*in muss sich zunächst an und wieder abmelden, damit ein neues Domänen-Profil erzeugt und gespeichert wird.

**Schritt-für-Schritt-Anleitung:**

1. **Anmeldung:** Melden Sie sich als lokaler Admin an (weder mit der lokalen noch mit der zugehörigen Domänenkennung).
1. **Eigenschaften öffnen:** Rechtsklick auf „Arbeitsplatz“ $\\rightarrow$ „Eigenschaften“.
1. **Profil-Einstellungen:** Wählen Sie die Registerkarte „Erweitert“ und klicken Sie im Abschnitt „Benutzerprofile“ auf „Einstellungen“.
1. **Kopieren starten:** Wählen Sie in der rechten Dialogbox die **lokale Benutzerkennung** aus und klicken Sie auf „Kopieren nach“.
1. **Zielpfad wählen:** Klicken Sie auf „Durchsuchen“ und wählen Sie das Verzeichnis `C:\Dokumente und Einstellungen`.
1. **Zielordner auswählen:** Wählen Sie den Ordner, der das Suffix **`.AD`** trägt (dies ist das Ziel des Kopiervorgangs).
1. **Berechtigung korrigieren (Wichtig!):** Klicken Sie im Abschnitt „Benutzer\*in“ auf „Ändern“. Hier muss die **Domänen-Benutzerkennung** die Zugriffsrechte erhalten, nicht die lokale Kennung.
1. **Bestätigung:** Geben Sie die vollständige Domänen-Benutzerkennung ein und bestätigen Sie die Auswahl.
1. **Kopieren abschließen:** Bestätigen Sie den Vorgang. Bei der Frage, ob das vorhandene Profil überschrieben werden soll, bestätigen Sie mit „Ja“ (da es sich um ein Standard-Profil handelt).

**Hinweis:**

- Die Kopie ist **einmalig**. Änderungen, die Sie im Domänen-Profil vornehmen, werden **nicht** an das lokale Profil zurückgespielt.
- Im Normalfall sollten Sie sich ab sofort nur noch mit der Domänen-Kennung anmelden.
