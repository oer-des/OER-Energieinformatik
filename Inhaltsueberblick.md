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

# Inhaltsüberblick zur Vorlesung Einführung in die Energieinformatik

![](img/logoblock.png)

**Lernziele:** 
Dieses Lernobjekt soll die Bedeutung der Energieinformatik als Forschungsfeld verdeutlichen. Nach der Bearbeitung dieses Lernobjektes...


- haben Sie einen Überblick über die Inhalte der Vorlesung
- haben Sie einen ersten Einblick in die Energieinformatik gewonnen
- kennen Sie das energiepolitische Zieldreieck und das Konzept Cyber-Physischer Energiesysteme
- kennen Sie einige Forschungsfragen aus dem Forschungsfeld der Energieinformatik


## Fragen in der Vorlesung
Das Leitmotiv der Vorlesung ist die Flexibilisierung von Energiesystemen. So folgt die Vorlesung im Wesentlichen den nachfolgenden Fragestellungen: 

1.	Wie sind Energiesysteme aufgebaut?

2.	Warum ist Flexibilität für die Transformation der Energiesysteme wesentlich? 

3.	Wie kann die Flexibilisierung auf der Lastseite erfolgen?

4.	Wie kann auf der Erzeugungsseite Flexibilität erschlossen werden?

5.	Welche Rolle spielen die Märkte in diesem Zusammenhang?

6.	Wie werden IT-Systeme für die Energiesysteme in Transformation entwickelt?

7.	Welchen Regelungen sind die erneuerbaren Anlagen, die wir z.B. in Virtuellen Kraftwerken gebündelt an Märkte bringen wollen, in jedem Fall unterworfen?

8.	Welche aktuellen Forschungsarbeiten befördern die zuvor genannten Entwicklungen?

9.	Worin bestehen die Herausforderungen, in diesen komplexen Zusammenhängen Hardware/Software-Systeme zu entwerfen?


Dieses Lernobjekt ist Teil einer Sammlung, die Inhalte aus dem Basiskompetenzbereich der Energieinformatik, die die wesentlichen Informationen zu den genannten Fragen zusammenfasst.

## Was ist Energieinformatik

Das folgende Video vermittelt einen ersten Überblick über die Themen der Energieinformatik:

!?[](vid/2023-07-10_Energie_Informatik_master.mp4)

Nachfolgend wird im Rahmen einer Mindmap ein möglicher Auszug über die Forschungslandschaft im Bereich der Energieinformatik dargestellt. Dieser Auszug wurde auf der Grundlage von in der Energieinformatik beheimateten Konferenzen und Fachzeitschriften erstellt (und kann daher im Prinzip jährlich aktualisiert werden!).


<iframe src="https://wp.uni-oldenburg.de/oer-fuer-die-energieinformatik-sose2023/wp-admin/admin-ajax.php?action=h5p_embed&id=6" width="100%" height="840" frameborder="0" allowfullscreen="allowfullscreen" title=""></iframe>
Abbildung 2: Exemplarischer Überblick über verschiedene Themenfelder im Bereich der Energieinformatik (eigene Darstellung). Erkennbar ist aus der Mindmap, dass die Energieinformatik von der Entwicklung von Algorithmen für die Steuerung dezentraler Anlagen, über die Berechnung von Netzzuständen, Simulationstechniken bis hin zu Fragen der Standardisierung und spezifischen Vorgehensmodellen für die Softwareentwicklung in Smart Grids sehr unterschiedlichen Bereiche mit unterschiedlichen Schnittstellen in die Informatik umfasst.

## Energiepolitisches Zieldreieck
Grundsätzlich stehen sich bei der Entwicklung von Lösungen in Energiesystemen immer unterschiedliche konfliktäre Ziele gegenüber: Während einerseits eine ökonomische Optimierung gewünscht ist (Wirtschaftlichkeit), muss für die Versorgungssicherheit gesorgt werden (und dafür die ökonomische Optimierung in Teilen eingeschränkt werden, wenn z.B. für Redundanzen zu sorgen ist). Als dritte Dimension in diesem Konstrukt von Zielkonflikten ist die Dimension der ökologischen Nachhaltigkeit (bzw. Umweltverträglichkeit in der klassischen Fassung dieses Zielkonfliktes) anzusehen. 

![Zieldreieck](img/Inhaltsueberblick/energiepolit_dreieck.png "Abbildung 2: Energiepolitisches Zieldreieck (eigene Darstellung)")

