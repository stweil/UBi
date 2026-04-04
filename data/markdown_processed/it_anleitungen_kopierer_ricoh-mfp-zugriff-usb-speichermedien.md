---
title: USB-Speichermedien auf Ricoh Kopierern einrichten und formatieren
source_url_de: https://www.uni-mannheim.de/it/anleitungen/kopierer/ricoh-mfp-zugriff-usb-speichermedien/
source_url_en: https://www.uni-mannheim.de/en/
category: Services
tags: ['Ricoh', 'Kopierer', 'USB-Stick', 'FAT32', 'Konfiguration', 'Scan', 'Druck']
language: de
---

# Zugriff auf USB-Speichermedien an Ricoh Kopierern einrichten

Diese Anleitung beschreibt die Schritte zur Aktivierung des Zugriffs auf USB-Speichermedien (Scannen auf USB und Drucken von USB) an einem Ricoh Multifunktionsgerät (MFP).

## ⚠️ Wichtige Voraussetzungen vorab

Bevor Sie mit der Konfiguration beginnen, beachten Sie bitte folgende Punkte:

- **Adblocker deaktivieren:** Falls Sie einen Werbeblocker (Adblocker) in Ihrem Browser aktiv haben, deaktivieren Sie diesen bitte für das Webinterface des Kopierers. Andernfalls kann die Darstellung fehlerhaft sein.
- **IP-Adresse ermitteln:** Rufen Sie das Webinterface über die IP-Adresse des Kopierers auf (z.B. `https://IP-Adresse Ihres Kopierers`). Die IP-Adresse finden Sie auf dem Hauptbildschirm des Kopierers unter „Status prüfen“ $\\rightarrow$ „Gerätestatus“ / „Netzwerk“.
- **Spezialwarnung (Zertifikat):** Bei der ersten Anmeldung müssen Sie möglicherweise eine Warnmeldung bestätigen, da der Kopierer ein selbstsigniertes Zertifikat verwendet. **Bitte wenden Sie dieses Vorgehen nur in diesem Ausnahmefall an!**

## ⚙️ Schritt-für-Schritt-Anleitung zur Konfiguration

1. **Webinterface aufrufen:** Geben Sie die IP-Adresse des Kopierers in die Adresszeile Ihres Browsers ein.
1. **Login:** Klicken Sie oben rechts auf „Login“. Melden Sie sich mit der Kennung **`admin`** und dem bei der Ersteinrichtung erhaltenen Kennwort an.
   - *Kennwort vergessen?* Kontaktieren Sie bitte den IT-Support:
     - Hotline: -2000
     - E-Mail: [itsupport@uni-mannheim.de](mailto:itsupport@uni-mannheim.de)
     - Teams: „UNIT Support“
   - *Hinweis:* Halten Sie hierzu die Seriennummer des Kopierers bereit.
1. **Navigation:** Falls nach der Anmeldung ein bestimmter Bildschirm angezeigt wird, klicken Sie links oben auf „Home“. Andernfalls fahren Sie mit Schritt 4 fort.
1. **Gerätemanagement:** Fahren Sie mit der Maus über den Menüpunkt **„Gerätemanagement“** und klicken Sie auf **„Konfiguration“**.
1. **Systemeinstellungen:** Klicken Sie unter „Geräteeinstellungen“ auf **„System:“**.
1. **Mediensteckplatz aktivieren:** Wählen Sie bei „Allgemeine Einstellungen“ unter **„Verwendung des Mediensteckplatzes“** für folgende Optionen **„Erlauben“** aus:
   - „Im Speichergerät speichern“
   - „Vom Speichergerät drucken“
1. **Speichern und Abmelden:** Klicken Sie oben links auf **„OK“**, gefolgt von **„Abmelden“** rechts oben.

**✅ Fertig:** Die Konfiguration ist abgeschlossen. Sie können nun auf dem Ricoh-Kopierer sowohl auf USB-Sticks scannen als auch Dokumente ausdrucken, die auf dem Stick gespeichert sind.

## 💾 USB-Stick vorbereiten (FAT32 Formatierung)

Der USB-Stick **muss** im **FAT32**-Format vorliegen, andernfalls wird er vom System nicht erkannt.

### 🖥️ Anleitung zur Formatierung unter Windows

1. Schließen Sie den USB-Stick an Ihren Windows-PC an.
1. Öffnen Sie den Windows-Explorer (Windows-Taste + E) und suchen Sie den USB-Stick unter „Dieser PC“.
   - **⚠️ ACHTUNG:** Vergewissern Sie sich, dass Sie das korrekte Laufwerk auswählen, da sonst Datenverlust droht. Der gesamte Inhalt des Sticks wird gelöscht!
1. Klicken Sie mit der rechten Maustaste auf den USB-Stick und wählen Sie **„Formatieren“**.
1. **Einstellungen vornehmen:**
   - Dateisystem: **FAT32**
   - Volumebezeichnung: Einen Namen vergeben (z.B. „MFP-Stick“)
   - Häkchen bei „Schnellformatierung“ lassen.
1. Klicken Sie auf **„Starten“** und bestätigen Sie die Warnmeldung.
1. **Sich entfernen:** Melden Sie den USB-Stick anschließend wie gewohnt vom System ab („sicheres Entfernen“).

### 🔌 Sicheres Entfernen vom Kopierer

Ziehen Sie den Stick niemals einfach ab! Tippen Sie auf dem Hauptbildschirm links unten am Rand auf das **USB-Symbol** und wählen Sie **„Auswerfen“**.

[Weitere Anleitungen für Ricoh Kopierer](https://www.uni-mannheim.de/it/anleitungen/kopierer/)
