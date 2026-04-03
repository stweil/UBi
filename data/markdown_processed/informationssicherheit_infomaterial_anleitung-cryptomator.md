---
title: Anleitung zur Nutzung und Einrichtung von Cryptomator
source_url_de: https://www.uni-mannheim.de/informationssicherheit/infomaterial/anleitung-cryptomator/
source_url_en: https://www.uni-mannheim.de/en/information-security/information-material/instructions-for-cryptomator/
category: Benutzung
tags: ['Cryptomator', 'Verschlüsselung', 'Datenmanagement', 'Sicherheit', 'Tresor', 'Passwort', 'Cloud']
language: de
---

# Was ist Cryptomator?

Cryptomator ist eine kostenlose Anwendung, die es Ihnen ermöglicht, Daten einfach und komfortabel in einer Cloud oder einem NAS zu verschlüsseln und abzulegen. Die folgende Anleitung erklärt detailliert, wie Sie Daten mithilfe von Cryptomator verschlüsseln.

## ⚠️ Wichtige Hinweise und Voraussetzungen

Bevor Sie mit der Nutzung beginnen, beachten Sie bitte folgende Punkte:

- **Administrator-Rechte:** Für die Installation von Cryptomator benötigen Sie Administrator-Rechte auf Ihrem Computer. Falls diese fehlen, wenden Sie sich bitte an Ihren Administrator oder den IT-Support unter der -2000.
- **Passwortsicherheit:** Die Sicherheit Ihrer Daten hängt maßgeblich von der Stärke Ihres Passworts ab. Beachten Sie dies bei der Passwortwahl! Tipps zum Erstellen sicherer Passwörter finden Sie auf unserer Seite zur [Passwortsicherheit](https://www.uni-mannheim.de/informationssicherheit/sicherheitstipps/passwortsicherheit/).
- **Wiederherstellungsschlüssel:** Es besteht die Möglichkeit, einen Wiederherstellungsschlüssel zu erstellen. Sollten Sie Ihr Passwort vergessen, ist dieser Schlüssel die *einzige* Möglichkeit, wieder Zugriff auf Ihre verschlüsselten Daten zu erhalten. Bewahren Sie diesen Schlüssel sicher und für Dritte unzugänglich auf.
- **Gemeinsame Ordner:** Bei der Verwendung eines gemeinsamen verschlüsselten Ordners (z. B. in OneDrive) ist es nicht möglich, zeitgleich an den dort abgelegten Dateien zu arbeiten.
- **Austausch:** Wenn Sie einen mit Cryptomator verschlüsselten Ordner mit jemandem austauschen möchten, muss diese Person ebenfalls Cryptomator installiert haben, um den Ordner öffnen zu können.

## Vorteile und Nachteile von Cryptomator

**Vorteile:**

- Verschlüsselte Ordner können einfach und unkompliziert erstellt werden.
- Innerhalb der Tresore können Dateien hinzugefügt, bearbeitet oder gelöscht werden.

**Nachteile:**

- Beim Öffnen eines verschlüsselten Ordners, ohne diesen zuvor zu entsperren, werden die Dateien zwar angezeigt, aber Cryptomator wandelt sie in das C9R-Format um. Dadurch ist kein Rückschluss auf die ursprünglichen Dateiformate, Erstellungsdaten oder Dateinamen möglich; lediglich die Anzahl der Dateien ist ersichtlich.
- Aktuell gibt es noch keine offizielle portable Version dieser Anwendung.

## 🛠️ Wie kann ich Cryptomator nutzen?

### 1. Download & Installation

**Schritt 1: Cryptomator herunterladen**
Laden Sie Cryptomator unter folgendem Link herunter und installieren Sie es: [https://cryptomator.org/de/downloads/](https://cryptomator.org/de/downloads/)
*(Hinweis: Bitte beachten Sie die oben genannten Hinweise zu den Administrator-Rechten.)*
Neben Windows sind unter diesem Link auch Versionen für MacOS oder Linux verfügbar.

**Schritt 2: Installation**
Öffnen Sie die heruntergeladene EXE-Datei, um die Installation zu starten. Nach erfolgreicher Installation können Sie Cryptomator direkt starten.

### 2. Neuen Tresor erstellen

1. **Tresor hinzufügen:** Starten Sie Cryptomator und wählen Sie das „+“-Symbol, gefolgt von „Neuen Tresor erstellen...“.
1. **Tresorname festlegen:** Geben Sie einen Namen für Ihren Tresor ein und bestätigen Sie diesen mit „Weiter“.
1. **Speicherort auswählen:** Wählen Sie über „Durchsuchen...“ den gewünschten Speicherort für Ihren Tresor und bestätigen Sie diesen mit „Weiter“.
1. **Experteneinstellung:** Überspringen Sie das nächste Fenster direkt mit „Weiter“.
1. **Passwort festlegen:** Geben Sie ein sicheres Passwort mit mindestens 12 Zeichen ein.
1. **Wiederherstellungsschlüssel:** Erstellen Sie den Wiederherstellungsschlüssel. Drucken Sie diesen aus oder speichern Sie ihn in einem Passwortmanager/auf einem USB-Stick. **Dieser Schlüssel darf niemals zusammen mit dem verschlüsselten Tresor aufbewahrt werden.**
1. **Tresor entsperren:** Entsperren Sie den neuen Tresor durch Eingabe des Passworts.
1. **Dateien verwalten:** Sie können nun Dateien einfügen, bearbeiten oder löschen. Die Datei „WILLKOMMEN.rtf“ enthält kurze Infos und kann nach dem Lesen gelöscht werden.
1. **Tresor sperren:** Sperren Sie den Tresor, wenn Sie mit der Bearbeitung der Dateien fertig sind.

### 3. Existierenden Tresor öffnen

1. **Tresor öffnen:** Wählen Sie das „+“-Symbol und „Bestehenden Tresor öffnen...“ aus.
1. **Datei auswählen:** Öffnen Sie den gewünschten Tresor und wählen Sie die Datei „vault.cryptomator“ aus.
1. **Tresor entsperren:** Geben Sie das Passwort ein, um den Tresor zu entsperren. Anschließend können Sie die darin abgelegten Dateien öffnen, bearbeiten, löschen oder neue hinzufügen.

### 4. Passwort zurücksetzen

Sollten Sie Ihr Passwort vergessen haben, benötigen Sie zwingend den Wiederherstellungsschlüssel.

1. **Tresoroptionen:** Wählen Sie bei dem entsprechenden Ordner „Tresoroptionen“.
1. **Passwort zurücksetzen:** Unter dem Reiter „Passwort“ haben Sie die Möglichkeit, Ihr Passwort zurückzusetzen.
