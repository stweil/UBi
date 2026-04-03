---
title: "Anleitung: Ricoh Kopierer als Drucker unter Windows einrichten"
source_url_de: N/A (Content derived from IT Guide)
source_url_en: https://www.uni-mannheim.de/en/
category: Benutzung
tags: ['Ricoh', 'Drucker', 'Windows', 'Installation', 'Treiber', 'Kopierer', 'IT-Support']
language: de
---

# Wie nutze ich den Ricoh-Kopierer als Drucker unter Windows?

**Wichtiger Hinweis vorab:**
Diese Anleitung gilt **nicht** für die Verwaltung! Bitte wenden Sie sich direkt an den IT-Support:

- **Hotline:** -2000
- **E-Mail:** itsupport@uni-mannheim.de
- **MS Teams:** „UNIT Support“

______________________________________________________________________

## ⚙️ Vorbereitung und Voraussetzungen

Bevor Sie beginnen, benötigen Sie folgende Informationen:

1. **IP-Adresse und Modellbezeichnung** Ihres Ricoh-Kopierers.
   - *Tipp:* Falls Sie die IP-Adresse nicht griffbereit haben, kontaktieren Sie bitte den IT-Support (Hotline -2000, E-Mail itsupport@uni-mannheim.de, MS Teams „UNIT Support“) und halten Sie hierzu die Seriennummer des Kopiergeräts bereit.

## 📥 Schritt 1: Treiber herunterladen

1. Rufen Sie die Ricoh Support Website auf: [https://www.ricoh.de/support/](https://www.ricoh.de/support/) und geben Sie Ihr Kopierermodell ein (z. B. „IM C3010“).
1. Wählen Sie das passende Modell aus der Ergebnisliste und klappen Sie den Punkt „Treiber und Software“ auf.
1. Klicken Sie auf den angezeigten Link, um zur Downloadseite zu gelangen.
1. Wählen Sie Ihr Betriebssystem und anschließend den gewünschten Treiber. Wir empfehlen wahlweise den **„PCL6 Driver for Universal Print“** oder den **„PS Driver for Universal Print“**.
1. Klicken Sie auf „Herunterladen“ und speichern Sie die Datei auf Ihrem Computer.
1. Führen Sie die heruntergeladene Datei aus. Das Entpackungsprogramm für den Druckertreiber wird aufgerufen.
1. **Merken Sie sich den Pfad**, in den der Treiber entpackt wird (standardmäßig wird ein Ordner unter `C:\Temp` vorgeschlagen). Klicken Sie auf „Unzip“, warten Sie, bis der Vorgang abgeschlossen ist, und beenden Sie das Programm.

## 🖨️ Schritt 2: Kopierer als Drucker hinzufügen (Windows 10)

1. Klicken Sie auf **Start** → **Einstellungen** (Zahnradsymbol) → **Bluetooth und Geräte** → **„Drucker und Scanner“**.
1. Klicken Sie oben auf **„Gerät hinzufügen“**.
1. Warten Sie, bis der Text „Der gewünschte Drucker ist nicht aufgelistet“ erscheint, und klicken Sie anschließend auf **„Fügen Sie ein neues Gerät manuell hinzu“**.
1. Wählen Sie im folgenden Dialog die unterste Option: **„Lokalen Drucker oder Netzwerkdrucker mit manuellen Einstellungen hinzufügen“** und klicken Sie auf „Weiter“.
1. Wählen Sie die Option **„Neuen Anschluss erstellen“** und wählen Sie als „Anschlusstyp: **Standard TCP/IP Port**“ aus.
1. Tragen Sie im Feld „Hostname oder IP-Adresse“ die IP-Adresse Ihres Ricoh-Kopierers ein. Behalten Sie die automatisch ausgefüllten Einstellungen bei und klicken Sie auf „Weiter“.
1. Klicken Sie im folgenden Dialog zunächst auf **„Datenträger“**.
1. Klicken Sie auf **„Durchsuchen“** und wählen Sie den Speicherort, an dem Sie den Treiber entpackt haben. Navigieren Sie zu `C:\Temp\disk1` und wählen Sie die Datei **`oemsetup.inf`** aus.
1. Klicken Sie im ursprünglichen Dialogfeld auf **„OK“**.
1. Wählen Sie den Treiber **„PCL6 Driver for Universal Print“** aus und klicken Sie auf „Weiter“.
1. Vergeben Sie einen Namen für den Drucker und klicken Sie auf „Weiter“.
1. Wählen Sie auf der Folgeseite die Option **„Drucker nicht freigeben“** und klicken Sie auf „Weiter“.
1. Beenden Sie den Druckerinstallationsassistenten mit **„Fertig stellen“**.

## ✅ Abschluss und Überprüfung

1. Rufen Sie den neu installierten Drucker aus der Übersichtsliste auf und wählen Sie **„Druckereigenschaften“**.
1. Klicken Sie auf der Registerkarte **„Zubehör“** auf den Button **„Jetzt aktualisieren“**. Der Kopierer wird abgefragt, und das Modell sowie installierte Optionen (z. B. Finisher) werden im Treiber hinterlegt.
1. Schließen Sie alle Einstellungsfenster. Die Druckereinrichtung ist hiermit abgeschlossen.

______________________________________________________________________

### ⚠️ Wichtiger Hinweis zum Netzwerkzugriff (eduroam)

Bitte beachten Sie, dass die Kopierer aus dem Universitäts-WLAN „eduroam“ nur dann angesprochen werden können, wenn das betreffende Endgerät mit einer Uni-ID am WLAN angemeldet ist, welche die Ausprägung **„staff“** hat! Dies ist bei allen Mitarbeitendenkennungen der Fall.

Studentische Kennungen (Ausprägung „student“) können aus Sicherheitsgründen leider nicht direkt auf die Kopierer zugreifen.

[Weitere Anleitungen für Ricoh Kopierer](https://www.uni-mannheim.de/it/anleitungen/kopierer/)
