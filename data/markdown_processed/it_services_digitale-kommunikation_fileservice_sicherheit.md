---
title: Sicherheitsaspekte beim Zugriff auf den zentralen Fileservice
source_url_de: https://www.uni-mannheim.de/it/services/digitale-kommunikation/fileservice/sicherheit/
source_url_en: https://www.uni-mannheim.de/en/
category: Services
tags: ['Sicherheit', 'Fileservice', 'VPN', 'Datenzugriff', 'Verschlüsselung', 'Uni-ID', 'Zugriffsberechtigung']
language: de
---

# Sicherheitsaspekte beim Zugriff auf den zentralen Fileservice

Daten, die auf Netzlaufwerken abgelegt werden, sind grundsätzlich Angriffen über das Netz ausgesetzt, die trotz aller technischen Abwehrmaßnahmen nie vollständig ausgeschlossen werden können. Um das Risiko solcher Angriffe zu minimieren und gleichzeitig den Nutzern der Universität den Zugriff auf ihre Daten von außen zu ermöglichen, gelten spezifische Sicherheitsvorgaben.

## Zugriff von außen und technische Maßnahmen

Der Zugang zum zentralen Fileservice von außen ist **ausschließlich über den VPN-Client** möglich.

- **VPN-Client:** Der Einsatz des VPN-Clients gewährleistet nicht nur die Verschlüsselung des gesamten Datenverkehrs zwischen Fileservice und Clientsystem, sondern schränkt auch den Kreis potenzieller Angreifer durch die Voraussetzung einer gültigen Uni-ID und des zugehörigen Passwortes erheblich ein.
- **Zugriffsberechtigung:** Der Schutz vor unberechtigtem Zugriff auf einzelne Dateien und Verzeichnisse wird durch das zugrunde liegende Zugriffsberechtigungssystem mittels ACLs (Access-Control-Lists) bewerkstelligt. Als Voreinstellung sind die Zugriffsrechte in den HOME-Verzeichnissen so gesetzt, dass nur der/die Eigentümer/in selbst Zugriffsrechte besitzt.

## Verantwortlichkeiten und Verschlüsselung

Die Sicherheit der Daten hängt maßgeblich vom verantwortungsvollen Umgang der Nutzer ab.

### Datenklassifizierung und Verschlüsselung

- **Personenbezogene Daten:** Es ist dringend davon abzuraten, nicht verschlüsselte „Personenbezogene Daten“ auf Shares des zentralen Fileservices abzulegen.
- **Verantwortung:** Die Verschlüsselung muss von den Personen selbst erfolgen. Die Nutzer sind **juristisch für die Daten verantwortlich**.

### Allgemeine Pflichten

Alle Personen, die den zentralen Fileservice nutzen, sind verpflichtet, die Vorgaben der [Verordnungen (PDF, 28 kB)](https://www.uni-mannheim.de/media/Einrichtungen/it/Benutzerordnung_und_wichtige_Dokumente/Benutzungsordnung_Informationssysteme_Universitaet_Mannheim.pdf) einzuhalten.

## Risikobewusstsein der Nutzer

Die Sicherheit setzt auf die Sorgfalt der Nutzer voraus:

1. **Uni-ID und Passwort:** Es wird ein sorgfältiger Umgang mit der eigenen Uni-ID und dem zugehörigen Passwort vorausgesetzt.
1. **Geräteverantwortung:** Jeder Rechner, der an das Netz der Universität Mannheim angeschlossen und eingeschaltet ist, trägt das gleiche oder ein noch höheres Risiko, Opfer eines Angriffs zu werden.
