---
title: Anleitung zur Einrichtung eines persönlichen Spam-Filters an der Universität Mannheim
source_url_de: N/A
source_url_en: https://www.uni-mannheim.de/en/information-security/information-material/instructions-spam-filter/
category: Benutzung
tags: ['Spam-Filter', 'E-Mail-Sicherheit', 'Informationssicherheit', 'Schlagwörter', 'Uni Mannheim', 'E-Mail', 'Richtlinien']
language: de
---

# Persönlicher Spam-Filter für E-Mails

Generell werden alle E-Mails der Universität Mannheim auf Viren geprüft. Da Spam jedoch immer wieder so gut getarnt ist, dass er die automatische Prüfung umgehen kann, empfiehlt das Team der Informationssicherheit dringend, einen **persönlichen Spam-Filter** einzurichten.

Für eine detaillierte Anleitung zur Erstellung Ihres Spamfilters für Ihre E-Mails finden Sie hier: [Anleitung Spamfilter](https://www.uni-mannheim.de/it/anleitungen/microsoft-exchange/spam-wortfilter/)

## Tipps zur Definition von Schlagwörtern

Um einen wirksamen Spamfilter zu erstellen, ist die Wahl der Schlagwörter entscheidend.

**Beispiel: Spam-Mails zum Thema „Höhle der Löwen“**

Um zu demonstrieren, wie man Schlagwörter wählt, betrachten wir das Beispiel des „Höhle der Löwen“-Spams:

- **Beispiel-Betreff 1:** „Löwen“ System macht Deutsche Bürger reich!
- **Beispiel-Betreff 2:** ?Höhle der Löwen? System macht Deutsche Bürger reich!

**Empfehlung:** Filtern Sie nach der Wortfolge: `macht Deutsche Bürger reich`, da beide Betreffzeilen diese spezifische Kombination enthalten.

### Was Sie vermeiden sollten: Suche nach einzelnen Wörtern

Das Anwenden von zu allgemeinen Schlagwörtern (z. B. „Hallo“) führt dazu, dass der Spam-Filter alle E-Mails nach diesem Wort durchsucht. Dies ist zu restriktiv, da dadurch auch legitime E-Mails im Spam-Ordner landen könnten, die Sie benötigen.

**Besser:** Wählen Sie immer ein **Textmuster** oder eine spezifische Wortfolge, wie zum Beispiel:

- `Hallo, Sie haben gewonnen`
- `Sie haben gewonnen`
