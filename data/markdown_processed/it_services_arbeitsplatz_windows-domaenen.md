---
title: Windows Domänen-Verwaltung an der Universität Mannheim
source_url_de: https://www.uni-mannheim.de/it/services/arbeitsplatz/windows-domaenen/
source_url_en: https://www.uni-mannheim.de/en/it/services/workplace/windows-domains/
category: Services
tags: ['Windows', 'Domäne', 'IT-Infrastruktur', 'Benutzerverwaltung', 'Active Directory', 'Arbeitsplatz', 'Uni-ID']
language: de
---

# Windows Domänen an der Universität Mannheim

Die Universitäts-IT betreibt eine zentrale Windows Domäne für die Universität unter der Adresse `ad.uni-mannheim.de`. Diese Domäne wird über die Seite [MyUni-ID](https://id.uni-mannheim.de/login.php?ref=index.php) der Universitäts-IT synchronisiert.

Mit der Windows-Domäne werden alle Aufgaben, die mit der Verwaltung von Uni-IDs verbunden sind, zentralisiert und automatisch abgewickelt. Die Nutzung der Domäne ist besonders vorteilhaft, wenn:

- **Viele Arbeitsplätze:** Eine große Anzahl von Rechnern von unterschiedlichen Personen genutzt wird, da die Uni-IDs nicht für jeden einzelnen Rechner manuell eingetragen werden müssen.
- **Einheitliche Verwaltung:** Einrichtungen eine zentrale und automatisierte Benutzerverwaltung für mehrere Rechner betreiben möchten.
- **Zentrale Ressourcen:** Rechner auf zentralen Ressourcen wie dem zentralen File-Service zugreifen müssen.
- **Gruppenberechtigungen:** Die Organisation eines Rechnerverbundes (z.B. an einem Lehrstuhl) erleichtert die Verwaltung von Nutzungsberechtigungen für private oder zentrale DV-Ressourcen mittels Gruppenberechtigungen im Active Directory (dem Verzeichnis-Dienst von Windows).

Bei der Integration einer größeren Anzahl von Arbeitsplätzen in die Domäne ist die Einrichtung einer Organisations-Einheit (OU) ratsam, was eine umfassende Planung erfordert.

## Hinweise zur Mitgliedschaft in der Domäne

### Abhängigkeiten und Betriebssicherheit

Die Mitgliedschaft in der Domäne führt zu einer zwangsläufigen Abhängigkeit von funktionierenden Domaincontrollern. Da die Authentifizierung der Accounts nicht mehr lokal, sondern an der Domäne erfolgt, sind rund um die Uhr verfügbare Domaincontroller für den Betrieb kritisch.

Um negative Auswirkungen dieser Abhängigkeit zu minimieren, wurde die technische Infrastruktur für die Domaincontroller so redundant wie möglich ausgelegt. Dennoch ist an jedem Arbeitsplatz weiterhin eine lokale Anmeldung möglich, wodurch die negativen Konsequenzen eines Totalausfalls der Domäne begrenzt sind.

### Domänen-Administration und Rechte

Eine Domäne dient der zentralen Organisation eines ausgedehnten Rechnerverbundes und zeichnet sich durch eine einheitliche Benutzerverwaltung aus.

**Administrative Rechte:**

- Standardmäßig besitzen Domänen-Admins (nach Windows-Voreinstellung) auf allen Mitgliedsrechnern administrative Rechte.
- Ein lokaler Administrator kann diese Rechte entziehen und den Rechner somit gegen externe Einflüsse sperren. Grundsätzlich behält der Domänen-Admin jedoch die Möglichkeit, solche Sperren wieder aufzuheben.

**Richtlinien der Universität Mannheim:**
In der Praxis wird von den weitreichenden Rechten des Domänen-Admins an der Universität Mannheim kein Gebrauch gemacht, da die Administration der Arbeitsplätze nicht Aufgabe der Universitäts-IT ist. Die IT beschränkt die Zugriffsmöglichkeiten des Domänen-Admins auf das technisch notwendige Minimum, um die Sicherheit zu erhöhen. Wird zur Aufnahme von Rechnern die von der Universitäts-IT bereitgestellte Skripte genutzt, werden den Domänen-Admins die administrativen Rechte automatisch entzogen.
