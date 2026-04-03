---
title: Anleitung und FAQ zum Exchange E-Mail-Service der Universität Mannheim
source_url_de: https://www.uni-mannheim.de/it/anleitungen/e-@und-kalender/
source_url_en: https://www.uni-mannheim.de/en/it/instructions/e-mail-and-calendar/
category: Services
tags: ['Exchange', 'E-Mail', 'Kalender', 'Anleitung', 'Outlook', 'Uni-ID', 'Postfach', 'Kommunikation']
language: de
---

# E-Mail- und Kalender-Service: Leitfaden und FAQ

Dieser Leitfaden bietet Informationen zum Zugriff auf Ihr Exchange Postfach sowie Antworten auf häufig gestellte Fragen zur Nutzung des universitären E-Mail-Services.

## 📧 Zugriff auf Ihr Exchange Postfach

Sie haben zwei primäre Möglichkeiten, auf Ihr Exchange Postfach zuzugreifen:

1. **Webmailer OWA (Outlook Web App):** Direkter Zugriff über den Webbrowser.
   - [Anleitung Login OWA](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/login-outlook-web-app/)
1. **E-Mail-Client:** Für die Bearbeitung von E-Mails, Terminen und Adressen über einen lokalen Client.
   - [Anleitungen zur Client-Verbindung](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/login-outlook-web-app/) (Hinweis: Die spezifischen Verbindungsschritte werden in den jeweiligen Anleitungen erklärt.)

## ⚙️ Erweiterte Exchange-Funktionen und Anleitungen

Für spezifische Aufgaben im Umgang mit Ihrem Postfach finden Sie detaillierte Anleitungen zu folgenden Themen:

