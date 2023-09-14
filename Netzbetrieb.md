<!-- 
author:   Prof. Dr. Astrid Nieße, Silke Welter, Jingyu Yang, Julia Heiken
email:    
Version:  1.0
language: de
license:  http://creativecommons.org/licenses/by/4.0/

mode:     Presentation

narrator: US English Female

logo:   img/uol_logo.png

icon:   img/uol_logo.png

        
-->

# Netzbetrieb

**Lernziele**

Nach Bearbeitung dieses Lernobjekts... 

- kennen Sie die Instrumente der Netzzustandsbeurteilung 
- kennen Sie den Aufbau und die Wichtigkeit von Lastprognosen
- können Sie die Aufgaben eines Störungsmanagements beschreiben
- kennen Sie den Unterschied zwischen Primär- und Sekundärtechnik

## Betriebsoptimierung

Zur Betriebsoptimierung gehören u.a. eine Berechnung des optimalen Lastflusses, sowie die Einsatzplanung der Kraftwerke (siehe dazu Lernobjekt „Einsatzplanung“), und ein Lastmanagement, das unter anderem Überlastungen der Betriebsmittel verhindert.

## Netzzustandsbeurteilung
Die Netzleitebene ist für verschiedene Aufgaben zuständig.

Im Rahmen der Netzzustandsbeurteilung ist sowohl eine Ausfallsimulation (n-1 von n Netzknoten) sowie eine Lastprognose von Bedeutung für die sichere Netzbetriebsführung.

