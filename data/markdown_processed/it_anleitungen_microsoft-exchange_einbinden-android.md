---
title: Exchange Postfach mit Android-Geräten verbinden
source_url_de: https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/einbinden-android/
source_url_en: https://www.uni-mannheim.de/en/it/instructions/microsoft-exchange/adding-an-exchange-account-to-android-devices/
category: Services
tags: ['Exchange', 'Android', 'Einrichtung', 'Postfach', 'Uni-ID', 'Anleitung', 'G@App']
language: de
---

# Anleitung: Exchange Postfach mit Android Smartphone oder Tablet verbinden

Diese Anleitung erklärt, wie Sie Ihr Exchange Postfach auf Ihren Android-Geräten einrichten. **Wichtig:** Diese Schritte können erst durchgeführt werden, nachdem Ihr Exchange Postfach erstellt wurde.

Die folgende Anleitung bezieht sich auf die **G@App**, die auf den meisten Android-Geräten vorinstalliert ist. Die beschriebenen Schritte können analog für andere Mail-Apps (außer Outlook) angewendet werden.

**Hinweis zu Outlook:** Die Verknüpfung mit der offiziellen Outlook-App für Android ist aus datenschutzrechtlichen Gründen nicht möglich.

**Alternative:** Sie können Ihr Exchange Postfach auch direkt über Ihren Webbrowser unter [https://exchange.uni-mannheim.de/owa](https://exchange.uni-mannheim.de/owa) aufrufen. Dort melden Sie sich mit Ihrer Uni-ID und dem zugehörigen Passwort an, um auf E-Mails, Kalender und Adressbücher zuzugreifen.

______________________________________________________________________

## ⚙️ Schritt-für-Schritt-Anleitung (Empfohlen: Exchange/Office 365)

### Teil 1: Erforderliche Informationen sammeln

Bevor Sie die App einrichten, müssen Sie Ihre vollständige Exchange-Absenderadresse ermitteln:

1. Öffnen Sie Ihren Internetbrowser (z. B. Chrome oder FireFox) und rufen Sie [https://exchange.uni-mannheim.de](https://exchange.uni-mannheim.de) auf.
1. Melden Sie sich mit Ihrer Uni-ID und dem Passwort an.
1. Klicken Sie oben links auf das Menüsymbol.
1. Suchen Sie Ihre Exchange-Absenderadresse. *Falls diese nicht vollständig sichtbar ist:* Melden Sie sich auf Ihrem Rechner/Laptop/Macbook an und klicken Sie rechts oben auf Ihr Profilbild, um die vollständige Adresse zu sehen.
1. **Notieren Sie sich diese vollständige Adresse** – dies ist die benötigte Exchange-Absenderadresse.

### Teil 2: Einrichtung in der G@App

1. Öffnen Sie die G@App.
1. Tippen Sie auf das Menüsymbol in der oberen linken Ecke.
1. Gehen Sie zu **Einstellungen**.
1. Tippen Sie auf **„Konto hinzufügen“**.
1. Wählen Sie im Menü **„Exchange und Office 365“**.
1. Geben Sie die in Teil 1 gesammelte Exchange-Absenderadresse ein und tippen Sie auf **„Manuell einrichten“**.
1. Tragen Sie die folgenden Werte in das Fenster ein und tippen Sie auf „Weiter“:
   - **Passwort:** Das Passwort Ihrer Uni-ID
   - **Domain\\Nutzer\*innenname:** `ad\Uni-ID`
   - **Server:** `exchange.uni-mannheim.de`
   - **Port:** `443`
   - **Sicherheitstyp:** `SSL/TLS`
1. Ihr Postfach ist nun eingerichtet.

**Optional:** Wenn Sie den Synchronisierungszeitraum anpassen möchten, gehen Sie in die Einstellungen, wählen Sie Ihr neues Postfach aus und passen Sie unter „E-Mails synchronisieren ab“ den gewünschten Zeitraum an.

______________________________________________________________________

## 📧 IMAP Kontoeinstellungen (Alternative)

Wir empfehlen dringend die Verwendung des **Exchange**-Kontotyps. Sollten Sie alternativ eine Verbindung über IMAP herstellen müssen, verwenden Sie bitte folgende Daten:

### IMAP (Posteingangsserver)

| Protokoll | IMAP |
| :--- | :--- |
| **Server** | `exchange.uni-mannheim.de` |
| **Port** | `993` |
| **Sicherheitstyp/Verschlüsselung** | `SSL/TLS` |
| **Benutzername** | `Uni-ID` |
| **Passwort** | Passwort Ihrer Uni-ID |

### SMTP (Postausgangsserver)

| Einstellung | Wert |
| :--- | :--- |
| **Server** | `exchange.uni-mannheim.de` |
| **Port** | `587` |
| **Sicherheitstyp/Verschlüsselung** | `STARTTLS` |
| **Authentifizierung erforderlich** | Ja |
| **Benutzername** | `Uni-ID` |
| **Passwort** | Passwort Ihrer Uni-ID |
