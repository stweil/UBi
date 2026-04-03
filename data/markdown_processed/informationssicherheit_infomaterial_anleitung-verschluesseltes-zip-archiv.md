---
title: Anleitung zur Erstellung und Entpackung verschlüsselter ZIP-Archive mit 7-Zip
source_url_de: https://www.uni-mannheim.de/informationssicherheit/infomaterial/anleitung-verschluesseltes-zip-archiv/
category: Benutzung
tags: ['7-Zip', 'Verschlüsselung', 'ZIP-Archiv', 'Passwort', 'Sicherheit', 'Datenübertragung', 'AES-256']
language: de
---

# Umgang mit verschlüsselten ZIP-Archiven

Der Einsatz von verschlüsselten ZIP-Archiven ist eine einfache und kostenlose Methode, um Informationen durch Verschlüsselung zu schützen, beispielsweise beim Versenden per E-Mail oder beim Speichern auf einem USB-Stick. Diese Anleitung erklärt die Erstellung und Entpackung solcher Archive mithilfe von 7-Zip.

## ⚠️ Wichtige Sicherheitshinweise vorab

Bevor Sie ein verschlüsseltes Archiv erstellen oder empfangen, beachten Sie bitte folgende Punkte:

1. **Passwortsicherheit:** Auch bei der Verwendung des sicheren Verfahrens AES-256 ist die Sicherheit der Datei ausschließlich von der Stärke Ihres Passworts abhängig. Nutzen Sie die Tipps zur [Passwortsicherheit](https://www.uni-mannheim.de/informationssicherheit/sicherheitstipps/passwortsicherheit/), um sichere Passwörter zu erstellen.
1. **Passwortübermittlung:** Wenn Sie ein verschlüsseltes ZIP-Archiv per E-Mail versenden, übermitteln Sie das Passwort **niemals** über denselben Kanal. Nutzen Sie stattdessen einen anderen Weg, wie z. B. telefonisch, per Brief oder persönlich.

## 🛡️ Technische Voraussetzungen und Updates

- **Software:** Alle Beschäftigten können 7-Zip kostenlos herunterladen.
- **Sicherheitslücken:** Bitte aktualisieren Sie 7-Zip auf die **Version 23.01 oder höher**, da in älteren Versionen Sicherheitslücken entdeckt wurden.
- **Installation:** Für die Installation von 7-Zip benötigen Sie Administrator-Rechte. Falls diese fehlen, wenden Sie sich bitte an Ihren Administrator oder den IT-Support unter der -2000.

## ⚙️ Anleitung: 7-Zip installieren und nutzen

### 📥 Download und Installation

Falls 7-Zip noch nicht auf Ihrem Computer installiert ist, laden Sie die Anwendung unter folgendem Link herunter und installieren Sie sie:
[https://www.heise.de/download/product/7-zip-13139](https://www.heise.de/download/product/7-zip-13139)

### 📂 Verschlüsseltes Archiv erstellen

1. **Dateiauswahl:** Klicken Sie mit der rechten Maustaste auf die Datei oder den Ordner, der verschlüsselt werden soll, und wählen Sie im Kontextmenü den Punkt „7-Zip“ > „Zu einem Archiv hinzufügen...“.
1. **Passwort festlegen:** Legen Sie ein sicheres Passwort fest (mindestens 12 Zeichen). Wählen Sie bei den Verfahren **AES-256**.
1. **Abschluss:** Bestätigen Sie die Eingaben mit „OK“, um das verschlüsselte Archiv zu erstellen.

### 🔓 Verschlüsseltes Archiv entpacken

1. **Öffnen:** Doppelklicken Sie auf das verschlüsselte Archiv, um 7-Zip zu starten.
1. **Speicherort wählen:** Klicken Sie auf „Entpacken“ und wählen Sie den gewünschten Speicherort.
1. **Passwort eingeben:** Geben Sie das korrekte Passwort ein und bestätigen Sie mit „OK“. Das Archiv wird nun entpackt.

## ⚖️ Vor- und Nachteile verschlüsselter ZIP-Archive

**Vorteile:**

- **Einfachheit:** Die Erstellung ist unkompliziert und mit wenigen Klicks möglich.
- **Kompatibilität:** ZIP-Archive können mit den entsprechenden Tools auf allen Betriebssystemen erstellt und entpackt werden.
- **Sicherheit:** Durch die Verwendung von AES-256 ist eine sichere Verschlüsselung gewährleistet.

**Nachteile:**

- **Umfang:** Es können nur einzelne Dateien oder Ordner gepackt werden; die Verschlüsselung eines gesamten USB-Sticks oder einer Festplatte ist nicht möglich.
- **Bearbeitung:** Ein einmal erstelltes Archiv kann nicht erweitert werden. Um Dateien hinzuzufügen, muss ein neues Archiv erstellt oder das bestehende entpackt, die Dateien hinzugefügt und anschließend alles in ein neues Archiv gepackt werden.
