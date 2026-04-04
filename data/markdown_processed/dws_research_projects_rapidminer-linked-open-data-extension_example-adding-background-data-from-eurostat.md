---
title: "Datenanreicherung mit Linked Open Data: Ein Beispiel mit RapidMiner und Eurostat"
source_url_de: https://www.uni-mannheim.de/dws/research/projects/rapidminer-linked-open-data-extension/example-adding-background-data-from-eurostat/
category: Services
tags: ['RapidMiner', 'Linked Open Data', 'Eurostat', 'Datenanalyse', 'Datenanreicherung', 'SPARQL', 'Entscheidungsbaum', 'Daten-Mining']
language: de
---

# Datenanreicherung mit Linked Open Data: Ein Beispiel mit RapidMiner und Eurostat

Dieses Dokument demonstriert, wie ein bestehendes Dataset mithilfe von Hintergrunddaten aus einer Linked Open Data Quelle angereichert werden kann. Als Beispiel wird hierfür Eurostat verwendet. Der entsprechende RapidMiner Workflow kann über myExperiment heruntergeladen werden.

**Input-Daten:**
Die ursprüngliche CSV-Datei, die die Daten enthält, ist unter [diesem Link](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/Web_Data_Mining/RapidMiner/alcohol-eu.csv) verfügbar.

**Hintergrundinformationen:**
Das ursprüngliche Dataset stammt von der [OECD](http://www.oecd-ilibrary.org/sites/9789264183896-en/02/06/index.html?contentType=/ns/StatisticalPublication,/ns/Chapter&itemId=/content/chapter/9789264183896-25-en&containerItemId=/content/serial/23056088&accessItemIds=&mimeType=text/html) und listet Länder sowie den Alkoholkonsum bei Erwachsenen auf. Ziel ist es, dieses Dataset zu erweitern, um mögliche Gründe für hohen Alkoholkonsum zu identifizieren und ein erklärendes Modell zu erstellen.

**Voraussetzung:**
Es wird angenommen, dass der Workflow durch die Konfiguration des SPARQL Endpunkts für Eurostat vorbereitet wurde, wie in [diesem Beispiel](https://www.uni-mannheim.de/dws/research/projects/rapidminer-linked-open-data-extension/example-reading-and-analyzing-data-from-eurostat/) beschrieben.

## Der Analyseprozess in RapidMiner

Der Prozess lässt sich in mehrere aufeinander aufbauende Schritte unterteilen:

### 1. Initialdaten und Verknüpfung (Linking)

Das ursprüngliche Input-Dataset enthält eine Tabelle mit Ländernamen und einem numerischen Wert für den Alkoholkonsum.

- **Label-based Linker:** Dieser Operator sucht nach Entitäten, deren Labels identisch mit einem der Ländernamen sind.
- **WebValidator:** Dieser Operator wird verwendet, um Instanzen zu entfernen, die in Eurostat nicht gefunden werden.
- **Ergebnis:** Die resultierende Tabelle enthält nun einen Link zu den entsprechenden Ländern in Eurostat.

### 2. Datenanreicherung (Property Generation)

Im nächsten Schritt liest der `DataPropertyGenerator` alle Daten-Eigenschaften (z.B. BIP, Bevölkerung, ...) aus den zuvor identifizierten Entitäten im Eurostat-Dataset.

- **Ergebnis:** Es entsteht eine erweiterte Datentabelle, die durch viele neue Attribute angereichert ist.

### 3. Modellbildung (Decision Tree)

Um ein Modell für die Zielvariable – den Alkoholkonsum – zu erstellen, wird ein Entscheidungsbaum trainiert.

- **Preprocessing:** Bevor der Entscheidungsbaum-Learner angewendet wird, müssen zwei Schritte durchgeführt werden:
  1. **Fehlende Werte ersetzen:** Da nicht alle Daten-Eigenschaften für alle Länder vorhanden sind, müssen fehlende Werte behandelt werden.
  1. **Diskretisierung:** Die Daten müssen diskretisiert werden, da der Entscheidungsbaum-Lernoperator keine numerischen Daten verarbeiten kann.
- **Ergebnis:** Der resultierende Entscheidungsbaum zeigt, dass der Alkoholkonsum in kleineren Ländern höher ist als in größeren, und dass der Konsum in Ländern mit starkem Bevölkerungswachstum niedriger ist.

## Zusammenfassung

Die RapidMiner Linked Open Data Extension ermöglicht es, Hintergrundinformationen zu einem gegebenen Dataset hinzuzufügen und erlaubt so eine tiefere Analyse sowohl mit den ursprünglichen als auch mit den hinzugefügten Hintergrunddaten.
