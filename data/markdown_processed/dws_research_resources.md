---
title: "Ressourcen der Data and Web Science Gruppe: Open Data, Software und Benchmarks"
source_url_de: https://www.uni-mannheim.de/dws/research/resources/
category: Services
tags: ['Daten', 'Web Science', 'Open Source', 'Benchmarks', 'Knowledge Graph', 'Datenquellen', 'NLP', 'KI']
language: de
---

# Ressourcen der Data and Web Science Gruppe

Die Data and Web Science Gruppe stellt folgende Ressourcen für den öffentlichen Download bereit:

- Open Data
- Open Source Software
- Benchmarks

## 📚 Open Data

Dieser Abschnitt listet verschiedene Datensätze und Korpora, die für Forschungsprojekte verfügbar sind.

### Web Data Commons

Das Web Data Commons Projekt extrahiert strukturierte Daten aus dem Common Crawl Webkorpus und bietet verschiedene Datensätze zum Download:

- **Microdata, RDFa, JSON-LD und Microformat Corpus:** Extrahiert alle Microformat-, Microdata-, JSON-LD- und RDFa-Daten aus dem Common Crawl. [Projektwebsite](http://www.webdatacommons.org/structureddata/)
- **Web Table Corpora:** Extrahiert relationale Web-Tabellen aus dem Common Crawl. [Link](http://www.webdatacommons.org/webtables/)
- **WebIsA Database:** Ein öffentlich zugänglicher Datenbank mit über 400 Millionen Hypernymie-Relationen, extrahiert aus dem Common Crawl. [Link](http://webdatacommons.org/isadb/)
- **DBkWik:** Ein konsolidierter Wissensgraph, der aus Tausenden von Wikis erstellt wurde. [Link](http://dbkwik.webdatacommons.org)
- **Product Data Corpus:** Ein großer Trainingssatz und ein Goldstandard für das Product Matching, bestehend aus über 26 Millionen Produktangeboten von 79.000 Websites. [Link](http://webdatacommons.org/largescaleproductcorpus/)

### Weitere Open Data Quellen

- **DBpedia:** Ein Gemeinschaftsprojekt zur Extraktion strukturierter Informationen aus Wikipedia-Ausgaben in über 90 Sprachen und zur Bereitstellung dieser Wissensbasis im Web. [DBpedia website](https://wiki.dbpedia.org/)
- **OPIEC:** Ein Open Information Extraction (OIE) Korpus, das aus Wikipedia erstellt wurde und über 341 Millionen Triples enthält. [OPIEC website](https://www.uni-mannheim.de/dws/research/resources/opiec/)

## 💻 Open Source Software

Hier finden Sie Frameworks und Bibliotheken für Datenintegration, Ontologie-Matching und Wissensgraphen.

- **AnyBURL:** Ein Regel-Lerner (Anytime Bottom Up Rule Learning), der für den Anwendungsfall des Knowledge Base Completion konzipiert ist. [Website](http://web.informatik.uni-mannheim.de/AnyBURL/)
- **ALCOMO:** Ein Debugging-System, das inkohärente Ausrichtungen durch Auswahl eines kohärenten Teilbereichs in kohärente Ausrichtungen transformieren lässt. [Website](http://web.informatik.uni-mannheim.de/alcomo/)
- **D2RQ Plattform:** Ein System zum Zugriff auf relationale Datenbanken als virtuelle, schreibgeschützte RDF-Graphen. [D2RQ website](http://d2rq.org/)
- **DESQ:** Ein allgemeiner Zweck-System für die häufige Sequenz-Mining. Es bietet eine einfache und intuitive Muster-Ausdruckssprache. [Github page](https://github.com/uma-pi1/desq)
- **ExtractGPT:** Ein Framework zur Extraktion von Produktattributwerten mithilfe von Large Language Models (LLMs) und verschiedenen Prompting-Ansätzen. [Github page](https://github.com/wbsg-uni-mannheim/ExtractGPT)
- **LibKGE:** Eine PyTorch-basierte Bibliothek für das effiziente Training, die Evaluierung und die Hyperparameter-Optimierung von Knowledge Graph Embeddings (KGE). [Github page](https://github.com/uma-pi1/kge)
- **MatchGPT:** Ein Framework für Entity Matching unter Verwendung von LLMs und verschiedenen Prompting-Ansätzen. [Github page](https://github.com/wbsg-uni-mannheim/MatchGPT)
- **MinIE:** Ein Open Information Extraction System, das kompakte Extraktionen mit semantischen Annotationen (Polarität, Modalität, Attribution, Mengen) liefert. [GitHub page](https://github.com/uma-pi1/minie)
- **MELT:** Ein Maven-basiertes Framework zur Entwicklung, Abstimmung, Evaluierung und Verpackung von Ontologie-Matching-Systemen. [GitHub page](https://github.com/dwslab/melt)
- **PyDI (Data Integration Framework):** Ein Python-Framework für die End-to-End-Datenintegration. Es implementiert symbolische und LLM-basierte Methoden für Datenvorverarbeitung, Schema-Matching, Identitätsauflösung, Datenfusion und Ergebnisbewertung. [Github page](https://github.com/wbsg-uni-mannheim/PyDI)
- **RapidMiner Linked Open Data Extension:** Ermöglicht die Nutzung von Linked Open Data sowohl als Input für Data Mining als auch zur Anreicherung bestehender Datensätze mit Hintergrundwissen. [Project Website](https://www.uni-mannheim.de/dws/research/projects/rapidminer-linked-open-data-extension/)
- **Silk:** Ein Framework-Tool zur Entdeckung von Beziehungen zwischen Datenobjekten aus verschiedenen Linked Data Quellen. [Silk website](http://silkframework.org/)
- **WDC Extraction Framework:** Das Framework, das vom Web Data Commons Projekt zur Extraktion von Microdata, Microformats und RDFa-Daten, Webgraphen und HTML-Tabellen aus Web-Crawls verwendet wird. [Web Data Commons website](http://webdatacommons.org/framework/)
- **WInte.r Data Integration Framework:** Ein Java-Framework für die End-to-End-Datenintegration, das Methoden für Datenvorverarbeitung, Schema-Matching, Identitätsauflösung, Datenfusion und Ergebnisbewertung implementiert. [WInte.r website](https://github.com/olehmberg/winter)

## 📊 Benchmarks

Dieser Abschnitt listet standardisierte Benchmarks zur Leistungsbewertung von Systemen in verschiedenen Bereichen.

- **WDC Products: A Multi-Dimensional Entity Matching Benchmark:** Dient zur Evaluierung von Entity-Matching-Systemen anhand von drei Dimensionen: (i) Anzahl der Corner-Cases, (ii) Anzahl unbekannter Entitäten und (iii) Größe des Entwicklungsdatensatzes. [Website](https://webdatacommons.org/largescaleproductcorpus/wdc-products/)
- **SOTAB (Schema.org Table Annotation Benchmark):** Kann zum Vergleich von Column Type Annotation und Columns Property Annotation Systemen anhand eines großen Satzes von Tabellen mit heterogenen Webdaten verwendet werden. [Website](https://webdatacommons.org/structureddata/sotab/v2/)
- **WebMall – Multi-Shop Web Agent Benchmark:** Ein Benchmark zur Evaluierung von Web-Agenten in einem Multi-Shop E-Commerce-Szenario. [Website](https://wbsg-uni-mannheim.github.io/WebMall/)
- **Berlin SPARQL Benchmark (BSBM):** Definiert eine Reihe von Benchmarks zum Vergleich der Leistung von Speichersystemen, die SPARQL-Endpunkte bereitstellen. [BSBM website](http://wbsg.informatik.uni-mannheim.de/bizer/berlinsparqlbenchmark/)
- **SW4ML Benchmark:** Sammelt eine Reihe von Machine-Learning-Datensätzen mit Links zu Semantic Web Datensätzen für das Benchmarking semantischer Web-basierter Machine-Learning-Ansätze. [SW4ML website](https://www.uni-mannheim.de/dws/research/resources/sw4ml-benchmark/)
- **T2D Gold Standard for Evaluating Web Table Matching Systems:** Bietet einen reichhaltigen Satz von Korrespondenzen zwischen einem öffentlichen Web-Tabellenkorpus und der DBpedia-Wissensbasis. [T2D website](http://webdatacommons.org/webtables/goldstandard.html)
- **SV-IDENT 2022 Benchmark:** Enthält die Daten, die in der Shared Task „Survey Variable Identification in Social Science Publications“ 2022 verwendet wurden. [SV-IDENT website](https://vadis-project.github.io/sv-ident-sdp2022/)
- **Speaker Attribution Benchmark (SpkAtt-2023):** Bietet ein Korpus deutscher Parlamentsdebatten, manuell annotiert für die Sprecherzuordnung, das in der Shared Task zu Speaker Attribution in Newswire and Parliamentary Debates 2023 verwendet wurde. [SpkAtt-2023 website](https://codalab.lisn.upsaclay.fr/competitions/10431)
