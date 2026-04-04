---
title: "Anleitung: Spam-Wortfilter in Outlook/Exchange einrichten und verwalten"
source_url_de: None
source_url_en: https://www.uni-mannheim.de/en/it/instructions/microsoft-exchange/spam-word-filter/
category: Services
tags: ['Spam', 'Wortfilter', 'Outlook', 'Exchange', 'Regeln', 'Posteingang', 'Junk-Ordner']
language: de
---

# Wortfilter in Posteingangsregeln zur Bekämpfung von Spam-Mails

Sie können einen eigenen Spam-Wortfilter für Ihr Exchange Postfach erstellen, um unerwünschte E-Mails zu filtern.

**Hinweis:** Falls Sie keine E-Mails mehr von ganzen Adressbereichen („Domains“) erhalten möchten, prüfen Sie bitte die [Mail Gateway Anleitung](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/proxmox-@gateway/#c347511) im Kapitel „Blacklist“.

## 1. Neue Spam-Wortfilter-Regel erstellen

Folgen Sie diesen Schritten, um die erste Regel einzurichten:

1. **Outlook Web App (OWA) aufrufen:** Gehen Sie zu [https://exchange.uni-mannheim.de](https://exchange.uni-mannheim.de).
1. **Anmelden:** Geben Sie Ihre Uni-ID und Ihr zugehöriges Passwort ein und klicken Sie auf „Anmelden“.
1. **Einstellungen öffnen:** Klicken Sie rechts oben auf das Zahnrad-Symbol, um die Einstellungen zu öffnen, und wählen Sie anschließend „Optionen“.
1. **Regeln aufrufen:** Klicken Sie im Menü auf „Posteingangs- und Aufräumregeln“ und klicken Sie auf das „+“-Symbol.
1. **Regel definieren:** Geben Sie einen Namen für die Regel ein. Klicken Sie unter „Wenn die Nachricht eintrifft […]“ auf das Dropdown-Menü, wählen Sie „Enthält diese Wörter“ und anschließend „im Betreff…“.
1. **Wörter hinzufügen:** Im sich öffnenden Fenster geben Sie nacheinander die gewünschten Wörter ein, die Sie filtern möchten. Klicken Sie nach jedem Wort auf das „+“-Symbol und bestätigen Sie abschließend mit einem Klick auf „OK“.
1. **Aktion festlegen:** Wählen Sie unter „Alle folgenden Aktionen ausführen“ die Aktion „Verschieben, kopieren, oder löschen“ und wählen Sie dort „Nachricht in Ordner verschieben…“.
1. **Zielordner wählen:** Wählen Sie Ihren Junk Ordner aus und bestätigen Sie mit einem Klick auf „OK“.
1. **Regel speichern:** Legen Sie die Regel abschließend mit einem Klick auf „OK“ an.

## 2. Bestehende Spam-Wortfilter-Regel ergänzen

Um die Regel nachträglich um weitere Wörter zu erweitern, gehen Sie wie folgt vor:

1. **Regeln aufrufen:** Gehen Sie wie in der Anleitung oben zu den „Posteingangs- und Aufräumregeln“.
1. **Regel bearbeiten:** Markieren Sie die bestehende Spam-Wortfilter-Regel mit einem Klick und klicken Sie anschließend auf das Stift-Symbol, um sie zu bearbeiten.
1. **Wörterliste öffnen:** Im sich öffnenden Fenster klicken Sie bei den Bedingungen auf die Wörterliste, um diese zu öffnen.
1. **Speichern:** Fügen Sie die weiteren Wörter hinzu und speichern Sie die Regel abschließend ab.

______________________________________________________________________

**Tipp:** Prüfen Sie regelmäßig Ihren Junk Ordner, um zu überprüfen, ob nach dem Anlegen der Wortfilter-Regel neue E-Mails dort landen.
