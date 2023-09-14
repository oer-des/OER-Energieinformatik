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

# Einsatzplanung

**Lernziele**

Nach Bearbeitung dieses Lernobjekts...

- kennen Sie die Gründe für und Verfahren der Kraftwerksplanung und Flexibilisierung der Erzeugungsseite
- sind Ihnen  die Probleme der Einsatzplanung bekannt und können Sie können sie algorithmisch einordnen. Insbesondere können Sie den Unterschied zwischen Unit Commitment und Economic Dispatch erläutern
- verstehen Sie das Konzept Virtueller Kraftwerke (VK) und können ihre Entstehung motivieren sowie den Status Quo in der Praxis darstellen.


## Netzstabilisierung
Früher wurden vor allem große thermische Kraftwerke zur Netzstabilisierung genutzt, während an die Verteilnetze nur Lasten angeschlossen waren. Daher floss damals der Strom vor allem von den Hoch- und Höchstspannungsebenen zur Verteilnetzebene. Heute und in der Zukunft gibt es weniger große thermische Kraftwerke und dafür mehr kleine und Umrichter-gekoppelte Anlagen. Auch kehrt sich der Stromfluss zu manchen Zeiten um und fließt dann aus der Verteilnetzebene in die höheren Ebenen. Der Stromfluss wird also zunehmend bidirektional. 

Zur Stabilisierung des Systems müssen auch von Kleinanlagen in den Verteilnetzen Beiträge zur Netzstabilität erbracht werden. Dies wird über die allgemein gültigen Regeln zur Integration von Anlagen im Niederspannungsnetz sowie zum Teil über die technischen Anschlussbedingungen (TAB) geregelt (siehe Lernobjekt "Netzbetrieb").

## Kraftwerkseinsatz: Economic Dispatch und Unit Commitment
Beim **Economic Dispatch** geht es um den optimalen Einsatz der N am Netz befindlichen Kraftwerksblöcke (Subproblem der Kraftwerkseinsatzplanung). Dabei sind thermische Kraftwerke durch einfachere mathematische Formulierung zu repräsentieren, z.B. durch die Multiplikatormethode von Lagrange sowie konvexe Zielfunktionen.

Beim **Unit Commitment** werden N Blöcke aus den zur Verfügung stehenden M Kraftwerksblöcken ausgewählt, sodass die Lastvorhersage optimal gedeckt werden kann. Um dieses Problem zu lösen ist eine komplexe mathematische Formulierung erforderlich, da auch Anfahrzeiten usw. zu berücksichtigen sind. Verwendete Methoden sind u.a. diskrete Optimierung und dynamische Programmierung. Dabei sollen die Fahrpläne der einzelnen Kraftwerke passend zu einem Einsatzplan kombiniert werden. Dazu findet eine Optimierung statt, die verschiedene Constraints, z.B. ökonomische und technische Aspekte berücksichtigt.
 

![unitcommitment](img/Einsatzplanung/UnitCommitment.png "Abbildung 1: Unit Commitment – aus der Kombination von Fahrplänen einzelner Kraftwerke soll ein optimaler Einsatzplan erstellt werden (eigene Darstellung)")

Unit Commitment kann als Rucksack-Problem modelliert werden. Dabei gilt es, aus einer Menge OS von möglichen Fahrplänen os (operation schedules) eine Auswahl zu treffen, sodass harte lokale Constraints eingehalten werden, lokale Präferenzen berücksichtigt werden und das globale Optimierungsziel angenähert wird. Für Lesende mit dem entsprechenden Hintergrund aus der Informatik oder Mathematik: Es handelt es sich um ein NP-vollständiges kombinatorisches Optimierungsproblem. In der Praxis wird zur Lösung daher häufig auf heuristische Ansätze zurückgegriffen. 

## Virtuelle Kraftwerke

### Entwicklung der virtuellen Kraftwerke
Markteintrittsbarrieren verhinderten eine lange Zeit die direkte Integration dezentraler Energieanlagen in die Energiemärkte. Zur Lösung dieses Problems wurde der Ansatz entwickelt, mehrere kleine Anlagen zu größeren nach dem Prinzip „Watt zu Kilo-Watt“ zu bündeln (aggregieren). In frühen Ansätzen ging es um die reine Bündelung von Erzeugungsanlagen. Dabei traten allerdings u.a. Probleme mit Prognosefehlern und der Stochastik in der Einspeisung auf. Weiterhin wurde mit fortschreitender Energiewende das Potential einer Lastanpassung, d.h. einer Flexibilisierung auch auf Lastseite, für einen fortschreitenden Paradigmenwechsel vom Lastfolgebetrieb hin zu – in Teilen – einem „Erzeugungsfolgebetrieb“ erkannt. 

In Abbildung 2 wird konzeptuell das Prinzip eines virtuellen Kraftwerks dargestellt. Neben klassischen Verbrauchern (z.B. Heizung) und Erzeugern (z.B. Windenergieanlagen), kommen auch so genannte Prosumer dazu, die sowohl Erzeuger (Producer) als auch Verbraucher (Consumer) sein können, zum Beispiel Haushalte, die eine eigene Solaranlage haben.

