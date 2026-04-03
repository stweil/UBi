---
title: "Kostenstellen-Einrichtung am Ricoh MFP: Anleitung für Webinterface und Druckertreiber"
source_url_de: https://www.uni-mannheim.de/it/anleitungen/kopierer/ricoh-mfp-kostenstellen/
category: Services
tags: ['Ricoh', 'MFP', 'Kostenstelle', 'Einrichtung', 'Webinterface', 'Authentifizierung', 'Druckertreiber']
language: de
---

# Kostenstellen-Einrichtung am Ricoh MFP

Diese Anleitung beschreibt zwei Verfahren zur Einrichtung von Kostenstellen (Anwender-Authentifizierung) am Ricoh Multifunktionsgerät (MFP): über das Webinterface des Kopierers und über den lokalen Druckertreiber.

## 🖥️ Kostenstellen-Einrichtung über das Webinterface

Folgen Sie diesen Schritten, um die Kostenstelle über die Verwaltungsoberfläche des Geräts einzurichten.

### 1. Zugriff auf das Webinterface

1. **IP-Adresse ermitteln:** Rufen Sie über Ihren Browser das Webinterface des Ricoh-Kopierers auf, indem Sie die IP-Adresse in die Adresszeile eingeben (z.B. `https://IP-Adresse Ihres Kopierers`).
   - *Hinweis:* Die IP-Adresse finden Sie auf dem Hauptbildschirm links unten unter „Status prüfen“ $\\rightarrow$ „Gerätestatus“ / „Netzwerk“.
1. **Warnmeldung bestätigen:** Bestätigen Sie **ausnahmsweise** die Warnmeldung, indem Sie auf „Erweitert“ und anschließend auf „Risiko akzeptieren und fortfahren“ klicken.
   - *Wichtig:* Dieses Vorgehen ist nur für diesen Fall notwendig, da das Gerät ein selbstsigniertes Zertifikat verwendet.
1. **Adblocker deaktivieren:** Deaktivieren Sie bitte alle Adblocker (Werbeblocker) für das Webinterface des Kopierers, um eine korrekte Darstellung aller Menüelemente zu gewährleisten.
1. **Login:** Klicken Sie oben rechts auf „Login“ und melden Sie sich mit der Kennung **`admin`** und dem bei der Ersteinrichtung erhaltenen Kennwort an.
   - *Hilfe:* Bei Problemen mit dem Kennwort kontaktieren Sie bitte den IT-Support unter der Hotline -2000, per E-Mail unter [itsupport@uni-mannheim.de](mailto:itsupport@uni-mannheim.de) oder per Teams unter „UNIT Support“. Halten Sie hierzu die Seriennummer des Kopierers bereit.

### 2. Konfiguration der Kostenstelle

1. **Navigation:** Klicken Sie links oben auf „Home“ (falls erforderlich). Fahren Sie mit der Maus über **„Gerätemanagement“** und klicken Sie auf **„Konfiguration“**.
1. **Authentifizierungseinstellungen:** Klicken Sie unter „Geräteeinstellungen“ auf **„Anwender-Authentifizierungsverwaltung“**.
1. **Standardeinstellung ändern:** Ändern Sie die Standardeinstellung von „Aus“ (1) auf **„Anwendercode“** (2).
1. **Druckerjob-Authentifizierung:** Wählen Sie unter „Druckerjob-Authentifizierung“ den Eintrag **„Gesamt“** aus (1).
1. **Funktionen einschränken:** Setzen Sie unter „Anwendercode-Authentifizierungseinstellungen“ bei „Einzuschränkende Funktionen“ die Häkchen bei **allen Optionen außer „PC-Steuerung“, „Document Server“ und „Fax“** (2). Klicken Sie abschließend auf **„OK“** (3).
1. **Zurück zur Konfiguration:** Sie werden automatisch zur Seite „Konfiguration“ zurückgeleitet. Klicken Sie dort links oben auf „Zurück“.
1. **Adressbuch öffnen:** Fahren Sie mit der Maus über **„Gerätemanagement“** und klicken Sie auf **„Adressbuch“**.
1. **Anwender hinzufügen:**
   - Klicken Sie auf den Reiter **„Detaillierte Eingabe“**.
   - Klicken Sie auf **„Anwender hinzufügen“**.
1. **Details eingeben:** Tragen Sie folgende Informationen ein:
   - **Name:** Der gewünschte Name der Kostenstelle (1).
   - **Titel 1 / Titel 2 / Titel 3:** Beachten Sie die Vorgaben: „Kein(e)“ / „1“ / „Kein(e)“.
   - **Oft hinzufügen:** Wählen Sie **„Aus“** (2).
   - **Anwendercode:** Geben Sie den gewünschten Code für die Kostenstelle ein (3).
   - **Verfügbare Funktionen:** Setzen Sie alle Häkchen, **außer** „Document Server“, „Fax“ und „Browser“, und wählen Sie **„Vollfarbe / Automatische Farbauswahl“** aus (4).
   - Schließen Sie die Einstellungen mit **„OK“** ab (5).
1. **Timer einstellen:** Kehren Sie zu „Gerätemanagement“ $\\rightarrow$ „Konfiguration“ zurück und klicken Sie unter „Geräteeinstellungen“ auf **„Timer“**.
   - Schalten Sie den **„Auto-Abmelde-Timer“** auf **„Ein“** und tragen Sie **`60`** bei „Sekunden“ ein. Speichern Sie die Einstellungen mit „OK“.

Die Konfiguration der Kostenstelle ist hiermit abgeschlossen.

______________________________________________________________________

## 🖨️ Kostenstellen-Einrichtung über den Druckertreiber (Windows)

Dieser Weg dient zur Verknüpfung des Codes direkt über die lokalen Druckereinstellungen.

1. **Einstellungen öffnen:** Drücken Sie die **Windows-Taste** und **`i`** gleichzeitig, um die Einstellungen zu öffnen.
1. **Geräteauswahl:** Wählen Sie in der Seitenleiste **Bluetooth und Geräte** (1) aus und klicken Sie danach auf **Drucker und Scanner** (2).
1. **Drucker auswählen:** Wählen Sie den passenden Drucker aus der Liste der verbundenen Geräte.
1. **Eigenschaften öffnen:** Klicken Sie auf **Druckereigenschaften**.
1. **Einstellungen:** Wählen Sie **Einstellungen...** aus.
1. **Code-Eingabe:** Klicken Sie auf **Anwendercode-Einst...** und geben Sie Ihren Kopiercode ein.

[Weitere Anleitungen für Ricoh Kopierer](https://www.uni-mannheim.de/it/anleitungen/kopierer/)
