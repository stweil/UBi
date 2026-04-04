---
title: Ergebnisse zur Aktivitätserkennung mit Wearable und Smart-Home-Sensoren
source_url_de: https://www.uni-mannheim.de/dws/research/projects/activity-recognition/results/
source_url_en: https://www.uni-mannheim.de/dws/research/projects/activity-recognition/results/
category: Projekte
tags: ['Aktivitätserkennung', 'Wearables', 'Smart Home', 'ADL', 'Sensorik', 'ML', 'Probabilistisch']
language: de
---

# Forschungsresultate zur Aktivitätserkennung

Diese Seite fasst die experimentellen Ergebnisse aus verschiedenen Forschungsprojekten zur Aktivitätserkennung (Activity Recognition) zusammen, die unter Verwendung von Sensordaten aus Smart Homes und Wearable Devices durchgeführt wurden.

## 1. POLARIS: Probabilistic and Ontological Activity Recognition in Smart-homes

Dieses Projekt beschäftigt sich mit der Erkennung alltäglicher Aktivitäten (ADLs) und nutzt probabilistische sowie ontologische Methoden.

**Experimentelle Ergebnisse:**
Die resultierenden Dateien enthalten die Testergebnisse für jeden einzelnen Patienten/Tag, dargestellt durch Präzision, Recall und F-Measure.

**Setup:**

- **MLNnc Solver:** [Ontology anzeigen](link_to_ontology)
- **WSU CASAS Dataset:**
  - MLNnc Model: [show](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/Projects/sensor/results/riboni2016unsupervised/mln/casas.mln)
- **SmartFaber Dataset:**
  - MLNnc Model: [show](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/Projects/sensor/results/riboni2016unsupervised/mln/smartfaber.mln)

## 2. Modeling and Reasoning with ProbLog: An Application in Recognizing Complex Activities

Dieses Forschungswerk kombiniert Supervised Learning mit wissensbasiertem Reasoning, um die Einschränkungen beider Ansätze bei der ADL-Erkennung zu überwinden.

**Experimentelle Ergebnisse:**
Diese Seite enthält zusätzliches Material zu der Veröffentlichung.

**Setup:**