### Zustandsschätzung
Ein Zustandsschätzungsalgorithmus (state estimation algorithm) ist ein Verfahren, um aus Messungen und anderen Netzinformationen den aktuellen Netzzustand zu berechnen. Dabei soll gleichzeitig der Einfluss von Messfehlern ausgeglichen und fehlende Netzgrößen berechnet bzw. abgeschätzt werden ([Heuck, 2013](#literaturverzeichnis)). Netzdaten schlechter Qualität sollen dabei eliminiert werden. State Estimation Algorithmen erlauben so eine bessere Überwachung des Netzes. Es soll also ein vollständiger und zuverlässiger Datensatz ermittelt werden. Wie und welche Eingangsdaten für die Zustandsschätzung verwendet werden, ist in Abbildung 1 dargestellt.
 
![stateestimation](img/Netzbetrieb/stateestimation.png "Abbildung 1: Übersicht zur Zustandsschätzung (eigene Darstellung)")


### Lastprognose
Um zu wissen, welche aktuelle Erzeugungslast vorhanden ist, wird eine Lastprognose durchgeführt. Das Ziel der Lastprognose ist es, einen zukünftigen Lastwert zu bestimmen und somit im Lastfolgebetrieb die Grundlage für die Kraftwerkseinsatzplanung zu schaffen. Dafür werden Zeitreihen vorangegangener Daten analysiert und die Zusammenhänge zwischen den verschiedenen Einflussgrößen modelliert. Es wird sowohl deterministisches sowie stochastisches Verhalten betrachtet. Lastwerte zeigen eine hohe Korrelation mit vorangegangenen Verläufen, sodass in Vortagesprognosen eine Genauigkeit besser als 5% erreicht werden kann ([Heuck, 2013](#literaturverzeichnis)).

Lastprognosen finden neben der Planung der Kraftwerkseinsätze sowohl in der Netzbetriebsplanung und Reservevorhaltung, wie auch in der Engpassdetektion Verwendung. Eine Vielzahl von Methoden kommt zum Einsatz und ist stets Gegenstand aktueller Forschung. Etablierte Methoden umfassen z.B. Kalman-Filter, Regressionsverfahren und Autoregressionen. 


![lastprofile](img/Netzbetrieb/lastprognose.png "Abbildung 2: Übersicht über verschiedene Standardlastprofile (eigene Darstellung basierend auf den BDEW-Standardlastprofilen)")

### Störungsmanagement
Im Rahmen des Störungsmanagement ist ein Engpassmanagement erforderlich.  In diesem Rahmen müssen Maßnahmen für den Netzwiederaufbau geplant sowie  die Reserveleistung koordiniert werden. Leitsysteme verfügen mittlerweile über eine starke Integration von IT-Systemen, die auch Daten der unterlagerten Ebenen aufnehmen und visualisieren.

### IT-Integration von Leitsystemen
Die Stationsleitebene umfasst Primär- und Sekundärtechnik. Zur Primärtechnik in elektrischen Energiesystemen gehören die Betriebsmittel, die direkt in den Transport und die Verteilung elektrischer Energie eingebunden sind. Mit dem Begriff der Sekundärtechnik umschreibt man die zur Automatisierung erforderlichen Betriebsmittel sowie die Schutzeinrichtungen (Schutz- und Leittechnik) ([Heuck, 2013](#literaturverzeichnis)).

Beide Bereiche sollen im Folgenden anhand des Beispiels eines Umspannwerkes erläutert werden: Zur Primärtechnik gehören die zur Umspannung notwendigen Transformatoren sowie alle Schaltanlagen und Kabel für den ober- und unterspannungsseitigen Anschluss. Zur Sekundärtechnik gehören nur Teile, die nicht direkt am Umspannungsprozess beteiligt sind, aber dennoch für den Betrieb unverzichtbar sind. Die Sekundärtechnik schützt beispielsweise die Betriebsmittel durch automatisches Veranlassen von Schutzmaßnahmen, z.B. bei unzulässigen Temperaturen, Spannungswerten oder Impedanzen.

Einen Überblick über den grundlegenden Aufbau der Netzbetriebsführung gibt Abbildung 3.

 
![netzführung](img/Netzbetrieb/netzfuehrung.png "Abbildung 3: Übersicht verschiedener Ebenen der Netzbetriebsführung (eigene Darstellung).")

## Anwendungsrichtlinien (AR) und technische Anschlussbedingungen (TAB)
Die [VDE-AR-N 4105](https://www.vde-verlag.de/normen/0100492/vde-ar-n-4105-anwendungsregel-2018-11.html) regelt allgemeine Anforderungen an die Integration dezentraler Anlagen. Die TAB regeln spezifische Anforderungen eines Netzbetreibers. Ein Beispiel dafür kann man bei [Enercity Netz](https://www.enercity-netz.de/) finden. 

Die AR stellt zum Beispiel Anforderungen an die Zugänglichkeit. Zudem wird eine ferngesteuerte Leistungsbegrenzung durch den Netzbetreiber und die Netztrennung, sobald die Frequenz außerhalb eines vorgegeben Rahmens fällt, gefordert. 

Die AR wurden mit dem zunehmenden Anteil von erneuerbaren Energie im Stromnetz einige Male geändert, wofür Abbildung 3 einen Überblick gibt. Im Rahmen der Spannungshaltung gibt die Richtlinie Verschiebungsfaktoren für bestimmte Anlagengrößen vor. Bei der Frequenzhaltung war früher eine Zwangsabschaltung aller EE-Anlagen bei 50,2 Hz vorgesehen. Da dies bei zunehmendem Anteil dieser Anlagen zu einem plötzlichem Wegfall großer Einspeisemengen führte, ist mittlerweile eine fP-Regelung vorgesehen, d.h. eine Frequenz-abhängige Reaktion des Wirkleistungsverhaltens.

Trotzdem sieht die Richtlinie eine Abschaltung vor, wenn die Spannung (184 V-253 V) oder die Frequenz (47,5 Hz- 51,5 Hz) aus einem zulässigen Band abweicht. Die Anlage darf sich auch nur zuschalten, wenn Spannung (195,5 V- 253 V) und Frequenz (47,5 Hz - 50,05 Hz) in einem zulässigen Band liegen. 

Der Bedarf für Netzstabilisierung ist mit den Richtlinien alleine nicht gelöst. Dies liegt unter anderem daran, dass eine Nachrüstung nur für Analgen > 10 kWp (nach erneuerbaren Energie Gesetz) vorgeschrieben ist. Im Rahmen der möglichen Lösungen entstehen neue Geschäftsmodelle. 

Hinweis: Die Regelungen in diesem Bereich unterliegen einem stetigen Wandel: Mit fortschreitender Energiewende entstehen neue Anforderungen an das Verhalten der Umrichter, an die Regelung der Wirk- und Blindleistungseinspeisung und auch bzgl. der Zu- und Abschaltgrenzen – wobei diese v.a. dem Schutz der Betriebsmittel dienen. 

 
![anwendungsrichtlinie](img/Netzbetrieb/Anwendungsrichtlinie.png "Abbildung 3: Anwendungsrichtlinie VDE-AR-N4105 Energiewende und Anpassungen über die Zeit (eigene Darstellung basierend auf Zahlen aus [statista. (17. 06 2022). Stromerzeugung aus Erneuerbaren Energien bis 2021.](https://de.statista.com/statistik/daten/studie/1807/umfrage/erneuerbare-energien-anteil-der-energiebereitstellung-seit-1991/))")

## Literaturverzeichnis
- Heuck, K. D.-D. (2013). Elektrische Energieversorgung. 9. edn. Springer.

- [VDE. (04. 05 2023). Anwendungsregeln: Erzeugungsanlagen am Niederspannungsnetz (VDE-AR-N 4105).](https://www.vde-verlag.de/normen/0100492/vde-ar-n-4105-anwendungsregel-2018-11.html)

- [statista. (17. 06 2022). Stromerzeugung aus Erneuerbaren Energien bis 2021.](https://de.statista.com/statistik/daten/studie/1807/umfrage/erneuerbare-energien-anteil-der-energiebereitstellung-seit-1991/)

- [enercity Netz. (04. 05 2023). Ergänzungen zur VDE-AR-N 4105](https://www.enercity-netz.de/)
