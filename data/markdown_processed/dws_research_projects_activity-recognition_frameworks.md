---
title: Frameworks für die Aktivitätserkennung
source_url_de: https://www.uni-mannheim.de/dws/research/projects/activity-recognition/frameworks/
source_url_en: https://www.uni-mannheim.de/dws/research/projects/activity-recognition/frameworks/
category: Projekte
tags: ['Framework', 'Aktivitätserkennung', 'Sensor', 'Feature-Extraktion', 'Online-Lernen', 'RandomForest', 'Java']
language: en
---

# Frameworks für die Aktivitätserkennung

Dieses Dokument beschreibt verschiedene technische Frameworks, die im Rahmen des Projekts zur Aktivitätserkennung entwickelt wurden.

## Sensor Feature Factory

[Sensor Feature Factory](https://www.uni-mannheim.de/dws/research/projects/activity-recognition/frameworks/features/)
Dieses Framework dient zur Verarbeitung der aufgezeichneten Beschleunigungssensordaten. Es berechnet alle notwendigen Merkmale (Features), wie beispielsweise Energie oder Entropie.

**Funktionalität:**

- Unterstützt Multi-Threading.
- Ermöglicht die Spezifikation verschiedener Einstellungen, beispielsweise bezüglich der Fenstergröße (windows).
- Ist darauf ausgelegt, so schnell wie möglich zu arbeiten und kann auch auf Android-Geräten ausgeführt werden.

## Online Random Forest Classifier

[Online Random Forest Classifier](https://www.uni-mannheim.de/dws/research/projects/activity-recognition/frameworks/onlineforest/)
Dies ist eine Java-Implementierung eines Online Random Forest Classifiers.

**Funktionalität:**

- **Online Machine Learning:** Ermöglicht die kontinuierliche Aktualisierung eines bestehenden Klassifikationsmodells, ohne dass die verarbeiteten Daten gespeichert oder alle Daten *a priori* bekannt sein müssen.
- Unterstützt Threading.
- Voraussetzung ist Java 1.7 (kompatibel mit Android).
