---
title: Exchange Postfach mit iOS Mail-App verbinden
source_url_de: https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/einbinden-ios/
source_url_en: https://www.uni-mannheim.de/en/it/instructions/microsoft-exchange/adding-an-exchange-account-to-ios/
category: Services
tags: ['Exchange', 'iOS', 'iPhone', 'iPad', 'Mail-App', 'Einbindung', 'Postfach', 'Konfiguration']
language: de
---

# Anleitung: Exchange Postfach mit iPhone oder iPad verbinden

Diese Anleitung erklärt, wie Sie Ihr Exchange Postfach mit der nativen **iOS Mail-App** auf Ihrem iPhone oder iPad verbinden.

**Wichtige Hinweise vorab:**

- Diese Anleitung kann erst angewendet werden, nachdem Ihr Exchange Postfach erstellt wurde.
- Die Schritte beziehen sich auf die **iOS Mail-App**. Diese Vorgehensweise kann analog für andere Mail-Apps (außer Outlook) auf iOS-Geräten angewendet werden.
- Die Verknüpfung mit der offiziellen Outlook-App für iOS ist aus datenschutzrechtlichen Gründen nicht möglich.
- **Alternative:** Falls Sie IMAP verwenden möchten, finden Sie die Verbindungsdaten zum Server [hier](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/einbinden-android/#c259568).
- **Webzugriff:** Sie können Ihr Postfach jederzeit auch über Ihren Webbrowser unter [https://exchange.uni-mannheim.de/owa](https://exchange.uni-mannheim.de/owa) aufrufen. Hier melden Sie sich mit Ihrer Uni-ID und dem Passwort an, um auf E-Mails, Kalender und Adressbücher zuzugreifen.

## Schritt-für-Schritt-Anleitung zur Einrichtung in der iOS Mail-App

Folgen Sie diesen Schritten, um Ihr neues E-Mail-Konto einzurichten:

### Teil 1: Erfassung der Exchange-Absenderadresse (Im Browser)

1. Öffnen Sie einen Internetbrowser (z. B. Safari, Chrome oder Firefox) und navigieren Sie zu [https://exchange.uni-mannheim.de](https://exchange.uni-mannheim.de).
1. Melden Sie sich mit Ihrer Uni-ID und dem zugehörigen Passwort an.
1. Klicken Sie im oberen Menü auf das Profilbild.
1. Notieren Sie sich die angezeigte **Exchange-Absenderadresse**.
   - *Tipp:* Sollte die Adresse nicht vollständig sichtbar sein, melden Sie sich auf einem PC/Laptop/Macbook an und klicken Sie dort rechts oben auf das Profilbild, um die vollständige Adresse zu sehen.

### Teil 2: Konfiguration in den iOS Einstellungen

1. Öffnen Sie die App **„Einstellungen“** auf Ihrem Smartphone oder Tablet.
1. Wählen Sie **„Mail“** und anschließend **„Accounts“**.
1. Tippen Sie auf **„Account hinzufügen“**.
1. Wählen Sie **„Microsoft Exchange“**.
1. Geben Sie Ihren Namen und die zuvor notierte **Exchange-Absenderadresse** ein. Wählen Sie eine gewünschte Beschreibung und tippen Sie auf „Weiter“.
1. **Konfigurationsdetails:**
   - Wählen Sie im nächsten Fenster **„Manuell konfigurieren“**.
   - Geben Sie unter **„Benutzername“** Ihre Uni-ID (= ehem. „Kennung“) ein, ergänzt durch **`AD\`** (Achtung: Verwenden Sie den Backwards-Slash `\`, nicht den Forwards-Slash `/`).
   - Geben Sie Ihr Passwort ein.
   - *Hinweis:* Bei manchen iOS-Versionen ist es notwendig, im Feld „Server“ den Eintrag `exchange.uni-mannheim.de` zu ergänzen.
1. Bestätigen Sie Ihre Eingaben mit „Weiter“.
1. Die Mail-App verbindet sich mit Ihrem Postfach und zeigt eine Auswahl an, welche Apps mit dem neuen Exchange-Account verwendet werden sollen. Setzen Sie alle gewünschten Haken und tippen Sie auf **„Fertig“**.

______________________________________________________________________

**Wichtiger Hinweis zur Sicherheit:**
Der Hinweis in den Einstellungen bezüglich der Verwaltung des Geräts per Fernzugriff bezieht sich auf die Möglichkeit, das Gerät zurückzusetzen, falls die PIN mehrfach falsch eingegeben wurde. Diese Möglichkeit ist auf dem Exchange der Universität Mannheim **DEAKTIVIERT**. Die Universitäts-IT hat keinen Zugriff auf Ihre Smartphone-Daten.
