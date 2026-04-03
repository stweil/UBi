---
title: Anleitung zur Nutzung und Einrichtung von KeePass als Passwort-Manager
source_url_de: N/A
source_url_en: https://www.uni-mannheim.de/en/information-security/information-material/keepass-instructions/
category: Benutzung
tags: ['Passwort-Manager', 'KeePass', 'Sicherheit', 'Passwortspeicherung', 'Einrichtung', 'Datenbank', 'Uni-Mannheim']
language: de
---

# KeePass: Ihr Passwort-Tresor

Ein Passwort Manager dient als sicherer Tresor, um Passwörter zu speichern und bei Bedarf darauf zugreifen zu können. Die Universität Mannheim stellt keinen zentralen Passwort Manager zur Verfügung, weshalb wir den kostenlosen Passwort Manager **KeePass** empfehlen.

**⚠️ Wichtige Sicherheitshinweise:**

- Laden Sie KeePass **ausschließlich** über die in dieser Anleitung angegebenen Links herunter.
- Seien Sie vorsichtig: Angreifer bauen Webseiten nach, um Sie zum Download von Schadprogrammen zu verleiten.

## 1. Installation und Einrichtung von KeePass

### 1.1 KeePass herunterladen

1. **Download der Portable Edition:** Laden Sie die „**Professional Edition Portable**“ Version von KeePass unter folgendem Link herunter: [https://www.heise.de/download/product/keepass-15712/download](https://www.heise.de/download/product/keepass-15712/download).
   - *Hinweis:* Das deutsche Sprachpaket kann separat von der Herstellerseite heruntergeladen werden.
1. **Betriebssystem-Hinweis:** Die Anleitung gilt für Windows-Systeme. Für andere Betriebssysteme finden Sie die Version unter [https://keepass.info/](https://keepass.info/).
1. **Sprachpaket (Optional):** Das deutsche Sprachpaket wird auf der Herstellerseite unter „Translations“ > „German“ heruntergeladen.
1. **Überprüfung der Integrität (Hash-Wert):**
   - Rechtsklicken Sie auf die heruntergeladene Zip-Datei und zeigen Sie den Hash-Wert unter „CRC-SHA“ -> „SHA-256“ an (erfordert ggf. 7-Zip).
   - Vergleichen Sie diesen Wert mit dem Hash-Wert der Originaldatei, der unter [https://keepass.info/integrity.html](https://keepass.info/integrity.html) zu finden ist. Stimmen die Werte überein, können Sie fortfahren. Stimmen sie nicht überein, wenden Sie sich bitte an den IT-Support (Tel.: +49 621 181–2000 oder E-Mail: [E-Mail-Adresse hier einfügen]).

### 1.2 KeePass starten

1. Entpacken Sie die Zip-Dateien auf Ihrem Desktop und öffnen Sie die Anwendung „KeePass.exe“.
1. Aktivieren Sie die automatische Update-Erinnerung, indem Sie „Enable (recommended)“ wählen.

### 1.3 Sprache ändern

Um die Sprache zu ändern, müssen Sie das deutsche Sprachpaket herunterladen und die Datei entpacken.

1. **Dateikopieren:** Kopieren Sie die Datei „German.lngx“ in den Ordner „KeePass-2.41\\Languages“.
1. **In KeePass auswählen:** Gehen Sie in KeePass zu „View“ -> „Change Language…“ und wählen Sie das deutsche Sprachpaket aus.
1. **Neustart:** Starten Sie KeePass anschließend neu.

## 2. Datenbank erstellen und sichern

Bevor Passwörter gespeichert werden können, muss eine neue Datenbank angelegt werden.

### 2.1 Neue Datenbank anlegen

1. **Datenbank erstellen:** Gehen Sie zu „Datei“ -> „Neu…“ und erstellen Sie die Datenbank.
1. **Speicherort wählen:** Wählen Sie einen Speicherort, bei dem **nur Sie** Zugriff haben. Speichern Sie die Datenbank **nicht** im KeePass-Ordner, um ein versehentliches Löschen zu verhindern.
   - *Für Verwaltungsangestellte:* Nutzen Sie den dafür vorgesehenen Ordner auf dem Netzlaufwerk. Bei Fragen wenden Sie sich an Herrn Martin Stachniss ([martin.stachniss@uni-mannheim.de](mailto:martin.stachniss@uni-mannheim.de) oder -3181).
1. **Hauptschlüssel vergeben:** Legen Sie ein Hauptpasswort fest. Dieses Passwort schützt alle Ihre Passwörter und sollte daher **sehr komplex und lang** sein (mindestens 12 Zeichen, Groß-/Kleinbuchstaben, Sonderzeichen und Zahlen).

### 2.2 Wahl des Schutzmechanismus

Sie entscheiden, ob die Datenbank zusätzlich durch eine Schlüsseldatei geschützt werden soll.

#### Datenbank MIT Schlüsseldatei schützen (Zwei-Faktor-Authentifizierung)

Diese Methode bietet den höchsten Schutz.

1. **Schlüsseldatei erstellen:** Setzen Sie den Haken bei „Expertenoptionen anzeigen:“ und erstellen Sie die Schlüsseldatei.
   - **Wichtig:** Legen Sie die Schlüsseldatei **sicher, getrennt von der Datenbank** und nicht im KeePass-Ordner ab. Sie benötigen eine separate Sicherung (z.B. auf einer verschlüsselten externen Festplatte), da ohne diese Datei die Datenbank nicht mehr zu öffnen ist.
1. **Einstellungen:** Geben Sie unter „Allgemein“ einen Namen und eine Beschreibung ein.
1. **Erweiterte Einstellungen:** Passen Sie unter „Erweitert“ die Einstellungen für den Hauptschlüssel an (z.B. Erinnerung an Passwortwechsel).
1. **Abschluss:** Bestätigen Sie mit „OK“. (Das Notfallblatt kann übersprungen werden.)

#### Datenbank OHNE Schlüsseldatei erstellen

Wählen Sie diesen Weg, wenn ein zusätzlicher Schutz nicht möglich ist.

1. **Einstellungen:** Geben Sie unter „Allgemein“ einen Namen und eine Beschreibung ein.
1. **Erweiterte Einstellungen:** Passen Sie unter „Erweitert“ die Einstellungen für den Hauptschlüssel an.
1. **Abschluss:** Bestätigen Sie mit „OK“. (Das Notfallblatt kann übersprungen werden.)

### 2.3 Weitere Sicherheitseinstellungen

Nach der Erstellung der Datenbank passen Sie die Sicherheitseinstellungen an:

1. **Optionen öffnen:** Gehen Sie zu „Extras“ -> „Optionen“.
1. **Sperren nach Inaktivität:** Unter dem Reiter „Sicherheit“ setzen Sie den Haken bei „Arbeitsfläche nach KeePass-Inaktivität sperren (Sekunden)“ und geben Sie den Wert **120** ein.
1. **Hauptschlüssel-Sicherung:** Setzen Sie den Haken bei „Hauptschlüssel auf sicherem Desktop eingeben“. Dies pausiert Hintergrundprozesse und blockiert potenzielle Keylogger.
   - *Tipp:* KeePass kann auch manuell über das Icon oder die Tastenkombination **Strg + L** gesperrt werden.

## 3. Verwaltung von Einträgen und Gruppen

### 3.1 Neuen Eintrag hinzufügen

1. **Gruppe auswählen:** Wählen Sie die Gruppe, in der der Eintrag gespeichert werden soll.
1. **Eintrag erstellen:** Gehen Sie zu „Bearbeiten“ -> „Eintrag hinzufügen…“.
1. **Details festlegen:** Geben Sie Titel, Benutzername und Passwort ein. Die Sicherheit des Passworts wird visuell angezeigt (grüner Balken).
1. **Passwort generieren:** Nutzen Sie das integrierte Passwort-Generator-Icon (Schlüssel und Stern), um ein Passwort zu generieren.
1. **Speichern:** Speichern Sie den Eintrag.
   - *Tipp:* Bestehende Einträge können per „Drag & Drop“ in eine andere Gruppe verschoben werden.

### 3.2 Gruppen verwalten

- **Gruppe hinzufügen:** Neue Gruppen können über „Bearbeiten“ -> „Gruppe hinzufügen…“ erstellt werden.
- **Gruppe bearbeiten:** Bestehende Gruppen können über „Bearbeiten“ -> „Gruppe bearbeiten…“ oder per Rechtsklick geändert werden.

### 3.3 Passwort-Generator einrichten (Eigenes Profil)

Um ein eigenes Profil für den Passwort-Generator zu erstellen:

1. **Öffnen:** Gehen Sie zu „Extras“ -> „Passwort generieren...“.
1. **Profil wählen:** Wählen Sie oben „(Benutzerdefiniert)“.
1. **Einstellungen:** Setzen Sie die gewünschten Zeichenkategorien (Groß-/Kleinbuchstaben, Ziffern) und fügen Sie zusätzliche Zeichen wie `!@#$%()+=:;",.?/**` hinzu.
1. **Speichern:** Speichern Sie das Profil unter einem Namen (z.B. „Vorgabe Kennung“) und bestätigen Sie mit „OK“.

### 3.4 Anmeldung an Webseiten und Anwendungen

1. Wählen Sie den entsprechenden Eintrag aus.
1. **Benutzername:** Klicken Sie auf das Menschen-Icon oder nutzen Sie „Benutzernamen kopieren“, um den Benutzernamen zu kopieren.
1. **Passwort:** Klicken Sie auf das Schlüssel-Icon oder nutzen Sie „Passwort kopieren“, um das Passwort zu kopieren.
1. **Öffnen:** Bei hinterlegter URL kann diese über „URL(s)“ oder das Weltkugel-Icon geöffnet werden.

## 4. Datenbank aktualisieren

Wenn eine neue portable Version für Windows verfügbar ist:

1. **Herunterladen:** Laden Sie die neue Version über [https://www.heise.de/download/product/keepass-15712/download](https://www.heise.de/download/product/keepass-15712/download) herunter.
1. **Setup:** Führen Sie die Schritte „KeePass starten“ und „Sprache ändern“ durch.
1. **Datenbank importieren:** Gehen Sie zu „Datei“ -> „Öffnen“ -> „Datei öffnen…“ und fügen Sie Ihre alte Datenbank hinzu.
1. **Anmelden:** Geben Sie Ihr Hauptpasswort ein (und wählen Sie ggf. die Schlüsseldatei aus).
1. **Abschluss:** Bestätigen Sie mit „OK“.
1. **Aufräumen:** Löschen Sie anschließend den Ordner mit der veralteten KeePass Version. **Achten Sie darauf, dass die Datenbank und die Schlüsseldatei nicht in diesem Ordner liegen.**
