---
title: Anleitung und FAQ zu Microsoft Exchange an der Universität Mannheim
source_url_de: N/A
source_url_en: https://www.uni-mannheim.de/en/it/instructions/microsoft-exchange/
category: Benutzung
tags: ['Exchange', 'E-Mail', 'Kalender', 'Anleitung', 'OWA', 'Postfach', 'Uni-Mannheim', 'Kommunikation']
language: de
---

# Microsoft Exchange Universität Mannheim

Mit Microsoft Exchange steht allen Beschäftigten und Studierenden der Universität Mannheim ein einheitliches System für E-Mail, Kalender und Adressbücher zur Verfügung.

## Zugriff auf Ihr Exchange-Postfach

Sie haben zwei Hauptmöglichkeiten, auf Ihr Exchange Postfach zuzugreifen:

- **Über den Webmailer OWA (Outlook Web App):** [Anleitung Login OWA](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/login-outlook-web-app/)
- **Über einen E-Mail-Client:** Um Ihre E-Mails, Termine und Adressen über einen E-Mail-Client bearbeiten zu können, finden Sie in den folgenden Anleitungen die Verbindungsvorgänge für Ihr Exchange-Postfach.

**\[Exchange Video-Tutorials\](Link zu Video-Tutorials einfügen)**

## Weitere Exchange-Anleitungen und Funktionen

Für spezifische Aufgaben finden Sie detaillierte Anleitungen zu folgenden Themen:

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

## Häufig gestellte Fragen (FAQ)

Hier finden Sie Antworten auf häufig gestellte Fragen zur Nutzung von Microsoft Exchange.

### Wie lautet meine Exchange E-Mail-Adresse?

