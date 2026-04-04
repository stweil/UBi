---
title: "Anleitung: Exchange Postfach mit Desktop-Clients (Outlook, Thunderbird) verbinden"
source_url_de: https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/einbinden-windows/
source_url_en: https://www.uni-mannheim.de/en/it/instructions/microsoft-exchange/adding-an-exchange-account-to-windows/
category: Services
tags: ['Exchange', 'Outlook', 'Thunderbird', 'Einrichtung', 'E-Mail', 'Windows', 'Anleitung', 'Postfach']
language: de
---

# Verbindung Ihres Exchange Postfachs mit Desktop-Clients

Diese Anleitungen zeigen Ihnen, wie Sie Ihr Exchange Postfach mit einem E-Mail-Programm auf Ihrem Windows-Gerät verbinden. **Bitte beachten Sie:** Diese Anleitungen können erst angewendet werden, nachdem Ihr Exchange Postfach erstellt wurde.

**Empfehlung der Universitäts-IT:**
Wir empfehlen dringend die Verwendung von **Outlook** als E-Mail-Client, da dieser alle Funktionen Ihres Exchange Postfachs (wie Kalender oder Adressbücher) optimal nutzen kann. Alternative Clients (wie Thunderbird) können sich nur mit eingeschränktem Funktionsumfang verbinden und benötigen Add-ons, deren Aktualität nicht garantiert werden kann. Die Universitäts-IT bietet daher den vollständigen Support nur für Outlook.