Entwickeln wir nun Lösungen für Energiesysteme, so wurde mit dem sogenannten „Energiepolitischen Zieldreieck“, das diese konfliktären Ziele beschreibt, skizziert, dass eine Positionsbestimmung erforderlich sei, da z.B. die wirtschaftlichste Lösung nicht die umweltverträglichste sei. Es ist ggf. schon offensichtlich, dass hier von einem klaren und ggf. strittigen Verständnis von Wirtschaftlichkeit (nämlich unter Nicht-Einpreisung des relevanten Ressourcenverbrauchs von z.B. Beschaffungskosten) ausgegangen wird. Nichtsdestotrotz hat sich diese Sicht des energiepolitischen Zieldreiecks zu Beginn der Entwicklung des Forschungsfeldes der Energieinformatik politisch entwickelt und langfristigen Eingang in die Sicht auf die Entwicklung von Systemen in diesem Spannungsfeld gefunden. Heute werden weiterhin deutlich feingranularere Metriken eingebracht. Insbesondere soll hier angemerkt werden, dass im Verständnis einer starken Nachhaltigkeit keine Abwägung oder Gewichtung zwischen Aspekten der Nachhaltigkeit und z.B. ökonomischen Metriken möglich ist.

Energiewirtschaftsgesetz (EnWG), §1: „Zweck des Gesetzes ist eine möglichst sichere, preisgünstige, verbraucherfreundliche, effiziente und umweltverträgliche leitungsgebundene Versorgung der Allgemeinheit mit Elektrizität und Gas, die zunehmend auf erneuerbaren Energien beruht (Quelle: Energiewirtschaftsgesetz, siehe z.B. [gesetze-im-internet](https://www.gesetze-im-internet.de/enwg_2005/__1.html)).

### Energiepolitische Ziele

**Qualitative Ziele**

- Versorgungssicherheit

- Kernenergieausstieg

- Kohleausstieg

- Bezahlbarkeit & Wettbewerbsfähigkeit

- Umweltverträglichkeit

- Netzausbau

- Sektorkopplung

- Digitalisierung

- Forschung & Innovation

- Investitionen, Wachstum & Beschäftigung


**Quantitative Ziele**

- Reduktion der Treibhausgasemissionen

- Ausbau der Erneuerbaren Energien

  - Bruttoendenergieverbrauch

  - Bruttostromverbrauch

  - Wärmeverbrauch

- Energieverbrauch & Energieeffizienz

  - Primärenergieverbrauch

  - Endenergieproduktivität

  - Bruttostromverbrauch

  - Nicht erneuerbarer Primärenergieverbrauch

  - Wärmebedarf Gebäude

  - Endenergieverbrauch Verkehr


## Cyber-Physisches System

Ein cyber-physisches System (CPS) ist ein Verbund von elektro-mechanischen Komponenten mit IT-Schnittstellen und -Funktionalitäten, die über ein Kommunikationssystem verbunden sind. Ein cyber-physisches System ist durch seinen hohen Grad an Komplexität gekennzeichnet. Die Ausbildung von cyber-physischen Systemen entsteht aus der Vernetzung eingebetteter Systeme durch Kommunikationsnetze. Die Begriffsbildung folgt dem Bedarf nach einer neuen theoretischen Grundlage für die Erforschung und Entwicklung großer, verteilter, komplexer Systeme.

Die Energieinformatik spezialisiert diesen Bedarf nach einer theoretischen Grundlage für die Erforschung und Entwicklung von Energiesystemen, die wir als CPS mit besonderen Eigenschaften verstehen können:

- Wird zu den kritischen Infrastrukturen gezählt (KRITIS)

    - Unverzichtbare Lebensader moderner Gesellschaften

- Kontinentübergreifende Größe

    - Von Nordafrika bis Skandinavien, von Irland bis Asien

- Ausbreitung von Phänomenen und deren Dynamik

    - Instantane Ausbreitungsgeschwindigkeit von Instabilitäten

- Allgegenwärtige Zielkonflikte

    - Monetäre, technische, (nationale/internationale) politische Interessen

- Im schnellen und grundlegenden Wandel begriffen...


## Forschungsfragen und Forschungsfeld

**Zentrale Forschungsfragen**

- Wie lässt sich die Digitalisierung der Energiewende sicher und sichernd gestalten?

- Wie lassen sich systemische Eigenschaften digitalisierter Energiesysteme modellieren, simulieren und testen?

- Wie lassen sich digitalisierte Energiesysteme im Spannungsfeld von Zielkonflikten und dynamischer Nebenbedingungen effizient konstruieren, betreiben und optimieren?


**Zentrale Forschungsfragen – was bedeuten sie für uns in dieser Lehrveranstaltung?**

- Welche Forschungsfragen ergeben sich aus diesem Kontext für die Energieinformatik?

    - Überblick gewinnen und Fragestellungen verstehen!

- Welches methodische Umfeld wird benötigt, um einen Beitrag für die Fragestellungen zu leisten?

    - INFORMATIK-Fragestellungen und -Methoden einordnen können!

- Welche Grundlagen aus dem Bereich der Energiesysteme sind erforderlich, um sinnvoll Fragen zu stellen und zu beantworten?

    - Grundlagen lernen und Grenzen einschätzen können!


**Energieinformatik als Forschungsfeld**

- Innovation in data-driven energy services and business models

- Big Data-driven smart Energy Management Systems

- Management of data and information flow in the Digital Energy System 4.0

- Data analytics for energy-cost efficient system operation

- Privacy issues in energy data management

- Digitalization of energy production, delivery and consumption, including policy and strategy

- Digital technologies for enabling energy-aware user behavior 

- Contextual computing for supporting human and energy system interactions

- Energy-efficient Cloud Computing and data centers

- Cyber security issues for safe and reliable Smart grid operation 

- Social media’s role in the transition towards sustainable energy

- Application of Artificial Intelligence and Agent-based technology in smart energy systems

- Model-based and data-driven energy forecasting, including energy production and use 

- Management of public and private procurement of digital energy technology

- Socioeconomic opportunities and barriers for adoption of digital energy technologies

- Sociotechnical aspects related to design and implementation of smart energy systems

- Innovation management in smart energy business eco-systems

- Digital entrepreneurship in emerging energy markets

- Smart grid communication architectures and protocols for improving grid resiliency, including graceful degradation and self-healing

- Demand-side management, including demand response, dynamic pricing and incentive design

- Microgrid and distributed generation management and control

- Monitoring and control of Smart Buildings, including Smart Grid interoperability

(Quelle: [Springer Journal Energy Informatics](https://energyinformatics.springeropen.com/about))





> Was sind die aktuellen Forschungstrends in der Energieinformatik?
>
> -	[Springer Journal für Energieinformatik](https://energyinformatics.springeropen.com/about)
>
> -	[ACM: Association of Computing Machinery – SIGEnergy (SIG: special interest group)](https://energy.acm.org/) 
>
> -	[Gesellschaft für Informatik, Fachgruppe Energieinformationssysteme](https://fg-wi-eins.gi.de/themengebiete/)


## Weiterführende Quellen im Internet zur Energieversorgung 

Nachfolgend werden einige interessante Quellen rund um das Thema Energieverbrauch und 
-erzeugung in Deutschland aufgeführt, die hier lediglich als Anregung für eine eigene Recherche aufgeführt werden sollen. 
Auf der Webseite der [AG Energiebilanzen e.V.](https://ag-energiebilanzen.de/) gibt es verschiedene aktuelle sowie historische Bilanzen, Auswertungstabellen, Energieflussbilder und weitere interessante Informationen zur Energiewirtschaft in Deutschland, sowie einen praktischen Energieeinheitenumrechner. 
Die Webseite des [Fraunhofer-Instituts für Solare Energiesysteme ISE](https://www.ise.fraunhofer.de/) stellt aktuelle sowie historische Daten und Studien zu erneuerbaren Energien und der Stromerzeugung in Deutschland sowie wegweisende Forschungsprojekte und weitere Themen rund um solare Energiesysteme vor.


## Literaturverzeichnis

https://www.gesetze-im-internet.de/enwg_2005/__1.html

https://ag-energiebilanzen.de/

https://www.ise.fraunhofer.de/

https://energy.acm.org/

https://fg-wi-eins.gi.de/themengebiete/


## Impressum

![](img/logoblock.png)

**Titel:**	Einführung in die Energieinformatik - Inhaltsüberblick

**Autor\*in:**	Prof. Dr. Astrid Nieße

**Herausgeber:**	Carl von Ossietzky Universität Oldenburg, [C3L – Center für lebenslanges Lernen](www.uol.de/c3l)

**Copyright:**	CC-BY 4.0

Dieses Werk ist lizenziert unter einer Creative Commons Namensnennung 4.0 Lizenz. Ausgenommen von dieser Lizenz sind Organisationslogos und falls gekennzeichnet einzelne Abbildungen oder sonstiges Drittmaterial sowie Bilder, auf denen Personen gezeigt werden.

**Zitierhinweis:**	Nieße, A. (2023): Einführung in die Energieinformatik - Inhaltsüberblick. Carl von Ossietzky Universität Oldenburg, abrufbar unter www.twillo.de 
