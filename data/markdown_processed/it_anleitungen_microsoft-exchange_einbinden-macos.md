---
title: Exchange Postfach mit macOS (Outlook & Apple Mail) verbinden
source_url_de: https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/einbinden-macos/
source_url_en: https://www.uni-mannheim.de/en/it/instructions/microsoft-exchange/adding-an-exchange-account-to-macos/
category: Services
tags: ['Exchange', 'macOS', 'Outlook', 'Apple Mail', 'Einrichtung', 'Uni-ID', 'Postfach']
language: de
---

# Anleitung: Exchange Postfach mit MacBook oder iMac verbinden

Diese Anleitungen zeigen Ihnen, wie Sie Ihr Exchange Postfach mit Ihrem MacBook oder iMac verbinden. **Wichtig:** Diese Anleitungen können erst angewendet werden, nachdem Ihr Exchange Postfach erstellt wurde.

**Alternative zum Client:** Sie sind nicht auf Mail-Clients wie Outlook oder Apple Mail angewiesen. Ihr Exchange Postfach können Sie auch direkt über Ihren Webbrowser unter [https://exchange.uni-mannheim.de/owa](https://exchange.uni-mannheim.de/owa) aufrufen. Dort melden Sie sich mit Ihrer Uni-ID (= ehem. „Kennung“) und dem zugehörigen Passwort an, um auf E-Mails, Kalender und Adressbücher zuzugreifen.

______________________________________________________________________

## 💻 Anleitung für Outlook für Mac

Folgen Sie diesen Schritten, um Ihr Exchange-Konto in Outlook 365 einzurichten:

**Schritt 1:** Starten Sie Outlook 365. Klicken Sie oben links auf „Outlook“ und wählen Sie „Einstellungen“.
**Schritt 2:** Klicken Sie auf „Konten“.
**Schritt 3:** Klicken Sie links unten auf „+ Neues Konto hinzufügen“.
**Schritt 4:** Geben Sie Ihre Exchange-Adresse ein und klicken Sie auf „Weiter“.

- **Falls das IdP-Login-Fenster** der Uni Mannheim erscheint (Schloss im Hintergrundbild und Logo der Uni im Vordergrund): Führen Sie die Schritte 5–7 aus.
- **Falls sofort das Exchange-Anmeldedaten-Fenster** erscheint: Überspringen Sie die Schritte 5–7 und fahren Sie mit Schritt 8 fort.

**Schritte 5–7 (Nur bei IdP-Login):**
5\. Schließen Sie das IdP-Fenster mit einem Klick auf den Schließen-Button links oben.
6\. Klicken Sie im darunterliegenden Fenster auf „Nicht Microsoft 365?“.
7\. Klicken Sie auf den „Exchange“-Button.

**Schritt 8 (Konfiguration):**

1. Tragen Sie im Feld „DOMÄNE\\Benutzername“ ein: **`AD\Uni-ID`** (Beispiel: `AD\memuster`).
   > **Achtung:** Verwenden Sie den Backslash (`\`), nicht den Schrägstrich (`/`). Dies kann mit `ALT + Shift + 7` erzeugt werden.
1. Geben Sie das Passwort Ihrer Uni-ID ein.
1. Tragen Sie im Feld „Server“ folgenden Wert ein: [https://exchange.uni-mannheim.de/EWS/Exchange.asmx](https://exchange.uni-mannheim.de/EWS/Exchange.asmx)
1. Bestätigen Sie mit einem Klick auf „Konto hinzufügen“.

**Schritt 9 (Abschluss):**
Bestätigen Sie danach erneut mit einem Klick auf „Dieses Mal überspringen“. Ihr Postfach wird eingerichtet und synchronisiert. Dies kann je nach Postfachgröße einige Zeit in Anspruch nehmen.

______________________________________________________________________

## 🍎 Anleitung für Apple Mail

### 📧 E-Mail-Konto einrichten

1. **Vorbereitung (Web-Login):** Öffnen Sie Ihren Internetbrowser (z. B. Safari oder Chrome) und rufen Sie [https://exchange.uni-mannheim.de](https://exchange.uni-mannheim.de) auf. Melden Sie sich mit Ihrer Uni-ID und dem Passwort an.
1. **Absenderadresse notieren:** Klicken Sie nach der Anmeldung auf das Profilbild rechts oben. Ihre Exchange-Absenderadresse wird im Pop-Up angezeigt. **Notieren Sie sich diese Adresse**, da sie für die Einrichtung benötigt wird.

**Wenn Sie Apple Mail noch nicht verbunden haben:** Fahren Sie mit Schritt 7 fort.

**Wenn Sie bereits ein Konto verbunden haben:** Fahren Sie mit Schritt 4 fort.

**Schritte 5–6 (Mail-App öffnen):**
5\. Starten Sie die Mail-App auf Ihrem Mac und klicken Sie auf „Mail“ > „Einstellungen“.
6\. Klicken Sie im folgenden Fenster auf den Reiter „Accounts“ und dann auf das „+“-Symbol.

**Schritte 7–9 (Konto hinzufügen):**
7\. Wählen Sie „Anderer Mail-Account …“ und klicken Sie auf „Fortfahren“.
8\. Geben Sie den gewünschten Namen, Ihre **Exchange-Absenderadresse** und das Passwort Ihrer Uni-ID ein. Klicken Sie auf „Anmelden“.
9\. **Fehlerbehebung:** Es erscheint die Meldung, dass Accountname/Passwort nicht überprüft werden konnten. Dies ist normal. Geben Sie Ihren Accountnamen im Format **`AD\Uni-ID`** (z. B. `AD\memuster`) ein und tragen Sie in die Felder Server für eintreffende & ausgehende E-Mails **`exchange.uni-mannheim.de`** ein. Klicken Sie auf „Anmelden“.
\> **Achtung:** Verwenden Sie den Backslash (`\`), nicht den Schrägstrich (`/`).

**Schritt 10 (Abschluss):**
10\. Wählen Sie „Mail“ und ggf. „Notizen“ aus und klicken Sie auf „Fertig“. Ihr E-Mail-Postfach wird nun eingerichtet und synchronisiert.

### 📅 Kalender und Kontakte einbinden

Um Ihren Kalender und Kontakte einzubinden, führen Sie bitte die folgenden Schritte durch:

1. **Kalender-App öffnen:** Öffnen Sie die Kalender-App und klicken Sie links oben auf „Kalender“ > „Account hinzufügen …“.
1. **Konto wählen:** Wählen Sie „Microsoft Exchange“ und klicken Sie auf „Fortfahren“.
1. **Details eingeben:** Tragen Sie Ihren gewünschten Namen und Ihre Exchange-Adresse ein und klicken Sie auf „Anmelden“.
1. **Konfiguration:** Wählen Sie im folgenden Fenster „Manuell konfigurieren“.
1. **Passwort und Benutzername:** Geben Sie das Passwort Ihrer Uni-ID ein und klicken Sie auf „Anmelden“.
1. **Fehlerbehebung:** Es erscheint die Meldung, dass Accountname/Passwort nicht überprüft werden konnten. Dies ist normal. Tragen Sie im Feld „Benutzername“ Ihre Uni-ID im Format **`AD\Uni-ID`** (z. B. `AD\memuster`) ein und klicken Sie auf „Anmelden“.
1. **Server-URLs (falls nötig):** Falls das nachfolgende Fenster erscheint, tragen Sie in den Feldern Interne- und Externe URL bitte **`https://exchange.uni-mannheim.de/EWS/Exchange.asmx`** ein und klicken Sie auf „Anmelden“.
1. **Auswahl:** Wählen Sie im nächsten Fenster **„Kalender“**, **„Erinnerungen“** und **„Kontakte“** aus und klicken Sie auf „Fertig“.
   > **Wichtig:** Wählen Sie **NICHT** „Mail“ aus.

Ihr Kalender und freigegebene Kalender beginnen nun mit der Synchronisation.
