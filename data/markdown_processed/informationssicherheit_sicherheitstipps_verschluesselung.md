---
title: Verschlüsselungsmethoden und Best Practices für die Datensicherheit
source_url_de: None
source_url_en: https://www.uni-mannheim.de/en/information-security/security-tips/encryption/
category: Services
tags: ['Verschlüsselung', 'Datensicherheit', 'Bitlocker', 'FileVault', 'Cloud', 'Datenmanagement']
language: de
---

# Verschlüsselung: Was und wie Sie Daten schützen

Diese Seite erklärt, warum und wie Sie verschiedene Arten von Daten – von lokalen Dateien bis zu Cloud-Speichern – verschlüsseln können, um sie vor unbefugtem Zugriff zu schützen.

## 💻 Verschlüsselung auf Computern

**Warum verschlüsseln?**
Wenn Ihr Computer gestohlen oder verloren geht, kann durch den Ausbau der Festplatte auf alle Daten zugegriffen werden. Eine Festplattenverschlüsselung schützt die Daten vor fremdem Zugriff.

- **Apple Geräte:** Nutzen Sie **FileVault**. [FileVault Anleitung](https://www.uni-mannheim.de/it/anleitungen/filevault/)
- **Windows:** Nutzen Sie **Bitlocker**. [Bitlocker Anleitung](https://www.uni-mannheim.de/informationssicherheit/infomaterial/anleitung-bitlocker/)
- **Linux:** Aufgrund der Vielfalt der Distributionen gibt es keine einheitliche Anleitung. Bitte erkundigen Sie sich bei Ihrer jeweiligen Distribution.

**Hinweis zur Universitäts-IT:**
Wenn Sie einen Computer über die Universitäts-IT bestellen oder einrichten lassen, wird die Festplatte durch die Beschäftigten der Universitäts-IT verschlüsselt (seit November 2022).

- **Überprüfung:** Sie können unter „Einstellungen\\Datenschutz und Sicherheit/BitLocker-verwalten“ prüfen, ob Ihre Festplatten verschlüsselt sind und dort bei Bedarf aktivieren.
- [Mehr Infos zur Verschlüsselung des digitalen Arbeitsplatzes](https://www.uni-mannheim.de/it/services/arbeitsplatz/digitaler-arbeitsplatz/verschluesselung/)

## 💾 Verschlüsselung externer Speichermedien

Externe Medien (USB-Sticks, SD-Karten, Festplatten) können leicht verloren gehen oder gestohlen werden. Zudem können Daten auf diesen Medien nicht immer zu 100% gelöscht werden.

- **Gesamtes Speichermedium verschlüsseln:** Dies ist mit **VeraCrypt** möglich. Beachten Sie, dass Administrator-Rechte für Installation und Verschlüsselung notwendig sind. [Anleitung VeraCrypt](https://www.uni-mannheim.de/informationssicherheit/infomaterial/anleitung-veracrypt/)
- **Erweiterbarer verschlüsselter Ordner:** Mit **Cryptomator** können Sie einen verschlüsselten Ordner anlegen, der jederzeit erweitert, ergänzt oder bearbeitet werden kann. [Anleitung Cryptomator](https://www.uni-mannheim.de/informationssicherheit/infomaterial/anleitung-cryptomator/)
- **Einzelne Dateien/Ordner:** Für Dateien oder Ordner, die nicht mehr bearbeitet werden müssen, eignet sich ein **verschlüsseltes ZIP-Archiv**. Folgen Sie der [Anleitung für verschlüsselte ZIP-Archive](https://www.uni-mannheim.de/informationssicherheit/infomaterial/anleitung-verschluesseltes-zip-archiv/).

## 📄 Verschlüsselung von Dokumenten und E-Mails

### Office Dokumente (Word, Excel etc.)

Einzelne Office Dokumente können mit dem integrierten Dokumentenschutz mittels eines Passworts verschlüsselt werden.

- [Detaillierte Anleitung zur Office-Dokumentenverschlüsselung](https://www.uni-mannheim.de/informationssicherheit/infomaterial/anleitung-office-dokumentenverschluesselung/)
- **Wichtig:** Das Passwort des Dokuments niemals per E-Mail versenden, sondern auf einem anderen Weg (persönlich, telefonisch oder per Brief).

### E-Mails

Der Versand von E-Mails ist wie das Versenden einer Postkarte; jeder kann den Inhalt lesen.

- **S/MIME-Verschlüsselung:** E-Mails können sicher über S/MIME übertragen werden. Hierfür benötigen Sie ein digitales Zertifikat, das mit einem Passwort verbunden ist.
  - Antragsformular und Infos zum Zertifikat: [Hier](https://www.uni-mannheim.de/it/services/digitale-zertifikate)

### Anhänge per E-Mail

Auch ohne S/MIME können einzelne Anhänge durch ein **verschlüsseltes ZIP-Archiv** geschützt werden. Übermitteln Sie das Passwort für das ZIP-Archiv nicht per E-Mail.

## ☁️ Verschlüsselung in verschiedenen Speichermedien

### 🌐 Netzlaufwerke der Universität Mannheim (NAS)

Auch hier wird die Nutzung der uni-internen Netzlaufwerke empfohlen.

- **Erweiterbarer Ordner:** Nutzen Sie **Cryptomator** für einen verschlüsselten Ordner. [Anleitung Cryptomator](https://www.uni-mannheim.de/informationssicherheit/infomaterial/anleitung-cryptomator/)
- **Einzelne Objekte:** Schützen Sie einzelne Ordner/Dateien mit einem **verschlüsselten ZIP-Archiv**. Beachten Sie, dass dieses Archiv nicht mehr erweitert werden kann.

### ☁️ Cloud-Dienste (OneDrive, Teams, OneNote & andere)

**Microsoft-Cloud (M365):**

- Bei der Verarbeitung von Daten in der M365-Cloud ist der Umgang mit den Informationen sorgsam zu gestalten (z.B. nur Verwaltungsdaten der Klassifizierung TLP white). [Nutzerrichtlinien M365 Cloud Services](https://www.uni-mannheim.de/it/nutzungsbedingungen/richtlinien-m-365-cloud-services/)
- **Erweiterbarer Ordner:** **Cryptomator** kann auch in der Cloud genutzt werden. Bei gemeinsamen Ordnern ist keine gleichzeitige Bearbeitung möglich. [Anleitung Cryptomator](https://www.uni-mannheim.de/informationssicherheit/infomaterial/anleitung-cryptomator/)
- **Einzelne Objekte:** Nutzen Sie ein **verschlüsseltes ZIP-Archiv**.

**Andere Cloud-Dienste (iCloud, Dropbox, GoogleDrive etc.):**

- **Warnung:** Das Informationssicherheitsteam rät von der dienstlichen Nutzung solcher Dienste ab, da die Datenverarbeitung durch Dritte nicht vollständig transparent ist.
- **Sicherheit:** Auch hier können Sie **Cryptomator** oder **verschlüsselte ZIP-Archive** nutzen.

## 🌐 Sichere Kommunikation im Internet

### Allgemeine Sicherheitstipps

- **Webseiten:** Achten Sie beim Eingeben vertraulicher Daten (z.B. Passwörter) auf das **Schloss-Symbol** im Browser-Adressfeld, um eine verschlüsselte Verbindung (HTTPS) zu gewährleisten.
- **WLAN:** Nutzen Sie bei der Nutzung von WLAN immer **WPA2**-verschlüsselte Verbindungen. Bei fremden oder öffentlichen Netzen (z.B. Hotel-WLAN) verwenden Sie ausschließlich HTTPS und aktivieren Sie die [VPN-Verbindung](https://www.uni-mannheim.de/it/anleitungen/vpn/) zur Universität.
- **Messenger Dienste:** Achten Sie bei der Wahl eines Messengers auf **Ende-zu-Ende-Verschlüsselung** und **Open-Source**-Natur des Dienstes. Für den dienstlichen Gebrauch wird deren Nutzung jedoch nicht empfohlen.

## 🔬 Grundlagen der Verschlüsselung

### Arten der Verschlüsselung

- **Symmetrische Verschlüsselung:** Es wird ein einziger Schlüssel sowohl zum Ver- als auch zum Entschlüsseln verwendet. Das Hauptproblem ist die sichere Übertragung dieses Schlüssels.
- **Asymmetrische Verschlüsselung:** Es werden zwei Schlüssel verwendet: ein **öffentlicher Schlüssel** (öffentlich zugänglich) und ein **privater Schlüssel** (geheim). Daten werden mit dem öffentlichen Schlüssel verschlüsselt und nur mit dem privaten Schlüssel entschlüsselt.

______________________________________________________________________

*Für Schulungen zu diesem Thema finden Sie hier eine [Schulungsübersicht](https://www.uni-mannheim.de/informationssicherheit/schulungen/).*