- [Kalender freigeben](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/kalender-freigabe/)
- [Archiv Mailbox verwalten](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/archiv-mailbox/)
- [Spam Quarantäne-Box (Proxmox Mail Gateway)](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/proxmox-@gateway/)
- [Spam-Wortfilter-Regel erstellen](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/spam-wortfilter/)
- [Gelöschte E-Mails wiederherstellen](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/wiederherstellen-geloeschter-mails/)
- [Anzeigenamen/Adresse meiner Funktionskennung(en) anpassen](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/funktionskennung/)
- [Weiterleitungen an universitäre E-Mail-Adressen einrichten](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/weiterleitung-einrichten/)
- [Weiterleitungs- und andere Regeln für Alias-Adressen erstellen](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/postfachregeln-fuer-aliasadressen/)
- [Ordner im Webmailer OWA freigeben oder einen freigegebenen Ordner hinzufügen](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/ordner-freigeben-outlook-web-app/)
- [Abwesenheitsnotiz via Outlook oder Webmailer OWA einstellen](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/abwesenheitsnotizen/)
- [Kontakte freigeben](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/kontakte-freigabe/)
- [E-Mail aus einem Funktionspostfach im Webmailer OWA erstellen](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/funktionspostfach-im-webmailer/)
- [Mail Header in Outlook auslesen und tatsächlichen Absender bestimmen](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/outlook-@header-auslesen/)
- [Mailinglisten (z. B. für Massenversand von E-Mails) erstellen und verwalten mit Mailman](https://www.uni-mannheim.de/it/anleitungen/mailman/)
- [Signatur für Ihren Uni-Mailaccount erstellen](https://signatur.uni-mannheim.de/)

## ❓ Häufig gestellte Fragen (FAQ)

### E-Mail-Adresse und Adressstruktur

**Wie lautet meine Exchange E-Mail-Adresse?**
Sie können Ihre Exchange E-Mail-Adresse im [Outlook Web-Client](https://exchange.uni-mannheim.de/owa) über Ihren Webbrowser einsehen.

- **Anleitung:** Rufen Sie [https://exchange.uni-mannheim.de/](https://exchange.uni-mannheim.de/) auf, melden Sie sich mit Ihrer Uni-ID und dem Passwort an. Klicken Sie anschließend auf das Profilbild oben rechts; Ihre E-Mail-Adresse wird im Pop-Up angezeigt.
- [Videoanleitung](https://www.uni-mannheim.de/media/Einrichtungen/it/Anleitungen/Exchange/FAQ/Exchange_Absender_Adresse_GER.mp4)
- **Hinweis zur Adressstruktur:** Aufgrund der einheitlichen Adressstruktur entfallen zukünftig die Subdomains (Adress-Zusätze vor „uni-mannheim.de“) für Absenderadressen. Sie können jedoch weiterhin E-Mails empfangen, die an Adressen mit einer Subdomain gesendet werden.

### E-Mail-Empfang und Formatierung

**Warum erhalte ich manche Mails als Anhang?**
Eingehende E-Mails von extern, die **signiert** wurden, können aus technischen Gründen nicht den Hinweis „External Sender: Achtung bei Links […]“ im Originalformat erhalten. Das Exchange Mailsystem erstellt daher eine neue leere E-Mail, fügt den Hinweis hinzu und hängt die ursprüngliche E-Mail als Anhang an.

- **Tipp:** Wenn Sie dem Inhalt vertrauen, ziehen Sie den Anhang mit der Maus in den Posteingang. Die ursprüngliche E-Mail wird dann im Posteingang erstellt und kann normal beantwortet werden.
- *Alternative:* Ein anderer FAQ-Eintrag zeigt eine Variante des externen-Absender-Hinweises, bei der signierte E-Mails nicht als Anhang gepackt werden.

**Wie kann ich den „externe-Absender-Hinweis“ ändern?**
Sie können die Markierung eingehender externer E-Mails über [MyUni-ID](https://id.uni-mannheim.de/login.php) (Reiter E-Mail/Uni-ID → Externe E-Mails) anpassen. Es stehen folgende Ansichts-Optionen zur Auswahl:

- **Standard-Hinweistext:** Standardmäßig ausgewählt, geeignet für PC/Laptop. Verschlüsselte/signierte externe E-Mails werden als Anhang im Original angefügt.
- **Kurzer Hinweistext:** Minimale Veränderung des Vorschautextes, ideal für Smartphones. Verschlüsselte & signierte externe E-Mails werden als Anhang im Original angefügt.
- **Präfix im Betreff:** Fügt einen Präfix an den Betreff an. Je nach Client kann dies dazu führen, dass E-Mails einzeln und nicht mehr als Teil einer Konversation dargestellt werden. Verschlüsselte und signierte externe E-Mails werden normal empfangen und nicht als Anhang gepackt.

### Kalender und Terminplanung

**Warum erscheinen meine Outlook-Termine nicht in Microsoft Teams und umgekehrt?**
Das neue Exchange Mailsystem ist nicht vollständig mit den Microsoft 365 Cloud-Diensten (wie Teams) verbunden. Aktuell sind Ihr Teams-Kalender und Ihr Exchange-Kalender zwei getrennte Kalender, die sich nicht synchronisieren.

- *Hinweis:* Diese Funktion ist auf der M365-Instanz für Studierende nicht verfügbar.

**Warum kann ich meinen Kalender nicht freigeben?**
Die Kalenderfreigabe ist auf interne Postfächer mit Adressen der Domain „uni-mannheim.de“ beschränkt. Das Freigeben für externe Domains (z. B. „xyz@gmx.de“) wird abgelehnt.

- Bei Problemen bei der Freigabe für ein internes Uni-Mannheim-Postfach beachten Sie bitte die [Anleitung zur Freigabe von Kalendern](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/kalender-freigabe/).

**Warum kann ich keine Teams-Termine in Outlook erstellen?**

1. Beenden Sie Outlook und MS Teams und starten Sie beide Programme neu.
1. Falls das Problem bestehen bleibt, installieren Sie MS Teams neu, beenden Sie Outlook, starten Sie Teams, und rufen Sie danach Outlook auf.

- **Wichtig:** Sie können Teams-Termine nur für Ihren eigenen Kalender erstellen. Für freigegebene Kalender können Sie nur „normale“ Termine erstellen. Diese Funktion ist auf der M365-Instanz für Studierende grundsätzlich nicht vorhanden.

### Protokolle und Clients

**Wird das POP3 Protokoll noch zur Verfügung gestellt?**
Nein. POP3 ist ein veraltetes Protokoll. Es lädt E-Mails auf den lokalen Rechner herunter und löscht sie aus dem Exchange Postfach. Dies ist riskant, da bei einem Rechnerdefekt die E-Mails ohne Backup verloren gehen können. Daher ist die Einbindung über POP3 für die Postfächer des Exchange Mailsystems nicht akzeptabel.

**Warum kann ich die offizielle Outlook App nicht verwenden?**
Die offizielle Outlook App für Android & iOS verbindet sich nicht direkt mit dem Exchange Mailsystem der Universität, sondern mit Microsoft Servern. Diese Zwischenspeicherung von Daten (inkl. E-Mails der letzten 30 Tage) verletzt die universitären Anforderungen, keine E-Mails in der Cloud zu speichern. Daher wird der Zugriff blockiert.

### Suche und Adressbuch

**Warum findet die Outlook-Suche meine E-Mail nicht?**
Die Outlook-Anwendung durchsucht standardmäßig nur das **aktuell ausgewählte Postfach**. Wenn die gesuchte E-Mail in einem anderen, nicht ausgewählten Postfach liegt, wird sie nicht gefunden.

- **Lösung:** Geben Sie den Suchbegriff ein, klicken Sie links daneben auf „Aktuelles Postfach“ und wählen Sie anschließend „Alle Postfächer“ aus.
- **Standardeinstellung:** Um immer alle Postfächer zu durchsuchen, gehen Sie in Outlook zu *Datei* $\\rightarrow$ *Optionen* $\\rightarrow$ *Suchen* und wählen Sie „Allen Postfächern“.

**Warum finde ich im Outlook-Adressbuch einen Kontakt nicht?**
Stellen Sie sicher, dass Sie im Outlook-Adressbuch die **Globale Adressliste** und die Option **„Alle Spalten“** ausgewählt haben. Geben Sie dann den Namen ein und klicken Sie auf das Pfeil-Symbol.

### Funktionspostfächer

**Wo werden E-Mails gespeichert, die ich über ein Funktionspostfach versende?**
Seit dem 1.2.2023 werden alle E-Mails, die Sie über ein Funktionspostfach senden, sowohl in Ihrem persönlichen Postfach **als auch zusätzlich in Kopie** im Funktionspostfach unter „Gesendete Elemente“ gespeichert. Dies sorgt für eine übersichtliche Dokumentation der gesamten Kommunikation.

### Weitere Themen

- **Akademischer Titel anzeigen lassen:** Rufen Sie [MyUni-ID](https://id.uni-mannheim.de/) auf und setzen Sie unter „E-Mail | Uni-ID“ $\\rightarrow$ „Status Uni-ID“ den entsprechenden Haken. Korrekturen müssen direkt bei der Personalabteilung erfolgen.
- **Barrierefreiheit:** Hinweise zum Versenden und Empfangen barrierefreier Nachrichten finden Sie in der Anleitung [Barrierefreiheit](https://www.uni-mannheim.de/it/anleitungen/barrierefreiheit/).
