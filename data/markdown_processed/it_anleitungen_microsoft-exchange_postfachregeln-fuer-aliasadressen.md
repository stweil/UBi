---
title: Postfachregeln für Aliasadressen in Microsoft Exchange
source_url_de: https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/postfachregeln-fuer-aliasadressen/
source_url_en: https://www.uni-mannheim.de/en/it/instructions/microsoft-exchange/mailbox-rules-for-alias-addresses/
category: Benutzung
tags: Postfachregeln, Alias, Exchange, Weiterleitung, OWA, Einrichtung, E-Mail-Adresse, Umstellung
language: de
---

# Postfachregeln für Aliasadressen in Microsoft Exchange

**Wichtiger Hinweis:** Diese Anleitung kann übersprungen werden, falls Sie keine Postfachregeln eingerichtet haben oder falls Ihre Regeln nicht explizit nur für einzelne Alias-Adressen gelten.

Aufgrund einer technischen Anpassung von Microsoft Exchange funktionieren Postfachregeln, die sich auf explizite E-Mail-Adressen („Aliasse“) beziehen, nach der Umstellung auf das Proxmox Mail Gateway anders als bisher.

- **Betroffen sind nur Regeln**, die nur dann greifen sollen, wenn eine E-Mail an eine **bestimmte Adresse** Ihres Postfachs eingeht.
- Regeln, die grundsätzlich für **alle** eingehenden E-Mails gelten sollen, funktionieren weiterhin wie gewünscht und erfordern keine Änderungen.

## Schritt-für-Schritt-Anleitung zur Anpassung der Regel (Alternative 3)

Folgen Sie diesen Schritten, um die vorhandene Regel anzupassen:

**Schritt 1:** Rufen Sie die [Outlook Web App (OWA)](https://exchange.uni-mannheim.de) auf.

**Schritt 2:** Melden Sie sich mit Ihrer Uni-ID und Ihrem zugehörigen Passwort an.

**Schritt 3:** Navigieren Sie zu Ihren Einstellungen: Klicken Sie rechts oben auf das Zahnrad-Symbol, um die Einstellungen zu öffnen, und wählen Sie anschließend „Optionen“.

**Schritt 4:** Klicken Sie im Menü auf „Posteingangs- und Aufräumregeln“ und fügen Sie ein neues Regelzeichen („+“) hinzu.

**Schritt 5:** Geben Sie einen Namen für die Regel ein. Unter „Wenn die Nachricht eintrifft […]“ wählen Sie das Dropdown-Menü und navigieren zu „Enthält diese Wörter“ > „in der Nachrichtenkopfzeile…“.

**Schritt 6:** Tragen Sie die gewünschte Adresse in das obere Feld ein. Klicken Sie auf „+“ und anschließend auf „OK“.

- **Wichtig bei Teil-Suchtreffern:** Wenn Sie beispielsweise „unituni-mannheim.de“ eintragen und das Postfach auch die Adresse „sekretariat.unituni-mannheim.de“ enthält, greift die Regel auch bei dieser längeren Adresse, da der Suchbegriff enthalten ist. In solchen Fällen sollten Sie Alternativen 1 oder 2 erneut prüfen oder diese Alias-Adresse aus der Regel entfernen.

**Schritt 7:** Wählen Sie die gewünschte Aktion aus, die mit E-Mails an diese Adresse ausgeführt werden soll (meist Weiter- oder Umleitungen). Für die Einrichtung einer Weiterleitung können Sie diese Anleitung nutzen: [https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/weiterleitung-einrichten/](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/weiterleitung-einrichten/)
