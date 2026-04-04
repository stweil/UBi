---
title: Anleitung zum sicheren Löschen von Daten von Festplatten (HDD & SSD)
source_url_de: https://www.uni-mannheim.de/it/anleitungen/festplatten-und-ssds/
source_url_en: https://www.uni-mannheim.de/en/it/instructions/hard-drives-and-ssds/
category: Services
tags: ['Festplatten', 'SSDs', 'Datenlöschung', 'Sicherlöschen', 'HDD', 'SSD', 'ShredOS', 'ATA Secure Erase']
language: de
---

# Sicheres Löschen von Daten von Festplatten und SSDs

Um Daten von nicht mehr genutzten Speichermedien sicher zu entfernen, ist ein einfaches Löschen oder klassisches Formatieren nicht ausreichend, da die Daten potenziell wiederherstellbar sind. Die Methode hängt stark vom Medientyp ab:

- **HDDs (klassische Festplatten):** Erfordern ein mehrfaches Überschreiben der gespeicherten Daten mit Zufallsdaten.
- **SSDs:** Benötigen die Verwendung des speziellen Befehls „ATA Secure Erase“.

## 💾 Sicheres Löschen von HDDs („klassischen“ Festplatten)

### Voraussetzungen

Bevor Sie beginnen, stellen Sie sicher, dass folgende Punkte erfüllt sind:

- Die zu löschende Festplatte ist entweder noch im PC verbaut oder kann über einen Adapter angeschlossen werden.
- Ein leerer USB-Stick (Dieser wird für das Betriebssystem des Löschwerkzeugs benötigt).
- Ein PC mit Internetverbindung und Zugriff auf ein Administrator-Konto.

**Hinweis:** Beim Erstellen des Bootsticks werden **alle Daten** auf dem USB-Stick unwiederbringlich gelöscht.

### 1. Erstellung des ShredOS USB-Bootsticks

Wir verwenden die kostenlose Software [ShredOS](https://github.com/PartialVolume/shredos.x86_64) zur sicheren Datenlöschung.

**Schritte:**

1. Verbinden Sie den USB-Stick mit dem PC.
1. Laden Sie die neueste Version von [ShredOS](https://github.com/PartialVolume/shredos.x86_64) herunter.
1. Wählen Sie die Datei „... for USB Vanilla DRM“ (z.B. „ShredOS .img x86_64bit for USB Vanilla DRM“).

**Tools zur Bootstick-Erstellung:**

- **Windows:** Nutzen Sie [Rufus](https://rufus.ie/de/) (Weitere Informationen siehe unten).
  1. Laden Sie Rufus herunter und starten Sie es.
  1. Wählen Sie das Ziel-USB-Laufwerk aus.
  1. Fügen Sie die heruntergeladene ShredOS Image-Datei per Drag-and-Drop hinzu.
  1. Starten Sie den Schreibvorgang. Bestätigen Sie die Warnung, da **alle Daten** auf dem Stick gelöscht werden.
- **macOS und Linux:** Nutzen Sie [Balena Etcher](https://etcher.balena.io/) (Weitere Informationen siehe unten).
  1. Laden Sie Etcher herunter und installieren Sie es.
  1. Wählen Sie „Flash from file“ und öffnen Sie die ShredOS Image-Datei.
  1. Wählen Sie den Ziel-USB-Stick. **Achtung:** Alle Daten auf dem Stick gehen verloren.
  1. Klicken Sie auf „Flash“ und warten Sie, bis der Vorgang abgeschlossen ist.

### 2. Durchführung des Löschvorgangs

1. Entfernen Sie den erstellten USB-Stick sicher vom PC und schließen Sie ihn an den PC an, dessen Festplatte gelöscht werden soll.
1. Starten Sie den PC und wählen Sie im Boot-Menü (oft durch F12 erreichbar) den USB-Stick als Startlaufwerk aus.
1. ShredOS startet vom USB-Stick.
1. Wählen Sie die zu löschenden Festplatten aus (Navigation mit Pfeiltasten, Auswahl mit Leertaste).
1. Starten Sie den Löschvorgang, indem Sie **Shift + S** drücken.
1. Der Prozess wird angezeigt. Sie können den USB-Stick bereits in dieser Phase vom PC trennen.

## 💿 Sicheres Löschen von SSDs

Das Löschen von SSDs ist technisch anders als bei HDDs, da die interne Struktur und Datenspeicherung abweichen. Hier muss zwingend der Befehl **„ATA Secure Erase“** verwendet werden.

**Voraussetzung:** Ein PC, auf dem Windows installiert ist und in den die zu löschende SSD als zusätzliches Laufwerk eingebaut wurde.

**Wichtig:** Der „ATA Secure Erase“-Befehl muss mit der spezifischen Software des jeweiligen Herstellers aktiviert werden.

**Hersteller-spezifische Tools:**

- [Samsung](https://www.samsung.com/de/ssd/magiciansoftware/)
- [Crucial](https://www.crucial.de/support/storage-executive)
- [Kingston](https://www.kingston.com/de/support/technical/ssdmanager)
- [Intel](https://www.intel.de/content/www/de/de/support/articles/000006231/memory-and-storage.html)
- [Kioxia](https://europe.kioxia.com/de-de/personal/software/ssd-utility.html)
- [SanDisk und Western Digital](https://support-de.sandisk.com/app/answers/detailweb/a_id/50714)

**⚠️ Kritische Warnung:**
Die SSD darf beim Ausführen des „ATA Secure Erase“-Befehls **nicht** über einen USB-Adapter an dem ausführenden Rechner angeschlossen sein. Dies kann dazu führen, dass die SSD anschließend nicht mehr funktioniert oder die Daten nicht korrekt gelöscht wurden.
