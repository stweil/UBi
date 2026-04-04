---
title: Nameserver und DNS-Dienste der Universität Mannheim
source_url_de: (Nicht angegeben)
source_url_en: https://www.uni-mannheim.de/en/it/services/internet-and-servers/name-server/
category: Services
tags: ['Nameserver', 'DNS', 'IPv4', 'IPv6', 'Domain', 'Internet', 'IT-Dienste', 'Adressauflösung']
language: de
---

# Nameserver / DNS-Dienste

Die Universitäts-IT betreibt die zentralen Nameserver / DNS-Server für die Universität Mannheim.

## Technische Adressen

Die Nameserver sind für verschiedene Protokolle verfügbar:

**Über IPv4:**

- `134.155.96.51` (dns1.uni-mannheim.de)
- `134.155.96.52` (dns2.uni-mannheim.de)
- `134.155.96.53` (dns3.uni-mannheim.de)

**Über IPv6:**

- `2001:7c0:2900:60::869b:6033` (dns1.uni-mannheim.de)
- `2001:7c0:2900:60::869b:6034` (dns2.uni-mannheim.de)
- `2001:7c0:2900:60::869b:6035` (dns3.uni-mannheim.de)

## Funktionen der Nameserver

Nameserver sind zuständig für die Auflösung von Adressen und beinhalten folgende Kernfunktionen:

- **Adresszuordnung:** Umsetzung von öffentlichen und privaten IP-Adressen zu System-Namen und umgekehrt.
- **Mailrouting:** Bereitstellung von Informationen zum korrekten Routing von E-Mails.
- **Authoritative Dienste:** Die Nameserver sind für die Verbreitung registrierter IP-Adressen, System-Namen und des Mailroutings für alle eingetragenen Mailadressen der betriebenen Domains nach außen zuständig.

## Abgedeckte Domains und Netze

Die Universität Mannheim betreibt authoritative Nameserver für folgende Bereiche:

- `uni-mannheim.de`
- `uni-mannheim.eu`
- Die Netze `134.155.x.x`
- Die Netze `2001:7c0:600::`
- Zusätzlich werden Domains von Einrichtungen und Kooperationen der Universität Mannheim abgedeckt.

### Betrieb weiterer Domains

Bei entsprechender Notwendigkeit und Befürwortung besteht die Möglichkeit, andere Domains auf Servern innerhalb des Universitätsnetzes zu betreiben. Das Vorgehen hierzu ist unter [virtueller Webserver](https://www.uni-mannheim.de/it/services/internet-und-server/webhosting/#c223943) beschrieben.

Für weitere Informationen zur Domainstruktur der Universitätsnetze in Baden-Württemberg verweisen wir auf [BelWü](https://www.belwue.de/angebot/dienste/nameserver.html).
