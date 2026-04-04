---
title: "Datenanreicherung mit DBpedia in RapidMiner: Ein Workflow-Beispiel"
source_url_de: https://www.uni-mannheim.de/dws/research/projects/rapidminer-linked-open-data-extension/example-adding-background-information-from-dbpedia-with-multiple-generators/
category: Benutzung
tags: ['RapidMiner', 'DBpedia', 'Linked Open Data', 'Datenanreicherung', 'Workflow', 'Generatoren']
language: en
---

# Beispiel: Hintergrundinformationen aus DBpedia mit mehreren Generatoren hinzufügen

Dieses Dokument analysiert einen statistischen Datensatz zu Burnout-Raten in deutschen DAX-Unternehmen. Die Daten stammen aus einer Umfrage, deren CSV-Datei hier heruntergeladen werden kann: [women.csv](https://dws.informatik.uni-mannheim.de/fileadmin/lehrstuehle/ki/research/RapidMinerLODExtension/women.csv). Der gesamte Workflow ist auf [myExperiment](http://www.myexperiment.org/workflows/3813.html) verfügbar.

Das Beispiel demonstriert, wie mithilfe des voreingestellten DBpedia-Endpunkts Hintergrundinformationen abgerufen und kombiniert werden können, um einen Datensatz zu erweitern.

## ⚙️ Grundlegende Workflow-Architektur

Der grundlegende Workflow zur Kombination mehrerer Generatoren folgt diesen Schritten:

1. **Multiplizieren der Ausgaben:** Die Ausgaben beider Linker müssen multipliziert werden. Dies stellt sicher, dass sowohl die Datentabelle als auch die Liste der Attribute, die die Links enthalten, für verschiedene Generatoren verfügbar sind.
1. **Verknüpfen (Join):** Die Ergebnisse werden mithilfe des integrierten `Join`-Operators von RapidMiner zusammengeführt. Für diesen Join ist zwingend ein ID-Attribut erforderlich. Dieses kann entweder beim Datenimport oder mithilfe des `Set Role`-Operators (wie im Beispiel) gesetzt werden.

## 🔗 Verlinkung zu DBpedia (Pattern-Based Linker)

Um den Unternehmensdatensatz mit DBpedia zu verknüpfen, wird der **Pattern-Based Linker** verwendet. Dieser generiert URIs basierend auf einem vom Benutzer definierten Muster.

- **Funktionsweise:** Er verwendet den Wert des Feldes „Link to merge with“ und konkateniert diesen mit dem Wert des vom Benutzer spezifizierten Attributs.
- **Beispiel:** Der Attributwert „Henkel“ im Attribut „Company“ führt zum Link „http://dbpedia.org/resource/Henkel“.
- **Expertenparameter:**
  - **URL encoding:** Führt eine Kodierung von Sonderzeichen durch.
  - **Use DBpedia link format:** Führt spezielle String-Operationen für das DBpedia-Link-Format durch. Beispielsweise werden Leerzeichen durch Unterstriche ersetzt, sodass „Deutsche Telekom“ zum Link „http://dbpedia.org/resource/Deutsche_Telekom“ wird.

## 🧬 Spezifische Generatoren zur Datenanreicherung

In diesem Beispiel werden zwei spezifische Generatoren eingesetzt, um unterschiedliche Arten von Hintergrundinformationen zu extrahieren:

1. **Direct Types Generator:**

   - Dieser Generator erstellt für jeden direkten Typ ein boolesches Feature.
   - *Beispiel:* Da das Unternehmen Henkel in DBpedia den (YAGO-)Typ „ChemicalCompanies“ besitzt, wird ein Attribut für diesen Typ erstellt, das für die Instanz Henkel `true` und für andere Unternehmen `false` ist.

1. **DataProperties Generator:**

   - Dieser Generator erstellt Features für alle Daten-Eigenschaften, meist numerische Werte.
   - *Beispiel:* Dazu gehören Werte wie `netIncome`, `assets` und `numberOfEmployees`.

Die Ausgaben beider Generatoren werden anschließend mit dem `Join`-Operator zusammengeführt.

## 📊 Analyse und Ergebnisse

Aus dem zusammengeführten Output kann eine Korrelationsmatrix berechnet werden, um Attribute zu untersuchen, die mit dem anfänglichen Zielattribut (dem Frauenanteil in der Belegschaft) korrelieren.

**Beobachtete Erkenntnisse:**

- Unternehmen mit einer großen Anzahl von Mitarbeitern weisen tendenziell einen niedrigeren Frauenanteil auf.
- Unternehmen mit einem hohen operativen Einkommen zeigen einen niedrigeren Frauenanteil.
- Sportartikelhersteller weisen einen hohen Frauenanteil auf, während Kfz-Hersteller einen niedrigeren Anteil aufweisen.

Die ersten beiden Erkenntnisse basieren auf Daten des **Data Properties Generators** (numerische Fakten), während die dritte Erkenntnis Daten des **Direct Types Generators** nutzt (Klassifizierung des Unternehmenstyps).

**Zusammenfassung:** Dieses Beispiel veranschaulicht, wie Daten über Entitäten wie Unternehmen mithilfe verschiedener Generatoren gleichzeitig aus DBpedia hinzugefügt werden können.
