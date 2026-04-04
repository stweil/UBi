---
title: Spam-Quarantäne-Box (Proxmox Mail Gateway) Anleitung
source_url_de: https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/proxmox-@gateway/
source_url_en: https://www.uni-mannheim.de/en/it/instructions/microsoft-exchange/spam-quarantine-box-proxmox-mail-gateway-1/
category: Benutzung
tags: ['Spam', 'Phishing', 'Quarantäne', 'Mail Gateway', 'Uni-ID', 'Whitelist', 'Blacklist']
language: de
---

# Spam-Quarantäne-Box (Proxmox Mail Gateway)

Zur besseren Abwehr von Spam- und Phishing-Attacken wurde ein zentrales Mail Gateway (das Proxmox Mail Gateway) für alle Postfächer der Universität eingeführt. Erkennt Spam- oder Phishing-E-Mails werden nicht direkt ins Exchange Postfach zugestellt, sondern in die Quarantäne vorgehalten. Nach 30 Tagen werden diese E-Mails automatisch gelöscht.

In der Quarantäne-Box können Sie folgende Aktionen durchführen:

- E-Mails einsehen und löschen.
- E-Mails an Ihr Postfach weiterleiten.
- Absender whitelisten oder blacklisten.

## Zugriff auf die Quarantäne-Box

Sie können die Quarantäne-Box auf zwei Wegen erreichen:

1. **Täglicher Spam-Bericht:** Falls in den letzten 24 Stunden neue Spam-/Phishing-E-Mails eingegangen sind, wird einmal täglich eine Infomail an Ihr Exchange Postfach versandt. Die Links in dieser E-Mail führen direkt zur Quarantäne-Box.
1. **Webbrowser:** Die Quarantäne-Box ist jederzeit über folgenden Link erreichbar: [https://mailknast.uni-mannheim.de](https://mailknast.uni-mannheim.de)

**Anmeldung:**
| Feld | Wert |
| :--- | :--- |
| **Anmeldename** | `uni-id@ad.uni-mannheim.de` |
| **Passwort** | Passwort Ihrer Uni-ID |

***Hinweis zu Filtern:** Standardmäßig werden nur E-Mails der letzten 7 Tage angezeigt. Um ältere E-Mails (bis zu 30 Tage) einzusehen, muss der Datums-Filter angepasst werden.*

## Funktionen der Quarantäne-Box

Die Leseansicht bietet verschiedene Steuerelemente für die ausgewählte E-Mail:

| Button | Beschreibung |
| :--- | :--- |
| **Raw Umschalten** | Zeigt den Quellcode der ausgewählten E-Mail an. |
| **Spam Info umschalten** | Zeigt die Spam-Evaluations-Informationen der E-Mail an. |
| **Herunterladen** | Lädt die ausgewählte E-Mail als `.eml` Datei herunter. |
| **Whitelist** | Fügt den Absender zur persönlichen Whitelist hinzu. E-Mails von diesem Absender werden zukünftig nicht mehr als Spam gewertet und direkt zugestellt. Die ausgewählte E-Mail wird ebenfalls ins Postfach zugestellt. |
| **Blacklist** | Fügt den Absender zur persönlichen Blacklist hinzu. E-Mails von diesem Absender werden zukünftig sofort und unwiderruflich gelöscht, ohne in der Quarantäne vorgehalten zu werden. Die ausgewählte E-Mail wird gelöscht. |
| **Zustellen** | Stellt die ausgewählte E-Mail ins Exchange Postfach zu. |
| **Löschen** | Löscht die ausgewählte E-Mail unwiderruflich. |

## Whitelist und Blacklist Management

Über diese Bereiche können Adressen und Domains verwaltet werden, um den E-Mail-Fluss zu steuern.

### Whitelist (Direktzustellung)

Hier können Adressen und Domains hinzugefügt werden. E-Mails von diesen Quellen werden **ohne Spam-Überprüfung** direkt in Ihr Exchange Postfach zugestellt.

**Beispiele:**

- `@gmail.com`: Alle E-Mails von Absendern, die auf `@gmail.com` enden.
- `unit.uni-mannheim.de`: Alle E-Mails, die auf diesen Adressbereich enden (z. B. `muster@sekretariat-unit.uni-mannheim.de`).
- `melanie-muster@vertrieb-xyz.de`: Alle E-Mails von dieser spezifischen Adresse.

### Blacklist (Sofortige Löschung)

Hier können Adressen und Domains hinzugefügt werden. E-Mails von diesen Quellen werden **ohne Spam-Überprüfung direkt und unwiderruflich gelöscht**. Die Einträge werden analog zur Whitelist angelegt.