- **ProbLog Online Editor:** [show](https://dtai.cs.kuleuven.be/problog/editor.html)

**ProbLog Modelle:**
| Modell | Beschreibung | Download |
| :--- | :--- | :--- |
| #1 | Minimal ProbLog Model (Abbildung 1) | Download |
| #2 | Final ProbLog Model (Laufendes Beispiel) | Download |

*Kooperation zwischen der [University of Milano](https://www.unimi.it/ENG/) und der [University of Mannheim](http://dws.informatik.uni-mannheim.de/)*

## 3. Hips Do Lie! A Position-Aware Mobile Fall Detection System (2018)

Ziel war die Implementierung eines selbstadaptiven, ortsabhängigen Sturzerkennungsansatzes für reale Lebenssituationen.

**Experimentelle Ergebnisse:**
Die resultierenden Dateien enthalten die individuellen (nicht aggregierten) Ergebnisse.

**Datasets:**
| Dataset | Source | Publication | Traces | Download |
| :--- | :--- | :--- | :--- | :--- |
| MMSys | Source | Publication | Traces | Download |
| UMA | Source | Publication | Traces | Download |
| MiBShar | Source | Publication (PDF) | | Download |
| SisFall | Source | Publication | | Download |

**Ergebnisse:**
| Test | Details | Link |
| :--- | :--- | :--- |
| #1 | Fall Detection | ReadMe, Table III-VI, [show](link) |
| #2 | Positioning | ReadMe, Table VII, [show](link) |
| #3 | Fullstack (FallDetection) | ReadMe, Table VIII, [show](link) |
| #4 | Fullstack (Positioning) | ReadMe, Table IX, [show](link) |
| #5 | Clustering | ReadMe, - | [show](link) |

**Zusätzliche Ergebnisse (F-measure):**
| Metrik | Tabelle | Link |
| :--- | :--- | :--- |
| #1 | F0.5, F1, und F2 | Table IV, [show](link) |
| #2 | F0.5, F1, und F2 | Table V, [show](link) |
| #3 | F0.5, F1, und F2 | Table VII, [show](link) |
| #4 | F0.5, F1, und F2 | Table VIII, [show](link) |
| #5 | F0.5, F1, und F2 | Table IX, [show](link) |

*Kooperation zwischen der [Chair of Information Systems II](https://becker.bwl.uni-mannheim.de/home) und der [Chair of Artificial Intelligence](http://dws.informatik.uni-mannheim.de/en/research/artificial-intelligence-prof-stuckenschmidt/)*

## 4. Online Personalization of Cross-Subjects based Activity Recognition Models on Wearable Devices (2017)

Dieses Projekt adressiert die Herausforderung, Modelle zu entwickeln, die für Patienten und Senioren funktionieren, die keine ausreichend großen, subjektsspezifischen Datensätze bereitstellen können.

**Experimentelle Ergebnisse:**
Die Ergebnisse enthalten Testwerte (Präzision, Recall, F-measure) für jeden einzelnen Probanden, sind aber nicht aggregiert.

**Hinweis:**
Alle Experimente wurden mit Random Forest als Klassifikator durchgeführt (Online- und Offline-Lernen).

**Vorverarbeitete Beschleunigungsdaten (Fenster):**
| Setup | Beschreibung | Download | Datenpunkte |
| :--- | :--- | :--- | :--- |
| #1 | Einzelsensor-Setup, getrennt nach Position und Proband | Download | ~120 |
| #2 | Zwei-Teile-Setup, getrennt nach Kombination und Proband | Download | ~690 |
| #3 | Drei-Teile-Setup, getrennt nach Kombination und Proband | Download | ~1600 |
| #4 | Vier-Teile-Setup, getrennt nach Kombination und Proband | Download | ~2100 |
| #5 | Fünf-Teile-Setup, getrennt nach Kombination und Proband | Download | ~1600 |
| #6 | Sechs-Teile-Setup, getrennt nach Kombination und Proband | Download | ~640 |

**Cross-Subjects Activity Recognition (Abschnitt VI, Teil A):**
| # | Szenario | Tabelle | Link |
| :--- | :--- | :--- | :--- |
| #1 - #6 | Randomy (1 bis 6 Beschleunigungssensoren, Offline) | Table II | [show](link) |
| #7 - #12 | L1O (1 bis 6 Beschleunigungssensoren, Offline) | Table II | [show](link) |
| #13 - #18 | Unser Ansatz (1 bis 6 Beschleunigungssensoren, Offline) | Table II | [show](link) |
| #19 - #20 | Subject-Specific (1 bis 2 Beschleunigungssensoren, Offline) | - | [show](link) |

**Personalisierung: Online und Aktives Lernen (Abschnitt VI, Teil B):**
| # | Szenario | Tabelle | Link |
| :--- | :--- | :--- | :--- |
| #1 - #3 | Unser Ansatz (1 Beschleunigungssensor, Online) | - | [show](link) |
| #4 - #9 | Unser Ansatz (2 Beschleunigungssensoren, Online) | Table V/VI | [show](link) |
| #10 - #11 | Subject-Specific (1 bis 2 Beschleunigungssensoren, Online) | - | [show](link) |

## 5. Position-Aware Activity Recognition with Wearable Devices (2017)

Dieses Projekt zielt auf ein robustes, tragbares Aktivitätserkennungssystem für reale Situationen ab, wobei die Körperposition des Geräts berücksichtigt wird.

**Experimentelle Ergebnisse:**
Die Ergebnisse enthalten Testwerte (F-Measure, Confusion Matrix, ...) für jeden einzelnen Probanden.

**Hinweis:**
Verweis auf detaillierte Ergebnisse zu Abschnitt 5.1–5.3.

**Subject-Specific Activity Recognition (Abschnitt 5.2):**
| Setup | Ergebnisse | Link |
| :--- | :--- | :--- |
| #1 | Single Sensor | Figure V | [show](link) |
| #2 | Zwei-Teile-Setup (alle Kombinationen) | - | [show](link) |
| #3 | Drei-Teile-Setup (alle Kombinationen) | - | [show](link) |

**Cross-Subjects Activity Recognition (Abschnitt 5.4):**
| # | Szenario | Tabelle | Link |
| :--- | :--- | :--- | :--- |
| #1 - #6 | Dynamic Activity Recognition (verschiedene Konfigurationen) | Table 10, 11 / Table 12 | [show](link) |
| #7 - #8 | Activity Recognition (2 Beschleunigungssensoren, nur Taille) | Table 12, 13 | [show](link) |
| #9 - #12 | Position Recognition (verschiedene Konfigurationen) | Table 12, 13 | [show](link) |

## 6. Self-Tracking Reloaded: Applying Process Mining to Personalized Health Care from Labeled Sensor Data (2016)

Dieses Werk nutzt Process Mining, um personalisierte Gesundheitsversorgung zu fördern, indem es detaillierte Daten aus alltäglichen Aktivitäten analysiert.

**Experimentelle Ergebnisse:**
Die Seite liefert persönliche Prozesskarten und Ergebnisse der Trace Alignment Clustering.

**Hinweis:**
Die XES-Dateien stammen von anderen Forschern.

**Persönliche Prozessmodelle (Fuzzy Model):**
| Aktivität | Beschreibung | Wert | Link |
| :--- | :--- | :--- | :--- |
| #1 | Hauptaktivität aller Nutzer an Werktagen (Frequenz) | 6.2 | show (PDF, 5 kB) |
| #2 | Hauptaktivität aller Nutzer am Wochenende (Frequenz) | 6.2 | show (PDF, 5 kB) |
| #3 | Hauptaktivität aller Nutzer an Werktagen (Dauer) | 6.2 | show (PDF, 5 kB) |
| #4 | Hauptaktivität aller Nutzer am Wochenende (Dauer) | 6.2 | show (PDF, 6 kB) |

**Prozessmodelle (XES):**
| Modell | Beschreibung | Link |
| :--- | :--- | :--- |
| #1 | Activity Log UCI Detailed (Woche) | show |
| #2 | Activity Log UCI Detailed (Wochenende) | show |
| #3 - #8 | hh102, hh104, hh110 (Woche/Wochenende) | show |

**Trace Alignment:**
| # | Beschreibung | Link |
| :--- | :--- | :--- |
| #1 | Clustered Traces, Subject 1 (basierend auf unserem Datensatz) | show |

## 7. Unsupervised Recognition of Interleaved Activities of Daily Living through Ontological and Probabilistic Reasoning

Dieses Projekt adressiert die Schwierigkeit der Datenerfassung durch den Fokus auf unüberwachtes Lernen mittels ontologischer und probabilistischer Schlussfolgerungen.

**Experimentelle Ergebnisse:**
Die Ergebnisse enthalten Testwerte für jeden einzelnen Patienten/Tag sowie sensor- und instanzbasierte Ergebnisse.

**Setup:**

- **MLNnc Solver:** [show](http://executor.informatik.uni-mannheim.de/systems/n-rockit/)
- **Ontology:** [show](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/Projects/sensor/results/riboni2016unsupervised/ont/adlont.owl)

**WSU CASAS Dataset:**
| Quelle | Modell | Link |
| :--- | :--- | :--- |
| #1 | Wahrscheinlichkeiten aus unserer Ontologie | Table II,III, [show](link) |
| #2 | Wahrscheinlichkeiten aus dem Datensatz | Table II,III, [show](link) |

**SmartFaber Dataset:**
| Quelle | Modell | Link |
| :--- | :--- | :--- |
| #1 | Wahrscheinlichkeiten aus unserer Ontologie | Table IV,V, [show](link) |
| #2 | Wahrscheinlichkeiten aus dem Datensatz | Table IV,V, [show](link) |

## 8. On-body Localization of Wearable Devices: An Investigation of Position-Aware Activity Recognition (2016)

Dieses Projekt konzentriert sich auf die Erkennung der Körperposition des tragbaren Geräts in realen Lebenssituationen.

**Experimentelle Ergebnisse:**
Die Ergebnisse enthalten Testwerte (F-Measure, Confusion Matrix, ...) für jeden einzelnen Probanden.

**Hinweis:**
Es wurde ein 10-facher Kreuzvalidierungsansatz mit 10 Durchläufen angewendet.

**Vergleich der Klassifikatoren (Position Detection & Activity Recognition):**
Die Ergebnisse werden für verschiedene Klassifikatoren (Random Forest, Naive Bayes, ANN, Decision Tree, k-NN, SVM) nach folgenden Kategorien dargestellt:

- **Position Detection (alle Aktivitäten):** Alle Modelle zeigen Ergebnisse in **Table II**.
- **Position Detection (nur statische Aktivitäten):** Alle Modelle zeigen Ergebnisse in **Table III** (mit/ohne Gravitationsmerkmal in Table IV).
- **Activity Recognition (alle Aktivitäten):** Alle Modelle zeigen Ergebnisse in **Table VII, VIII** (für Single Classifier) und **Table IX, X** (für RF-basiert).

*(Die vollständige Tabelle der Ergebnisse für alle 6 Algorithmen ist in der Quelle enthalten und wird hier strukturell zusammengefasst.)*
