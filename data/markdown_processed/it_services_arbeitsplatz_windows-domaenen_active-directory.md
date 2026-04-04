---
title: Active Directory Verzeichnisdienst an der Universität Mannheim
source_url_de: None
source_url_en: https://www.uni-mannheim.de/en/
category: Services
tags: ['Active Directory', 'Verzeichnisdienst', 'Benutzergruppen', 'Zugriffsrechte', 'IT-Support', 'Domäne', 'Organisationseinheiten']
language: de
---

# Active Directory Verzeichnisdienst

Das Active Directory ist der zentrale Verzeichnisdienst von Windows. In diesem Verzeichnis werden Informationen über die gesamte Organisationsstruktur einer Domäne sowie über deren Mitglieder (Organisationseinheiten, Computer, Benutzerkonten etc.) gespeichert.

## Struktur und Aufbau

Die Struktur des Active Directory ist hierarchisch aufgebaut:

1. **Grobstruktur:** Auf der obersten Ebene sind die Organisationseinheiten (Fakultäten und universitäre Einrichtungen) definiert.
1. **Unterstruktur:** Unter diesen Haupteinheiten finden sich weitere, untergeordnete Organisationseinheiten (z.B. Lehrstühle).
1. **Elemente:** Die untersten Ebenen enthalten die eigentlichen Elemente wie **Benutzergruppen** und einzelne Benutzerkonten.

Im Active Directory werden alle Informationen gespeichert, die für die Nutzung einer Benutzerkennung erforderlich sind. Neben allgemeinen Daten wie Name und E-Mail-Adresse sind dies auch technische Details zu grundlegenden Eigenschaften der Benutzerkennung und dem Ablageort der Benutzerdaten.

## Verwaltung von Benutzergruppen und Zugriffsrechten

### Gruppen vs. Einzelbenutzerkonten

Die Verwaltung von Zugriffsrechten ist besonders effizient über **Benutzergruppen** möglich.

- **Vorteil:** Wenn Zugriffsrechte an Gruppen gebunden werden, muss bei einem Personalwechsel lediglich der Mitarbeiter aus der entsprechenden Gruppe entfernt oder hinzugefügt werden. Dies ist deutlich einfacher und schneller als die Anpassung von Berechtigungen auf Basis einzelner Benutzerkonten, was bei einem Personalwechsel ansonsten an vielen Verzeichnishierarchien erfolgen müsste.

### Erstellung und Verwaltung

Gruppen können genauso definiert werden wie Benutzerkonten. Die Verwaltung von Mitgliedern ist intuitiv: Mitglieder können einfach zur Gruppe hinzugefügt oder entfernt werden.

Um eine neue Gruppe zu erstellen, wird innerhalb der gewünschten Organisationseinheit (OU) mit der rechten Maustaste geklickt und „Neu -> Gruppe“ ausgewählt. Anschließend kann der gewünschte Name in das erscheinende Dialogfeld eingegeben werden.

## Support

Bei Fragen zur Nutzung oder Verwaltung des Active Directory wenden Sie sich bitte an unseren [IT-Support](https://www.uni-mannheim.de/it/support/).