Sie können Ihre Exchange E-Mail-Adresse über Ihren Webbrowser (z.B. FireFox, Edge, Chrome) im [Outlook Web-Client](https://exchange.uni-mannheim.de/owa) einsehen.

**Videoanleitung:** [Die Anleitung als Video](https://www.uni-mannheim.de/media/Einrichtungen/it/Anleitungen/Exchange/FAQ/Exchange_Absender_Adresse_GER.mp4)

**Vorgehen:**

1. Rufen Sie in Ihrem Webbrowser [https://exchange.uni-mannheim.de/](https://exchange.uni-mannheim.de/) auf.
1. Melden Sie sich mit Ihrer Uni-ID und dem dazugehörigen Passwort an.
1. Klicken Sie nach der Anmeldung auf das Profilbild rechts oben; Ihre E-Mail-Adresse wird im Pop-Up angezeigt.

**Hinweis zur Adressstruktur:** Aufgrund der einheitlichen Adressstruktur fallen die Subdomains (Adress-Zusätze vor „uni-mannheim.de“, z.B. @\*\*unit.\*\*uni-mannheim.de) zukünftig für Absenderadressen weg. Sie können jedoch weiterhin E-Mails empfangen, die an Adressen mit einer Subdomain gesendet werden.

### Warum erhalte ich manche Mails als Anhang?

Eingehende E-Mails von extern, die **signiert** wurden, können aus technischen Gründen nicht den Hinweis „External Sender: Achtung bei Links […]“ im Original erhalten. Daher erstellt das Exchange Mailsystem eine neue leere E-Mail, fügt diesen Hinweis ein und hängt die ursprüngliche E-Mail als Anhang an.

**Empfehlung:** Wenn Sie dem Inhalt der ursprünglichen E-Mail vertrauen oder die Warnung gelesen haben, ziehen Sie den Anhang mit der Maus in den Posteingang. Dadurch wird die ursprüngliche E-Mail im Posteingang erstellt, sodass Sie normal darauf antworten können.

*Hinweis:* Ein anderer FAQ-Eintrag zeigt eine Variante des externen-Absender-Hinweises, bei der signierte E-Mails nicht als Anhang gepackt, sondern normal empfangen werden.

### Wie kann ich den „externe-Absender-Hinweis“ ändern?

Eingehende E-Mails von extern werden in Ihrem Postfach entsprechend markiert. Diese Markierung können Sie über [MyUni-ID](https://id.uni-mannheim.de/login.php) (Reiter E-Mail/Uni-ID → Externe E-Mails) nach Ihren Wünschen anpassen.

**Verfügbare Ansichts-Optionen:**

- **Standard-Hinweistext:** Standardmäßig ausgewählt und für die Nutzung von E-Mail-Anwendungen auf PC/Laptop geeignet. Verschlüsselte und signierte externe E-Mails werden als Anhang im Original angefügt.
- **Kurzer Hinweistext:** Diese Variante verändert den Vorschautext einer Nachricht am geringsten und eignet sich besonders bei der Nutzung von Smartphones. Verschlüsselte & signierte externe E-Mails werden als Anhang im Original angefügt.
- **Präfix im Betreff:** Diese Variante fügt an den Anfang des Betreffs einen Präfix ein. Je nach E-Mail-Client kann dies dazu führen, dass E-Mails nicht mehr als Bestandteil einer Konversation, sondern einzeln dargestellt werden. Verschlüsselte und signierte externe E-Mails werden normal empfangen und nicht als Anhang gepackt.

### Warum erscheinen meine Outlook-Termine nicht in Microsoft Teams und umgekehrt?

Das neue Exchange Mailsystem ist nicht vollständig mit den Microsoft 365 Cloud-Diensten der Universität, zu denen auch Teams gehört, verbunden. Daher sind aktuell Ihr Microsoft Teams Kalender und Ihr Exchange Kalender zwei voneinander getrennte, eigene Kalender, die sich nicht gegenseitig synchronisieren.

*Hinweis:* Diese Funktion ist auf der M365-Instanz für Studierende nicht vorhanden.

### Warum kann ich meinen Kalender nicht freigeben?

Die Kalenderfreigabe ist auf interne Postfächer mit Adressen „...@uni-mannheim.de“ beschränkt, also innerhalb der Domain „uni-mannheim.de“. Wird versucht, den Kalender für andere Domains (z.B. „xyz@gmx.de“) freizugeben, wird dies als externe Adresse abgelehnt.

Falls Sie Ihren Kalender für ein Uni-Mannheim-internes Postfach freigeben möchten und dennoch eine Fehlermeldung erhalten, folgen Sie bitte der [Anleitung zur Freigabe von Kalendern](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/kalender-freigabe/).

### Warum kann ich die offizielle Outlook App nicht verwenden?

Die offizielle Outlook App für Android & iOS verbindet sich nicht direkt mit dem Exchange Mailsystem der Universität, sondern mit Microsoft Servern. Dabei werden diverse Daten, einschließlich aller E-Mails der letzten 30 Tage, auf diesen Microsoft Servern zwischengespeichert. Dies verletzt die universitären Anforderungen, keine E-Mails in der Cloud zu speichern, weshalb der Zugriff blockiert wird.

### Warum findet die Outlook-Suche meine E-Mail nicht?

Die Outlook-Anwendung durchsucht beim Starten einer Suche standardmäßig das **aktuell ausgewählte Postfach**. Wenn Sie mehrere Postfächer eingebunden haben und die gewünschte E-Mail in einem anderen, nicht ausgewählten Postfach liegt, wird diese nicht angezeigt.

**Um alle Postfächer zu durchsuchen:**

1. Geben Sie Ihren Suchbegriff ein.
1. Klicken Sie links daneben auf „Aktuelles Postfach“ und wählen Sie anschließend „Alle Postfächer“ aus.

**Standardmäßig über alle Postfächer suchen lassen:**

1. Öffnen Sie Outlook auf Ihrem Rechner.
1. Klicken Sie links oben auf „Datei“ und dann unten links auf „Optionen“.
1. Klicken Sie im sich öffnenden Fenster auf den Reiter „Suchen“.
1. Wählen Sie „Allen Postfächern“ aus und bestätigen Sie mit „OK“.

### Warum finde ich im Outlook-Adressbuch einen Kontakt nicht?

Wenn Sie einen Kontakt nicht finden, gehen Sie bitte wie folgt vor:

1. Öffnen Sie das Outlook Adressbuch.
1. Vergewissern Sie sich, dass die Globale Adressliste und die Option „Alle Spalten“ ausgewählt sind.
1. Geben Sie den gewünschten Namen in das Suchfeld ein und klicken Sie auf das Pfeil-Symbol.

### Warum kann ich keine Teams-Termine in Outlook erstellen?

1. Beenden Sie Outlook und MS Teams und starten Sie beide Programme neu.
1. Sollte das Problem bestehen, installieren Sie MS Teams neu und beenden Sie Outlook. Starten Sie Teams nach der Neuinstallation und rufen Sie anschließend Outlook auf.

**Wichtige Hinweise:**

- Sie können Teams-Termine nur für Ihren eigenen Kalender erstellen. Für freigegebene Kalender können Sie nur „normale“ Termine erstellen.
- Diese Funktion ist auf der M365-Instanz für Studierende grundsätzlich nicht vorhanden.

### Wird das POP3 Protokoll noch zur Verfügung gestellt?

Nein. Das POP3 Protokoll ist ein veraltetes Mailprotokoll. Es lädt E-Mails auf den lokalen Rechner der Nutzer\*innen herunter und löscht diese im Exchange Postfach. Bei einem Defekt oder Komplikationen mit dem Rechner sind diese E-Mails ohne Backup verloren und nicht wiederherstellbar. Daher ist die Einbindung über POP3 für die Postfächer des Exchange Mailsystems nicht akzeptabel.

### Wie kann ich meinen akademischen Titel in Exchange anzeigen lassen?

Um Ihren akademischen Titel im Exchange Anzeigenamen erscheinen zu lassen, rufen Sie die Seite [MyUni-ID](https://id.uni-mannheim.de/) auf und setzen Sie unter „E-Mail | Uni-ID“ → „Status Uni-ID“ unten den entsprechenden Haken. Korrekturen an dem gespeicherten akademischen Grad müssen direkt bei der Personalabteilung der Universität Mannheim beantragt werden.

### Wo werden E-Mails gespeichert, die ich über ein Funktionspostfach versende?

Seit dem 1.2.2023 werden alle E-Mails, die Sie über ein Funktionspostfach senden, nach Aktivierung einer Komforteinstellung sowohl in Ihrem persönlichen Postfach **als auch zusätzlich in Kopie** im Funktionspostfach unter „Gesendete Elemente“ gespeichert. Dies vereinfacht die Verwaltung der gesamten Kommunikation.

**Informationen für Administratoren:**
Sind Sie Admin an einem Lehrstuhl oder in einer Einrichtung? [Hier finden Sie alle notwendigen Informationen](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/informationen-admins/) für die Unterstützung beim Umzug auf das Exchange Mailsystem.