Alternativ können Sie Ihr Postfach jederzeit über einen Webbrowser unter [https://exchange.uni-mannheim.de](https://exchange.uni-mannheim.de) aufrufen. Die Anmeldung erfolgt mit Ihrer Uni-ID und dem dazugehörigen Passwort.

**Verfügbare Anleitungen:**

- [Anleitung Outlook](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/einbinden-windows/)
- [Anleitung Outlook für Verwaltung](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/einbinden-windows/)
- [Anleitung Thunderbird](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/einbinden-windows/)
- [Anleitung Windows Mail App](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/einbinden-windows/)

______________________________________________________________________

## ⚙️ Initialer Einrichtungsschritt (Für alle Outlook-Versionen)

**Wichtig:** Beim allerersten Verbinden von Outlook auf Ihrem PC/Laptop mit dem Exchange müssen Sie **einmalig** folgende Schritte durchführen, um die Verbindung zu initialisieren:

1. **RegKey-Datei herunterladen:** Laden Sie die Datei „Outlook Autodiscovery RegKey setzen.bat“ herunter: [Download Outlook Autodiscovery RegKey.bat](https://www.uni-mannheim.de/media/Einrichtungen/it/Anleitungen/Exchange/Outlook_Autodiscovery_RegKey/Outlook_Autodiscovery_RegKey_setzen.bat)
   - *Voraussetzung:* Die Datei setzt ein bereits installiertes Outlook voraus (365, 2019 oder 2016).
1. **Datei ausführen:** Führen Sie die heruntergeladene Datei „Outlook Autodiscovery RegKey setzen.bat“ mit einem Doppelklick aus.
   - *Hinweis:* Sollte die Datei von Windows Defender oder einer anderen Antiviren-Software blockiert werden, lassen Sie diese bitte zu.
   - *Hinweis:* Falls sich ein schwarzes Konsolenfenster öffnet, tippen Sie „j“ ein und bestätigen Sie die Eingabe mit der Enter-Taste.
1. **Web-Login und Adresse notieren:**
   - Öffnen Sie Ihren Internetbrowser (z. B. FireFox oder Chrome) und rufen Sie [https://exchange.uni-mannheim.de](https://exchange.uni-mannheim.de) auf.
   - Geben Sie dort Ihre Uni-ID und das dazugehörige Passwort ein und klicken Sie auf „Anmelden“.
   - Klicken Sie nach dem Anmelden auf das Profilbild rechts oben. Ihre **Exchange-Absender\*innen-Adresse** wird im Pop-Up angezeigt. **Bitte notieren Sie sich diese Adresse**, da sie für die Einrichtung in Outlook benötigt wird.

______________________________________________________________________

## 📧 Verbindung mit Microsoft Outlook

### Anleitung für Microsoft Outlook 365

[Die Anleitung als Video](https://www.uni-mannheim.de/media/Einrichtungen/it/Anleitungen/Exchange/Einbinden_Windows/Exchange_Outlook365_GER.mp4)

**Nach der initialen Einrichtung:**

1. Starten Sie Outlook 365. Falls dies der erste Start ist, werden Sie automatisch zum Verbinden aufgefordert. Andernfalls klicken Sie auf den Reiter „Datei“.
1. Klicken Sie auf den „+ Konto hinzufügen“-Button.
1. Geben Sie Ihre Exchange-E-Mail-Adresse ein. Klicken Sie auf „Erweiterte Optionen“, setzen Sie den Haken bei „Ich möchte mein Konto manuell einrichten“ und klicken Sie auf „Verbinden“.
1. Wählen Sie im folgenden Fenster „Exchange“ aus.
1. Im Login-Fenster:
   - Öffnen Sie „Weitere Optionen“ $\\rightarrow$ „Anderes Konto verwenden“.
   - Geben Sie Ihre Uni-ID (=ehem. „Kennung“) mit einem vorangestellten „ad\\“ und Ihr Passwort ein. (*Achtung: Verwenden Sie „\\“, nicht „/“*).
   - Setzen Sie den Haken bei „Anmeldedaten speichern“ und klicken Sie auf „OK“.
1. Bestätigen Sie eventuelle weitere Pop-ups mit „OK“.
1. Belassen Sie „Verwenden Sie den Exchange-Cache-Modus“ angewählt, wählen Sie „1 Jahr“ für das Herunterladen und klicken Sie auf „Weiter“.
1. Bestätigen Sie das Fenster mit „Vorgang abgeschlossen“.
1. Stimmen Sie der Aufforderung zu, die Seite `exchange.uni-mannheim.de/Einstellungen` an Ihrem Konto vornehmen zu lassen.
1. Beenden Sie Outlook und starten Sie es neu. Ihr Postfach wird synchronisiert.

### Anleitung für Microsoft Outlook 2019

**Nach der initialen Einrichtung:**

1. Starten Sie Outlook 2019. Falls dies der erste Start ist, werden Sie automatisch zum Verbinden aufgefordert. Andernfalls klicken Sie auf den Reiter „Datei“.
1. Klicken Sie auf den „+ Konto hinzufügen“-Button.
1. Geben Sie Ihre Exchange-E-Mail-Adresse ein.
1. *Optional:* Stimmen Sie der Aufforderung zu, die Seite `exchange.uni-mannheim.de/Einstellungen` an Ihrem Konto vornehmen zu lassen.
1. Im Login-Fenster:
   - Öffnen Sie „Weitere Optionen“ $\\rightarrow$ „Anderes Konto verwenden“.
   - Geben Sie Ihre Uni-ID (=ehem. „Kennung“) mit einem vorangestellten „ad\\“ und Ihr Passwort ein. (*Achtung: Verwenden Sie „\\“, nicht „/“*).
   - Setzen Sie den Haken bei „Anmeldedaten speichern“ und klicken Sie auf „OK“.
1. Outlook verbindet sich mit Ihrem Postfach. Entfernen Sie den Haken bei „Outlook Mobile auch auf meinem Telefon einrichten“ und klicken Sie auf „OK“.
1. Beenden Sie Outlook und starten Sie es neu, um die Synchronisierung abzuschließen.

### Anleitung für Microsoft Outlook 2016

**Nach der initialen Einrichtung:**

1. Starten Sie Outlook 2016. Falls dies der erste Start ist, werden Sie automatisch zum Verbinden aufgefordert. Andernfalls klicken Sie auf den Reiter „Datei“.
1. Klicken Sie auf den „+ Konto hinzufügen“-Button.
1. Geben Sie Ihren Vor- und Nachnamen, Ihre Exchange-Absender\*innen-Adresse und das Kennwort Ihrer Uni-ID (=ehem. „Kennung“) ein und klicken Sie auf Weiter.
1. *Optional:* Stimmen Sie der Aufforderung zu, die Seite `exchange.uni-mannheim.de/owa/Einstellungen` an Ihrem Konto vornehmen zu lassen.
1. Im Login-Fenster:
   - Öffnen Sie „Weitere Optionen“ $\\rightarrow$ „Anderes Konto verwenden“.
   - Geben Sie Ihre Uni-ID (=ehem. „Kennung“) mit einem vorangestellten „ad\\“ und Ihr Passwort ein. (*Achtung: Verwenden Sie „\\“, nicht „/“*).
   - Setzen Sie den Haken bei „Anmeldedaten speichern“ und klicken Sie auf „OK“.
1. Klicken Sie auf „Fertig stellen“, um Outlook zu öffnen.

______________________________________________________________________

## 🐦 Verbindung mit Thunderbird

**Wichtiger Hinweis:** Die Universitäts-IT bietet für Thunderbird keinen Support für die Synchronisierung von Kalender und Kontakten an. Eine dauerhafte Funktionalität dieser Add-ons kann nicht garantiert werden. Wir empfehlen daher dringend die Nutzung von Outlook oder dem [Outlook Web-Client](https://exchange.uni-mannheim.de/owa).

### 1. E-Mail-Postfach einrichten

[Die Anleitung als Video](https://www.uni-mannheim.de/media/Einrichtungen/it/Anleitungen/Exchange/Einbinden_Windows/Thunderbird/Exchange_Thunderbird_GER.mp4)

1. **Web-Login:** Rufen Sie [https://exchange.uni-mannheim.de](https://exchange.uni-mannheim.de) auf, melden Sie sich mit Uni-ID und Passwort an und notieren Sie sich die **Exchange-Absender\*innen-Adresse**.
1. **Thunderbird starten:** Starten Sie Thunderbird und wählen Sie unter dem Anwendungsmenü die Option „Neu“ $\\rightarrow$ „Bestehendes E-Mail-Konto…“.
1. **Daten eingeben:** Geben Sie Ihren Namen, Ihre **Exchange-Absender\*innen-Adresse** und das Passwort ein. Klicken Sie auf „Manuell einrichten…“.
1. **Serverdaten eintragen:** Tragen Sie die folgenden Werte ein:

| Server | Protokoll | Port | SSL | Authentifizierung | Benutzername |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Posteingang** | IMAP | 993 | SSL/TLS | Passwort, normal | Uni-ID |
| **Postausgang** | - | 587 | STARTTLS | Passwort, normal | Uni-ID |

5. Thunderbird synchronisiert die E-Mails.

#### 📂 Umstellung der Systemordner in Thunderbird

Um sicherzustellen, dass die Ordnerstruktur mit dem Web-Client übereinstimmt, führen Sie folgende Schritte durch:

1. Rechtsklick auf das E@Konto $\\rightarrow$ „Abonnieren…“.
1. Klicken Sie auf „Aktualisieren“ (1), setzen Sie die gewünschten Ordner (2) und klicken Sie auf „Abonnieren“ (3) $\\rightarrow$ „OK“ (4).
1. Rechtsklick auf das E@Konto $\\rightarrow$ „Einstellungen“.
1. Gehen Sie zu „Kopien & Ordner“ (1). Aktivieren Sie unter „Beim Senden von Nachrichten automatisch“ die Option „Anderer Ordner“ (2). Wählen Sie dort den Ordner „Gesendete Elemente“ (4) aus Ihrem E@Account (NICHT „Lokaler Ordner“).

### 2. Kalender und Kontakte synchronisieren (Add-ons)

Um Kalender und Kontakte zu synchronisieren, müssen zwei Add-ons installiert und eingerichtet werden:

1. **Add-ons installieren:**
   - Klicken Sie im Anwendungsmenü auf „Add-ons“.
   - Suchen Sie nach **„tbsync“** und fügen Sie das Add-on „TbSync“ hinzu.
   - Wiederholen Sie dies für das Add-on **„Provider für Exchange ActiveSync“**.
1. **Konto einrichten:**
   - Klicken Sie unten rechts auf „TbSync: Leerlauf“.
   - Wählen Sie unter „Konto Aktionen“ $\\rightarrow$ „Neues Konto hinzufügen“ $\\rightarrow$ „Exchange-ActiveSync“.
   - Wählen Sie „Benutzerspezifische Konfiguration“ und tragen Sie Ihre Daten ein. Im Feld „Benutzername (E-Mail Adresse)“ geben Sie **`ad\Uni-ID`** ein (z.B. `ad\mamuster`). Klicken Sie auf „Konto hinzufügen“.
1. **Synchronisieren:**
   - Setzen Sie den Haken bei „Konto aktivieren und synchronisieren“.
   - Wählen Sie im Auswahlmenü die Häkchen bei **„Kontakte“** und **„Kalender“**.
   - Setzen Sie eine periodische Synchronisation (mindestens $\\ge 5$ Minuten) und klicken Sie auf „Jetzt synchronisieren“.

______________________________________________________________________

## ⚠️ Hinweise und Fehlerbehebung

**Funktionale Einschränkungen:**

- **Thunderbird:** Verbindet sich nur über das IMAP-Protokoll und kann daher nicht alle Ordnerstrukturen automatisch abbilden. Das Ordner-Mapping muss manuell in den Einstellungen vorgenommen werden.
- **Outlook/Web-Client:** Diese Clients übernehmen die Ordnerstruktur automatisch.

**Fehlermeldungen beim Synchronisieren:**

1. Stellen Sie sicher, dass Thunderbird im **Onlinemodus** ist (Button unten links).
1. Wenn das Problem weiterhin besteht, entfernen Sie den Haken bei „Konto aktivieren und synchronisieren“ und wechseln Sie anschließend zum Reiter „Kontoeinstellungen“, um die Eingaben zu überprüfen.
