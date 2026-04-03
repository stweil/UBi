---
title: "Malware-Schutz und -Erkennung: Leitfaden für die Universität Mannheim"
source_url_de: N/A
source_url_en: https://www.uni-mannheim.de/en/information-security/security-tips/malware/
category: Services
tags: ['Malware', 'Virenscanner', 'Ransomware', 'Phishing', 'IT-Sicherheit', 'Datenverlust', 'Schutzmaßnahmen', 'Schadprogramme']
language: de
---

# Schadprogramme (Malware): Schutz und Verhalten bei Infektionen

Schadprogramme, allgemein als Malware bezeichnet, sind Programme, die Computer und andere Geräte infizieren, negativ verändern oder beeinflussen. Ein Befall kann sowohl Einzelpersonen als auch die gesamte Universität gefährden. Dieser Leitfaden bietet eine Übersicht über die verschiedenen Malware-Arten, Schutzmaßnahmen und das Vorgehen im Falle einer Infektion.

## 🛡️ Prävention: So schützen Sie sich vor Malware

Die beste Verteidigung ist Prävention. Achten Sie auf folgende Verhaltensregeln:

- **Software aktuell halten:** Führen Sie regelmäßig Updates für das Betriebssystem und alle Anwendungen durch.
- **Virenscanner pflegen:** Halten Sie Ihren Virenscanner stets aktuell und führen Sie regelmäßig vollständige Scans durch.
- **Netzwerkzugriff einschränken:** Deaktivieren oder beschränken Sie unnötige Netzwerkfreigaben.
- **Firewall nutzen:** Setzen Sie eine Desktop Firewall (z. B. Windows Defender Firewall) ein.
- **Rechteverwaltung:** Arbeiten Sie nicht mit Administratorrechten, wenn es nicht zwingend notwendig ist.
- **Quellenprüfung:** Installieren Sie Programme niemals aus dubiosen Quellen und verzichten Sie auf unnötige Installationen.
- **E-Mail-Vorsicht:** Seien Sie extrem vorsichtig bei Dateien und Links, die Sie per E-Mail erhalten (siehe [Spam und Phishing](https://www.uni-mannheim.de/informationssicherheit/sicherheitstipps/spam-und-phishing/#c226684)).

## 🦠 Arten von Schadprogrammen (Malware)

Es gibt verschiedene Kategorien von Schadprogrammen, die jeweils unterschiedliche Mechanismen nutzen:

- **Viren & Würmer:**
  - **Viren:** Schadprogramme, die sich verbreiten, indem sie einen "Wirt" (z. B. eine Datei) infizieren und diesen mitnehmen. Für die Verbreitung ist oft eine aktive Handlung des Nutzers nötig.
  - **Würmer:** Diese sind unabhängiger und benötigen keine fremden Dateien. Sie nutzen lediglich eine Netzwerkverbindung und eine Sicherheitslücke, um sich rasend schnell zu verbreiten.
- **Trojanisches Pferd/Trojaner:** Schadprogramme, die sich als nützliche oder harmlose Anwendung tarnen, um unbemerkt auf den Rechner zu gelangen und dort Schaden anzurichten.
- **Spyware:** Sammelt im Hintergrund heimlich persönliche Daten (z. B. Passwörter) und protokolliert die Surfgewohnheiten des Nutzers.
- **Ransomware:** Verschlüsselt die Daten auf dem Rechner oder verhindert jeglichen Zugriff und fordert dafür Lösegeld.
- **Adware:** Software, die zusätzlich zur eigentlichen Funktion Werbung anzeigt oder Suchanfragen an Werbeseiten weiterleitet.
- **Scareware:** Täuscht durch das Vortäuschen eines angeblichen Sicherheitsproblems (oft mit Pop-ups, die an Systemmeldungen erinnern) vor, um den Nutzer zu verunsichern und den Kauf einer kostenpflichtigen, unnötigen "Sicherheitssoftware" zu erzwingen.

### 🔍 Spezielle Bedrohungen

- **Keylogger:** Eine Form von Spyware, die jeden Tastendruck des Nutzers aufzeichnet.
- **Backdoorprogramm:** Ermöglicht es Angreifern, sich fernzusteuern oder den Rechner einem Botnetz hinzuzufügen.

## 🚨 Was tun bei einer Malware-Infektion? (Sofortmaßnahmen)

**⚠️ Wichtiger Hinweis:** Bei diesen Maßnahmen kann es zu **Datenverlust** kommen, und in schweren Fällen kann das System nicht mehr starten.

**1. Schritt: PC vom Netzwerk trennen!**
Ziehen Sie umgehend den **Netzwerkstecker** ab und deaktivieren Sie die **WLAN-Verbindung**. Dies verhindert, dass Ihr Gerät andere PCs im Netzwerk infiziert oder dass das Schadprogramm Daten an die Außenwelt sendet.

**2. Schritt: Schadprogramm entfernen oder IT-Support kontaktieren**

- **Selbstbehebung:** Prüfen Sie das verseuchte System mit einem **aktuellen** Virenscanner und verschieben Sie betroffene Dateien in Quarantäne.
- **Hilfe anfordern:** Wenn Sie unsicher sind, kontaktieren Sie bitte den IT-Support unter **+49 621 181-2000**.

**3. Schritt: Sicherheitsupdates installieren!**
Sobald das System bereinigt ist, verbinden Sie es wieder mit dem Internet und installieren Sie **umgehend alle verfügbaren Sicherheitsupdates** für das System und alle Programme.

**4. Schritt: Auf merkwürdiges Verhalten achten**
Überprüfen Sie das Gerät auch nach der Bereinigung regelmäßig mit einem aktuellen Virenscanner. Bei anhaltend ungewöhnlichem Verhalten kontaktieren Sie den **IT-Support**.

## 🖥️ Technische Details

### Virenscanner

Ein Antiviren-Programm ist heute Standardausrüstung und muss regelmäßig aktualisiert werden, um zuverlässigen Schutz zu bieten. Der Scanner sollte idealerweise permanent im Hintergrund laufen und idealerweise auch den Internet- und E-Mail-Verkehr überwachen.

**Achtung:**

- **Kompatibilität:** Installieren Sie **niemals** zwei oder mehr Antivirenprogramme parallel, da diese sich gegenseitig behindern können.
- **Aktualität:** Ein **veralteter Virenscanner** bietet keinen zuverlässigen Schutz.

**Woher bekomme ich einen Virenscanner?**
Als Beschäftigte der Universität Mannheim können Sie den auf Windows-Rechnern integrierten [Windows Defender](https://www.uni-mannheim.de/it/anleitungen/virenscan/) nutzen.

### 🌐 Würmer vs. Viren (Kurzvergleich)

| Merkmal | Virus | Wurm |
| :--- | :--- | :--- |
| **Verbreitung** | Benötigt einen "Wirt" (Datei) und oft aktive Nutzeraktion. | Benötigt nur eine Netzwerkverbindung und eine Sicherheitslücke. |
| **Unabhängigkeit** | Nein | Ja |
| **Beispiele** | Infizierte Dokumente, USB-Sticks. | E-Mail-Anhänge, die sich selbst versenden. |
