---
title: Exchange Postfach mit Thunderbird auf Linux einbinden
source_url_de: https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/einbinden-linux/
source_url_en: https://www.uni-mannheim.de/en/it/instructions/microsoft-exchange/adding-an-exchange-account-to-linux/
category: Benutzung
tags: ['Thunderbird', 'Exchange', 'Linux', 'IMAP', 'Postfach', 'Einbindung', 'Uni-ID']
language: de
---

# Anleitung: Exchange Postfach mit Thunderbird auf Linux verbinden

Diese Anleitungen zeigen, wie Sie Ihr Exchange Postfach auf Linux-Geräten mit Thunderbird verbinden. **Bitte beachten Sie:** Diese Schritte können erst durchgeführt werden, nachdem Ihr Exchange Postfach eingerichtet wurde.

**Wichtiger Hinweis zu Synchronisation und Empfehlung:**
Die Universitäts-IT kann die dauerhafte Funktionalität der Synchronisierung von Kalender und Kontakten zwischen Thunderbird und Exchange nicht garantieren und bietet hierfür keinen Support an. Wir empfehlen daher ausdrücklich die Nutzung der **Outlook-Clients für Windows/Mac** oder des [Outlook Web-Clients](https://exchange.uni-mannheim.de/owa) für die Verwaltung Ihres Exchange Postfachs.

## 1. E-Mail-Konto mit Thunderbird verbinden

### Vorbereitung: Exchange-Absender-Adresse ermitteln

1. Öffnen Sie Ihren Internetbrowser (z. B. FireFox oder Chrome) und rufen Sie [https://exchange.uni-mannheim.de](https://exchange.uni-mannheim.de) auf.
1. Melden Sie sich mit Ihrer Uni-ID und dem zugehörigen Passwort an.
1. Klicken Sie nach der Anmeldung auf das Profilbild rechts oben. Ihre Exchange-Absender-Adresse wird in einem Pop-up angezeigt.
1. **Notieren Sie sich diese Adresse** – dies ist die Exchange-Absender-Adresse, die Sie für die Einrichtung in Thunderbird benötigen.

### Einrichtung in Thunderbird

1. Starten Sie Thunderbird und klicken Sie rechts oben auf das Anwendungsmenü, wählen Sie dort die Option „Neu“ und anschließend „Bestehendes E-Mail-Konto…“.
1. Geben Sie Ihren Namen, Ihre **Exchange-Absender-Adresse** und das Passwort Ihrer Uni-ID ein. Klicken Sie auf „Manuell einrichten…“.
1. Tragen Sie in die folgenden Felder die angegebenen Werte ein und klicken Sie auf „Fertig“.

**Server-Einstellungen:**

| Protokoll | IMAP |
| :--- | :--- |
| **Posteingangs-Server** | |
| Server | exchange.uni-mannheim.de |
| Port | 993 |
| SSL | SSL/TLS |
| Authentifizierung | Passwort, normal |
| Benutzername | Uni-ID |
| **Postausgangs-Server** | |
| Server | exchange.uni-mannheim.de |
| Port | 587 |
| SSL | STARTTLS |
| Authentifizierung | Passwort, normal |
| Benutzername | Uni-ID |

Nach der Einrichtung verbindet sich Thunderbird mit Ihrem Postfach und synchronisiert Ihre E-Mails.

### Systemordner in Thunderbird anpassen

Um sicherzustellen, dass die Ordnerstruktur in Thunderbird mit der des Microsoft Exchange OWA (Outlook Web Access) übereinstimmt, gehen Sie wie folgt vor:

1. **Ordner abonnieren:** Klicken Sie mit der rechten Maustaste auf Ihr E@Konto und wählen Sie „Abonnieren…“.
1. Klicken Sie auf „Aktualisieren“ (1), um die aktuelle Ordnerliste zu empfangen. Setzen Sie anschließend die Haken bei allen Ordnern, die in Thunderbird sichtbar sein sollen (2). Klicken Sie auf „Abonnieren“ (3) und abschließend auf „OK“ (4).
1. **Standardordner festlegen (Beispiel: Gesendete Elemente):**
   - Klicken Sie erneut mit der rechten Maustaste auf Ihr E@Konto und wählen Sie „Einstellungen“.
   - Gehen Sie im linken Menü zu „Kopien & Ordner“ (1).
   - Aktivieren Sie im mittleren Bereich unter „Beim Senden von Nachrichten automatisch“ die Option „Anderer Ordner“ (2).
   - Klicken Sie auf den Dropdown-Pfeil (3) und wählen Sie unter Ihrem E@Account (**NICHT** „Lokaler Ordner“) den Ordner „Gesendete Elemente“ (4).

Nach einem Neustart sollten die Systemordner korrekt angezeigt werden.

## 2. Kalender und Kontakte synchronisieren

Um Kalender und Kontakte zu synchronisieren, müssen zwei Add-ons installiert und konfiguriert werden:

1. **Add-ons installieren:**
   - Klicken Sie in Thunderbird rechts oben auf das Anwendungsmenü und wählen Sie „Add-ons“.
   - Suchen Sie nach `tbsync` und fügen Sie das Add-on „TbSync“ hinzu.
   - Wiederholen Sie diesen Vorgang für das Add-on „Provider für Exchange ActiveSync“.
1. **Synchronisation einrichten:**
   - Schließen Sie die Addon-Tabs und wechseln Sie zum Hauptfenster von Thunderbird.
   - Klicken Sie unten rechts auf „TbSync: Leerlauf“.
   - Wählen Sie in der Kontoverwaltung „Konto Aktionen“ > „Neues Konto hinzufügen“ > „Exchange-ActiveSync“.
   - Wählen Sie „Benutzerspezifische Konfiguration“ und tragen Sie Ihre Daten ein. Im Feld „Benutzername (E-Mail Adresse)“ geben Sie `ihread\Uni-ID` ein (z. B. `ad\mamuster`). Klicken Sie auf „Konto hinzufügen“.
   - Aktivieren Sie das Konto und setzen Sie den Haken bei „Konto aktivieren und synchronisieren“.
   - Wählen Sie im Auswahlmenü die Häkchen bei **„Kontakte“** und **„Kalender“**.
   - Setzen Sie eine periodische Synchronisation (mindestens ≥ 5 Minuten) und klicken Sie auf „Jetzt synchronisieren“.

Wenn neben Ihrem Kontonamen ein grünes Häkchen erscheint, ist die Synchronisation erfolgreich.

**Globales Adressbuch:** Um Kontakte aus dem globalen Adressbuch der Universität zu suchen, wechseln Sie in Thunderbird zum Adressbuch, markieren Sie Ihr neues Exchange Konto und suchen Sie im Suchfeld oben rechts.

## Hinweise und Fehlerbehebung

- **Funktionsumfang:** Thunderbird verbindet sich über das IMAP-Protokoll nur mit eingeschränktem Funktionsumfang. Die Ordnerstruktur wird nicht automatisch übernommen; das Mapping muss manuell in den Einstellungen vorgenommen werden.
- **Fehlermeldungen beim Synchronisieren:**
  1. Vergewissern Sie sich, dass Thunderbird im Onlinemodus ist (Button unten links prüfen).
  1. Falls das Problem weiterhin besteht, entfernen Sie den Haken bei „Konto aktivieren und synchronisieren“ und wechseln Sie auf den Reiter „Kontoeinstellungen“, um die Konto-Eingaben erneut zu überprüfen.
