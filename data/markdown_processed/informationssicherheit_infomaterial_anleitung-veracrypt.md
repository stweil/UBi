---
title: Anleitung zur Verschlüsselung externer Speichermedien mit VeraCrypt
source_url_de: None
source_url_en: https://www.uni-mannheim.de/en/
category: Benutzung
tags: ['VeraCrypt', 'Verschlüsselung', 'Speichermedium', 'USB-Stick', 'Datenverschlüsselung', 'Passwortsicherheit', 'Informationssicherheit']
language: de
---

# VeraCrypt: Verschlüsselung externer Speichermedien

Mit VeraCrypt ist es möglich, gesamte Speichermedien wie externe Festplatten und USB-Sticks zu verschlüsseln. Das System erlaubt es, jederzeit Dateien auf dem verschlüsselten Speichermedium hinzuzufügen, zu ändern oder zu löschen.

## ⚠️ Wichtige Hinweise und Voraussetzungen

Bevor Sie mit der Verschlüsselung beginnen, beachten Sie bitte folgende Punkte:

- **Administratorrechte:** Sowohl für die Installation als auch für die Verschlüsselung externer Speichermedien sind Administrator-Rechte auf dem Computer erforderlich. Falls diese Rechte fehlen, wird der Einsatz von [Cryptomator](https://www.uni-mannheim.de/informationssicherheit/infomaterial/anleitung-cryptomator/) empfohlen.
- **Passwortsicherheit:** Die Sicherheit der Datei hängt maßgeblich von der Stärke Ihres Passworts ab. Auch bei der Auswahl des sicheren Verfahrens AES-256 ist ein starkes Passwort entscheidend. Tipps zur Erstellung sicherer Passwörter finden Sie auf unserer Seite zur [Passwortsicherheit](https://www.uni-mannheim.de/informationssicherheit/sicherheitstipps/passwortsicherheit/).
- **Einsatzbereich:** VeraCrypt sollte **nicht** für die Systemfestplatte oder für Ablagen auf einem NAS oder in der Cloud verwendet werden.
- **Austausch:** Wenn Sie ein verschlüsseltes Speichermedium mit jemandem austauschen möchten, muss diese Person ebenfalls VeraCrypt installiert haben, um das Medium öffnen zu können.

### Vor- und Nachteile im Überblick

**Vorteile:**

- VeraCrypt ist eine kostenlose Anwendung mit umfangreichen Funktionen.
- Es ermöglicht die vollständige Verschlüsselung externer Speichermedien.
- Dateien können jederzeit auf dem verschlüsselten Speichermedium ergänzt, geändert und gelöscht werden.

**Nachteile:**

- Die Vielzahl an Einstellungsmöglichkeiten kann zu Fehlern führen, die die Sicherheit verringern.
- Die Installation und Verschlüsselung erfordern Administrator-Rechte.

## 🛠️ Anleitung: VeraCrypt nutzen

### 1. VeraCrypt herunterladen und installieren

1. **Download:** Laden Sie VeraCrypt unter folgendem Link herunter und installieren Sie es: [https://www.veracrypt.fr/en/Downloads.html](https://www.veracrypt.fr/en/Downloads.html)
   - *Erinnerung:* Administrator-Rechte sind für diesen Schritt zwingend erforderlich.
1. **Installation:** Öffnen Sie die heruntergeladene EXE-Datei, um die Installation durchzuführen. Nach erfolgreicher Installation können Sie VeraCrypt starten.

### 2. Externes Speichermedium verschlüsseln (Volume erstellen)

**Vorbereitung:** Wir empfehlen die Verwendung eines **leeren** Speichermediums.

1. **Speichermedium anschließen:** Starten Sie VeraCrypt und schließen Sie das zu verschlüsselnde Speichermedium an.
1. **Volume erstellen:** Klicken Sie auf den Button „Volume erstellen“.
1. **Auswahl:** Wählen Sie den Punkt „Eine Partition/ein Laufwerk verschlüsseln“ und bestätigen Sie mit „Weiter >“.
1. **Standard-Volume:** Wählen Sie „Standard VeraCrypt-Volumen“ und bestätigen Sie mit „Weiter“.
1. **Datenträger auswählen:** Wählen Sie über den Button „Datenträger ...“ Ihr eingestecktes Speichermedium aus und bestätigen Sie mit „OK“. Bestätigen Sie die Auswahl anschließend mit „Weiter >“.
1. **Formatierung:** Wählen Sie „Verschlüsseltes Volume erstellen und formatieren“ und bestätigen Sie mit „Weiter >“.
   - **Achtung:** Bei dieser Auswahl werden **alle** Daten auf dem Speichermedium gelöscht.
1. **Einstellungen:** Behalten Sie die Standardeinstellungen bei und bestätigen Sie diese mit „Weiter >“.
1. **Größe:** Da das gesamte Medium verschlüsselt wird, können hier keine Änderungen vorgenommen werden. Springen Sie mit „Weiter >“ zum nächsten Schritt.
1. **Passwort festlegen:** Legen Sie ein sicheres Passwort fest (mindestens 12 Zeichen).
1. **Datenmenge:** Lassen Sie die Standardeinstellung bei „Nein“, falls Sie keine großen Datenmengen (über 4 GB) ablegen möchten.
1. **Formatieren:** Bewegen Sie den Mauszeiger zufällig im Fenster, bis die Anzeige unten grün wird. Klicken Sie anschließend auf „Formatieren“ und bestätigen Sie die Sicherheitsabfrage mit „Ja“.
   - *Wichtig:* Die Formatierung kann je nach Größe des Speichermediums einige Zeit in Anspruch nehmen.
1. **Abschluss:** Nach Abschluss der Formatierung öffnet sich ein Fenster, das Sie über die korrekte Einbindung informiert. Bestätigen Sie diese Meldung mit „OK“ und beenden Sie VeraCrypt.

### 3. Verschlüsseltes Speichermedium öffnen und bearbeiten

Wenn Sie ein bereits verschlüsseltes Speichermedium anschließen, gehen Sie wie folgt vor:

1. **NICHT formatieren:** Wenn eine Meldung zur Formatierung erscheint, bestätigen Sie diese **NICHT** mit „Datenträger formatieren“, sondern klicken Sie auf „Abbrechen“.
1. **Auswählen:** Öffnen Sie VeraCrypt. Wählen Sie Ihr verschlüsseltes Speichermedium über „Datenträger ...“ aus und bestätigen Sie mit „OK“.
1. **Einbinden:** Klicken Sie auf „Einbinden“, um das ausgewählte Speichermedium virtuell einzubinden.
1. **Passwort eingeben:** Geben Sie das zuvor festgelegte Passwort ein und bestätigen Sie mit „OK“.
1. **Zugriff:** Das Speichermedium wird nun unter „Dieser PC“ als lokaler Datenträger angezeigt. Sie können Dateien abspeichern, ändern oder löschen.
1. **Trennen:** Nachdem Sie Ihre Arbeiten abgeschlossen haben, klicken Sie auf „Trennen“ und beenden Sie VeraCrypt. Das Speichermedium kann danach wie gewohnt entfernt werden.