Nach [Bitsch, 2002](#literaturverzeichnis) stellen virtuelle Kraftwerke eine „informationstechnische Bündelung“ dezentraler Anlagen dar, und werden typischerweise über eine zentrale Instanz geführt. Insbesondere erfolgt eine gemeinsame Prognose, Einsatzplanung und Betriebsführung. Grundsätzlich wird davon ausgegangen, dass eine stärkere Diversifizierung bezüglich des Anlagenpools zu einem internen Ausgleich der Prognoseabweichungen führt.



![virtuelleKraftwerke](img/Einsatzplanung/virtuelleKraftwerke.png "Abbildung 2: Beispiel für eine Kombinationen mehrerer Erzeuger und/oder Verbraucher zu einem virtuellen Kraftwerk. Während große Kraftwerke einzeln direkt (over-the-counter, OTC) oder am Markt gehandelt werden können, werden Erzeuger und Verbraucher aggregiert, um gebündelt am Markt teilnehmen zu können (eigene Darstellung)")

Zwei grundlegende Paradigmen in der Zusammensetzung des Anlagenpools und in der Betriebsführung sind zu erkennen:

**Paradigma 1:** Man setzt virtuelle Kraftwerke so zusammen, dass sie sich bzgl. ihrer Eigenschaften nur wenig von konventionellen Kraftwerken unterscheiden. Dies erfordert eine hohe Zuverlässigkeit des aggregierten Anlagenpools bzgl. der Prognosesicherheit der gebündelten Anlagen. Virtuelle Kraftwerke diesen Typs weisen somit hohe Sicherheitspuffer bzgl. der zu liefernden Strommenge auf, die z.B. mittels Speichern vorgehalten werden müssen. Virtuelle Kraftwerke nach diesem Paradigma stellen den aktuellen Stand in der Praxis dar und erlauben eine einfache Integration in die heutigen Energiemärkte. 

**Beispiel zu Paradigma 1:** Ein Unternehmen agiert als Aggregator an Energiemärkten und hat eine Menge von Biogasanlagen über entsprechende Verträge mit den Eigentümern in sein Virtuelles Kraftwerk integriert. Die Vermarktung der Anlagen an Energiemärkten erfordert eine hohe Zuverlässigkeit. Eine hohe Prognosegüte ist für den ökonomschen Betrieb des Virtuellen Kraftwerks erforderlich.

**Paradigma 2:** Man führt das virtuelle Kraftwerk so, dass die Fluktuationen der Komponenten entweder intern durch Flexibilität kompensiert werden, oder aber die intern verfügbare Flexibilität auch bei der Lieferung des Virtuellen Kraftwerks gewünscht und dargestellt wird. Dies erfordert einen hohen Grad an Flexibilität innerhalb des aggregierten Anlagenverbundes. Erforderlich ist weiterhin aus Sicht einer Beplanung der Aggregation eine geeignete Modellierung der verfügbaren Flexibilität. Möglich ist auch eine verminderte Dauerhaftigkeit der gebildeten Aggregationen, d.h. eine dem jeweils adressierten Markt oder Produkt stärker angepasste adaptive Anlagenaggregation.

**Beispiel zu Paradigma 2:** Das in Beispiel 1 genannte Unternehmen erweitert sein Anlagenportfolio um steuerbare Lasten und elektrische Speicher, um Prognoseunsicherheiten abfedern zu können. Weiterhin werden Verträge mit den Anlagenbetreibern dynamischer gestaltet, um durch kürzere Produktlieferzeiten eine hohe Prognosegüte zu erreichen. In diesem Umfeld werden viele unterschiedliche Ansätze in der Forschung diskutiert, die teilweise auch nur für neue Märkte der Systemstabilität oder im Redispatch relevant sind.

Grundsätzlich ist festzustellen, dass mittlerweile die Konzepte Virtueller Kraftwerke und die Methoden des Demand Side Managements sowie die regionaler Märkte deutlich konvergieren und anwendungsspezifische Ausprägungen entstehen, die teilweise spezifisch Aspekte der sicheren Netzbetriebs abbilden. So wurden neben hoch dynamisierten Ansätzen bereits früh auch auktionsbasierte Verfahren vorgestellt und Ansätze unter Berücksichtigung von Netzrestriktionen und Netztopologien entwickelt. Während rein bilanzielle Virtuelle Kraftwerke Bestandteil der energiewirtschaftlichen Praxis darstellen, sind unterschiedliche Konzepte zur Umsetzung von mehr Wettbewerb im Bereich der netzdienlichen oder netzberücksichtigenden Betriebsführung dezentraler Energieanlagen noch aktueller Gegenstand der Forschung, und dienen teils auch als reduzierte Anwendungsbeispiele z.B. im Kontext spieltheoretischer Arbeiten.

Wie im Lernobjekt "Energiemärkte" unter dem Thema "Regelleistungsmärkte" dargestellt, müssen sämtliche Kraftwerke, die zur Erbringung von Primärregelleistung eingesetzt werden sollen, präqualifiziert werden. Für virtuelle Kraftwerke ergeben sich wegen der möglichen räumlichen Verteiltheit besondere Anforderungen, die in beständig aktualisierten Regularien beachtet werden.


## Literaturverzeichnis
- Beer, S. (2016). Dynamic coalition formation in electricity markets. Universität Oldenburg, Niedersachsen, Oldenburg.

- Bitsch, R. F. (2002). Virtuelle Kraftwerke - Einbindung dezentraler Energieerzeugungsanlagen Grosse virtuelle Kraftwerke im Energiemix mit Systemeinbindung. 

- Heuck, K. D.-D. (2013). Elektrische Energieversorgung. 9. edn. Springer.

- Nieße, A. S. (2015). A fully distributed continuous planning approach for. In: Informatik 2015 : Tagung Vom 28. September – 02., (S. 151–165). Cottbus.

- Russel, S. N. (2010). Artificial Intelligence. A Modern Approach. Bosten: Pearson.

- Wooldridge, M. J. (1995). Intelligent agents: theory and practice. 


