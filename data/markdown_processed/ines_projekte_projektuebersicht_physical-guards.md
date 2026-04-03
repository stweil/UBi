---
title: "Physical Guards: KI-basierte Sicherheit für Smart Homes auf physikalischer Ebene"
source_url_de: N/A
source_url_en: https://www.uni-mannheim.de/en/
category: Projekte
tags: ['Physical Layer Security', 'Smart Home', 'KI', 'IoT-Security', 'Signalparameter', 'Intrusion Detection', 'Verschlüsselung', 'Datenanalyse']
language: de
---

# Physical Guards: KI-basierte Absicherung von Smart Home Systemen

Das Projektkonzept „KI-basierte Analyse und Nutzung physikalischer Signalparameter zur Absicherung von Smart Home Systemen“ entwickelt den Ansatz der **Physical-Guards**. Dieses Forschungsprojekt trägt zum Bereich „Physical Layer Security“ bei, indem es den Stand der Technik aus IT-Security und Data Science/Machine Learning weiterentwickelt.

## Projektziel und technischer Ansatz

Die Grundlage des Forschungsansatzes ist die Ausnutzung physikalischer Parameter (z.B. Lokale Signalstärke) von drahtloser Kommunikation in Smart Homes. Ziel ist es, folgende Funktionen zu gewährleisten:

1. Erkennung von Angriffen auf die Smart-Home-Infrastruktur.
1. Sicherung der Integrität von Signalen.
1. Gewährleistung der Vertraulichkeit sicherheitskritischer Informationen.

**Vorteile des Physical-Guards-Ansatzes:**

- **Naturgesetze:** Die physikalischen Eigenschaften von Kommunikationssignalen unterliegen Naturgesetzen. Die Berücksichtigung dieser Eigenschaften durch die Security-Infrastruktur macht viele Angriffsstrategien unmöglich oder erheblich erschwert.
- **Heterogenität:** Im Gegensatz zu vielen höheren Schicht-Security-Konzepten ist dieser Ansatz nicht durch die große Heterogenität an Standards und Protokollen in Smart Homes eingeschränkt.

Das Projektkonsortium besteht aus der Universität Mannheim (Forschungsgruppen Dependable Systems Engineering und Institute for Enterprise Systems), dem industriellen Technologiepartner M2M Germany sowie osapiens. Das Kernziel ist die kooperative Innovationsforschung für Hard- und Softwareprodukte für den wachsenden Smart-Home-Security-Markt.

## Forschungsziele und Schwerpunkte

Die Forschung konzentriert sich auf Sicherheitslösungen, die auf der Analyse und gezielten Manipulation physikalischer Signaleigenschaften drahtloser Kommunikation basieren. Da alle Teilsysteme (unabhängig von Protokollen wie Bluetooth oder ZigBee) dieselben physikalischen Kommunikationsmethoden nutzen (z.B. das 2.4 GHz ISM-Band), bietet der „Physical Layer“ einen idealen Ausgangspunkt für ganzheitliche Sicherheitslösungen.

Ein Physical-Guards-System kann zusätzlich installiert werden, ohne die bestehende Smart-Home-Infrastruktur zu verändern. Das System besteht aus einer zentralen Steuereinheit („Center“) und einem oder mehreren Geräten („Guard“), die Überwachung und Signalsendung übernehmen.

Die Forschung gliedert sich in drei Hauptschwerpunkte:

### 1. Physical Intrusion Detection (PID)

Dieser Schwerpunkt zielt darauf ab, IT-Sicherheitsrelevante Vorfälle zu erkennen und Angriffe abzuwehren. Physical Guards nutzt dabei, dass selbst ein Angreifer physikalische Spuren hinterlassen kann, die ihn verraten.

- **Forschung:** Entwicklung eines KI-basierten Klassifikators auf Basis von Methoden zu maschinellem Online-Learning, unter Nutzung von Data Science (Outlier-Detection) und IT-Security-Forschung.
- **Herausforderung:** Weiterentwicklung von Intrusion-Detection-Verfahren hinsichtlich der Verarbeitung physikalischer Signalparameter (Einsatz von Dynamic Data Streams, Knowledge Injection, Data Distillation).

### 2. Physical Integrity and Availability Enforcement (PIAE)

Hier sollen Mechanismen erforscht werden, um das drahtlose Kommunikationsmedium vor Manipulation oder Blockierung (Jamming) durch externe Angreifer zu schützen.

- **Ansatz:** Untersuchung von sogenannten Jamming Resistant Bits, die den physikalischen Beginn einer Nachricht nutzen, um Manipulationen zu verhindern.
- **Herausforderung:** Entwicklung eines passenden Angreifermodells und die Abwägung zwischen Sicherheit und Praktikabilität.

### 3. Physical Confidentiality Protection (PCP)

Dieser Bereich adressiert die Vertraulichkeit der Daten, die in Smart Homes gesammelt werden. Da kostengünstige Geräte oft keine ausreichende Verschlüsselung bieten, schützt die Physical-Guard-Architektur die Kommunikation, ohne auf die Geräte zugreifen zu müssen.

- **Prinzip:** Die grundlegende Idee ist die Überlagerung der Nachrichtensignale mit gewählten Störsignalen. Diese Störsignale können am Empfänger wieder annulliert werden, sodass Abhörer nur die überlagerten Signale erfassen, aber nicht die ursprünglichen Nachrichtensignale bestimmen können.
- **Herausforderung:** Die Sicherheitsanalyse und Realisierung der Störsignale, sodass die Nachrichten ausreichend geschützt sind, ohne andere Kommunikation ungewollt zu stören.

## Projektpartner

### M2M Germany GmbH

M2M ist spezialisiert auf die Entwicklung, Produktion und den Vertrieb von IoT-basierten Technologieneuheiten. Im Rahmen des Projekts ist M2M verantwortlich für:

- Die Entwicklung des **Multi-Radio-Gateways** (als „Center“ bezeichnet), das die KI-basierte Überwachung sicherheitsrelevanter Ereignisse auf der physikalischen Ebene ermöglicht.
- Die Planung der **Multi-Radio-Knoten** (als „Guards“ bezeichnet) zur aktiven Absicherung der Funkkommunikation.
  Das Unternehmen verfügt über erfahrene Hard-, Firm- und Software-Entwicklungsingenieure.

### osapiens Services GmbH

osapiens bringt Expertise aus dem Bereich der KI-Entwicklung und Datenverarbeitung ein. Ein Schwerpunkt liegt auf der Bereitstellung einer Standard-Plattform mit Fokus auf Massendatenverarbeitung und Learning-Prozessen.

- **Beitrag:** Die projektspezifische KI-Plattform-Entwicklung, die die dynamische Einbeziehung von Attributen in neuronale Netze zur Anomalieerkennung sowie einen Dienst zur Validierung von Sensordaten im Zeitverlauf beinhaltet.
- **Basis:** Nutzung der Erfahrungen aus früheren FuE-Arbeiten im Bereich der KI-Forschung.
