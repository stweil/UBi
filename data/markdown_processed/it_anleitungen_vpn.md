---
title: Anleitung zur Installation und Nutzung des VPN-Clients der Universität Mannheim
source_url_de: https://www.uni-mannheim.de/it/anleitungen/vpn/
source_url_en: https://www.uni-mannheim.de/en/it/instructions/vpn/
category: Services
tags: ['VPN', 'Installation', 'Verbindung', 'Uni-ID', 'Zugriff', 'Client', 'Remote-Zugriff']
language: de
---

# VPN-Client: Anleitung für den sicheren Zugriff auf universitäre Ressourcen

Einige wichtige Dienste der Universität Mannheim, wie Bibliotheksdatenbanken oder der FileService, sind nur über eine gesicherte Verbindung auf dem Campus zugänglich. Für den Zugriff von zu Hause oder unterwegs ist daher die Einrichtung einer VPN-Verbindung zwingend erforderlich.

## 🧑‍💻 Wer kann den VPN-Client nutzen?

Der VPN-Client steht ausschließlich folgenden Gruppen zur Verfügung:

- Beschäftigte der Universität Mannheim
- Immatrikulierte Promovierende
- Studierende (inkl. Senior- und Gaststudierende)
- Privatdozent\*innen der Universität Mannheim

## 🔑 Vorbereitung und Support

Bevor Sie mit der Installation beginnen, beachten Sie bitte folgende Punkte:

- **Zugangsdaten:** Sie benötigen Ihre **Uni-ID** und das dazugehörige Passwort.
- **Passwort vergessen?** Nutzen Sie die [Anleitung zur Passwortrücksetzung](https://www.uni-mannheim.de/it/anleitungen/passwort/).
- **Uni-ID oder Passwort vergessen?** Wenden Sie sich bitte an den Support:
  - Telefon: +49 621 181-2000
  - E-Mail: itsupport@uni-mannheim.de

## 🌐 VPN-Profile: WebVPN vs. WebVPN-Split

Beim Aufbau der Verbindung werden Ihnen zwei Profile zur Auswahl gestellt. Die Wahl des Profils bestimmt, welche Daten über den VPN-Tunnel geleitet werden:

1. **WebVPN (Standardprofil):**
   - **Funktion:** Der **komplette Internetverkehr** wird durch den VPN-Tunnel geleitet.
   - **Wann nutzen:** Dieses Profil ist **zwingend erforderlich**, wenn Sie auf Online-Bibliotheksdatenbanken zugreifen müssen.
1. **WebVPN-Split:**
   - **Funktion:** Nur der Datenverkehr, der zur Universität Mannheim gehört, wird durch den VPN-Tunnel geleitet. Der restliche Internetverkehr läuft über Ihre normale Verbindung.
   - **Vorteil:** Die Verbindung ist vergleichsweise schneller.
   - **Wann nutzen:** Wir empfehlen dieses Profil für Mitarbeitende der Universität. **Achtung:** Mit diesem Profil ist kein Zugriff auf die Bibliotheksdatenbanken möglich.

## ❓ Häufige Fragen und Fehlerbehebung

### ⚠️ Fehler: AnyConnect Client funktioniert nicht

**Fehlermeldung:** „The VPN client agent was unable to create the interprocess communication depot“
**Mögliche Ursache:** Auf einem oder mehreren Netzwerkinfaces ist die „Gemeinsame Nutzung der Internetverbindung“ aktiviert.
**Lösung:** Deaktivieren Sie die „Gemeinsame Nutzung der Internetverbindung“:

1. Systemsteuerung $\\rightarrow$ Netzwerk- und Freigabecenter.
1. Rechtsklick auf den betroffenen Netzwerkadapter (LAN/Drahtlos) $\\rightarrow$ Eigenschaften.
1. Reiter „Freigabe“ öffnen und das Häkchen bei „Anderen Benutzern im Netzwerk gestatten, diese Verbindung des Computers als Internetverbindung zu verwenden“ entfernen.

### 📚 Zugriff auf Online-Bibliotheken

**Problem:** Auf einige Online-Bibliotheken kann via VPN nicht zugegriffen werden.
**Lösung:**

1. **Profilwahl:** Wählen Sie **immer** das **WebVPN** Profil, um Bibliotheksdatenbanken nutzen zu können.
1. **Alternative:** Bitte beachten Sie zusätzlich den [Hinweis zur Datenbanknutzung](https://www.bib.uni-mannheim.de/datenbanknutzung/).

### 📊 Welche Daten gehen über den VPN-Tunnel?

Sie entscheiden über das Profil, welche Daten gesichert werden:

- **WebVPN:** Der **komplette Internetverkehr** wird gesendet (Ausnahme: private Netzwerkbereiche wie 192.168.X.X).
- **WebVPN-Split:** Nur der Datenverkehr, der zur Universität Mannheim gehört, wird gesendet.

### 🐧 Fehler: Zertifikatsprüfung fehlschlägt (Linux)

**Problem:** Beim Verbinden mit Cisco AnyConnect erscheint die Fehlermeldung: „The following Certificate received from the Server could not be verified“.
**Ursache:** Der Client sucht nach SSL-Stammzertifikaten an verschiedenen Stellen, was bei Linux-Distributionen zu Problemen führen kann.
**Lösung (Linux):** Erstellen Sie einen symbolischen Link für die SSL-Stammzertifikate:

1. `cd /opt/.cisco/certificates/ca`
1. `ln -s /etc/ssl/certs/T-TeleSec_GlobalRoot_Class_2.pem`

______________________________________________________________________

**Zusätzliche Ressourcen:**

- [Speedtest der Uni Mannheim](https://www.uni-mannheim.de/it/services/speedtest/) zur Überprüfung der Verbindungskennzahl.
- [Alle Anleitungen auf einen Blick](https://www.uni-mannheim.de/it/anleitungen/) für weitere technische Hilfestellungen.
