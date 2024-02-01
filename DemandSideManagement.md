<!--
author:   Prof. Dr. Astrid Nieße, Silke Welter, Jingyu Yang, Julia Heiken
email:  
Version:  1.0
language: de
license:  <http://creativecommons.org/licenses/by/4.0/>

mode:     Presentation

narrator: US English Female

logo:   img/uol_logo.png

icon:   img/uol_logo.png

\-->

# Demand Side Management (DSM)

![](img/logoblock.png)

**Lernziele**

Nach Bearbeitung dieses Lernobjekts...

- kennen Sie die Bedeutung der Modellierung von Lastverschiebungspotentialen und können sie anhand von  Beispielen ausführen
- können Sie die Grundprinzipien peak clipping, valley filling, load shifting unterscheiden
- können Sie die folgenden Konzepte aus dem Bereich des Demand Side Managements (DSM) erläutern und differenzieren:

  - Energieeffizienzmaßnahmen
  - Time of Use (ToU)
  - pricingMarket/Physical Demand Response

## Motivation für DSM

Konventionell erfolgte die Versorgung mit elektrischem Strom im Lastfolgebetrieb: die Erzeugung folgte der Last. Mit der erforderlichen Flexibilisierung dieser Betriebsweise, die sich aus der zunehmenden Versorgung mit stochastischen Erzeugern[^1] ergibt, werden typischerweise elektrische Batteriespeicher verbunden. Eine gewünschte Alternative zum Ausbau der Erzeugung und der Bereitstellung von Speichern ist die Anpassung von Lasten. Damit kann bei entsprechender Steuerung unter Berücksichtigung von Netzzuständen auch ein Netzausbau vermieden werden.

![](img/DemandSideManagement/Netzfrequenzwaage.png "Abbildung 1: Sind Last und Erzeugung nicht ausgeglichen, verändert sich die Netzfrequenz (eigene Darstellung).")

*Ist die Leistungsbilanz nicht ausgeglichen, verändert das die Netzfrequenz (siehe Abbildung 1). Frequenzhaltung oder -stabilität ist eine Anforderung an eine qualitativ hochwertige Versorgung mit elektrischer Energie.  Frequenzhaltung muss  gewährleistet werden – das ist technisch umgesetzt durch Frequency Containment Reserve (FCR) und automatic Frequency Restoration Reserve (aFRR),  genaue Erklärungen sind in den Lernobjekten "Komponenten" und "Koordinationsaufgaben" zu finden.*

Demand Side Management umfasst alle Maßnahmen, die zu einer Anpassung des Energiesystems auf der Seite der Lasten führen.

[^1]: d.h. die Erzeugung kann nicht genau, sondern nur anhand von Wahrscheinlichkeiten vorhergesagt werden

### Beispiele zur Anpassung von Lasten

![](img/DemandSideManagement/DSMMotivation.jpg "Abbildung 2: Beispiele für die Anpassung von Lasten (eigene Darstellung).")

In Abbildung 2 ist zu sehen, dass es verschiedene Methoden mit sehr unterschiedlichen Ansätzen gibt. Zur Kategorisierung können die im folgenden Kapitel (Typen des DSM) vorgestellten Taxonomien genutzt werden.

### Last als Freiheitsgrad = Flexibilität in Energiesystemen

Lasten sind als mögliche Freiheitsgrade bereits lange bekannt. Die Nutzung dieser Freiheitsgrade hängt wesentlich von drei Aspekten ab:

- Geeignete Modellierung der Lasten: Vorausschauende Planung der Effekte einer Lastbeeinflussung
- Eingebettete Systeme (Last-nah): Umsetzen der Signale zur Lastbeeinflussung
- Kommunikationsinfrastruktur (übergreifend): Übermittlung von Signalen zur Lastbeeinflussung

### Lastverschiebung – Modellierungsbedarf

Verschiebbare Lasten erfordern ggf. eine Modellierung eines gesamten Prozesses, beispielsweise bei den folgenden Verschiebungspotentialen:

- Inerte (träge) thermische Prozesse (Heizung und Kühlung), bei denen die Abhängigkeit der unterstützten Prozesse von definierter Temperatur wesentlich ist (Beispiele dafür sind Schmelzprozesse oder Kühlbäder),
- Massentransporte (Pumpen, Transportbänder etc.) oder logistische Prozesse, bei denen eine Optimierung von Produktionsplänen bis hin zur Pausengestaltung denkbar ist.

Eine Nutzung der Anlagenflexibilität zur Lastverschiebung hängt wesentlich von der Güte der Modellierung ab!

Die Grundprinzipien der Lastverschiebung **Peak Clipping**, **Valley Filling**, **Load Shifting** und **Load Reduction** sind in Abbildung 3 illustriert. Beim Peak Clipping (Spitzenreduktion) und Valley Filling werden jeweils besonders hohe oder niedrige Lasten verringert bzw. erhöht, damit der Unterschied zwischen den Extremwerten weniger stark ausgeprägt ist. Beim Load Shifting werden Lasten in einen günstigeren Zeitraum verschoben. Load Reduction bedeutet, dass die gesamte Last reduziert wird.

**Aufgabe:** Ordnen Sie die Begriffe den passenden Graphen zu.

<iframe src="https://wp.uni-oldenburg.de/oer-fuer-die-energieinformatik-sose2023/wp-admin/admin-ajax.php?action=h5p_embed&id=7" width="90%" height="840" frameborder="0" allowfullscreen="allowfullscreen" title=""></iframe>

## Typen des DSM

Es gibt unterschiedliche Taxonomien für DSM. Im Rahmen dieser Lernmaterialien wird die Differenzierung nach [Peter Palensky, 2011](#literaturverzeichnis) verwendet:

1. Energieeffizienz-Maßnahmen (EE)
2. Zeitabhängige Tarife (time of use, TOU)
3. Demand Response (DR)
4. Spinning Reserve (SR)

### Energieeffizienz-Maßnahmen (EE)

**Energieeffizienz – energy leaks**

Zur Steuerung der Energieeffizienz und zur Detektion von Energie-Leaks ist eine Einsicht in die entsprechenden Prozesse wesentlich. Häufige Energy-Leaks sind z.B. Druckluft-Leckagen, Filterverunreinigungen oder defekte Bauteile.

Abbildung 4 zeigt beispielsweise den Filter eines Kondenstrockners, der aufgrund eines Defektes verschmutzt ist. Dies führt im Betrieb zu einer schlechten Energieeffizienz. Im industriellen Umfeld gibt es ähnliche Beispiele.

![](img/DemandSideManagement/Leaks.png "Abbildung 4: Verschmutzter Filter eines Kondenstrockners (eigene Fotos)")

**Energieeffizienz – Detektion**

Wenn man die Basislast (baseline) mit der Spitzenlast vergleicht, kann eine hohe baseline auf schlechte Isolierung oder defekte Stand-by-Geräte hinweisen. Bei einem wöchentlichen Zeitreihenvergleich könnte beispielsweise auffallen, dass Licht oder Lüftung ggf. unnötig außerhalb der Nutzungszeiten aktiv sind. Insbesondere bei Filialisten ist ein einfacher Benchmark-Vergleich von Standorten möglich (z.B. Supermärkte). Ebenfalls kann untersucht werden, ob die Korrelation des Energieverbrauchs mit externen Größen (z.B. Temperatur) oder internen Prozessen (z.B. Anlieferung von Kühllasten) der Erwartung entspricht.

### Zeitabhängige Tarife (Time of Use, ToU)

Zeitabhängige Tarife stellen ein etabliertes Mittel zum Lastmanagement dar. Es gibt eine Doppeltarifzählung mit HT (Hoch-/Haupttarif) und NT (Nieder-/Nachttarif). Die technische Umsetzung (ohne Smart Metering) erfolgt durch zwei separate Rollenzählwerke (siehe Abbildung 5), die zu den im Stromzähler festgelegten Zeiten (eichrelevant) umspringen. Aufgrund der Beschränkung durch die Hardware  gibt es keinen natürlichen technologischen Entwicklungspfad von statischen ToU zu dynamischen Tarifen.  Dynamische Tarife werden erst mit Smart Metering möglich. HT/NT ist ein Relikt aus der Vor-Unbundlingzeit[^1] und funktioniert nur mit einer Vereinbarung zwischen Netzbetreiber und Lieferant.

Die ToU-Tarife sind in Deutschland im Zähler hinterlegt. Eine Änderung erfordert einen Tarifwechsel (vertragsrelevant) sowie eine Anpassung der Hardware. Konfigurierte Stromzähler dürfen nicht vor Ort umkonfiguriert werden!

Zeitabhängige Tarife bilden also ein statisches Modell der Lastdynamisierung mit guten Effekten bzgl. einer allgemeinen Anpassung von Standardlasten.


> **Zum Nachdenken und Vertiefen**
>
> Eine früher weit verbreitete Möglichkeit zur Nutzung der zeitabhängigen Tarife sind Nachtspeicheröfen. Dies sind Heizungen, die elektrische Energie speichern und in Form von Wärme abgeben. Sie werden aufgeladen, wenn der Strom günstig ist (im Nieder-/Nachttarif, daher der Name) und heizen anschließend tagsüber.
> Überlegen Sie:
>
> - Was ist die mögliche Motivation für Nachtspeicheröfen?
> - Wie beeinflussen Kern- oder Kohlekraftwerke diese?
> - Erklären Sie auch die hohe Durchdringung mit Nachtspeicheröfen im Ruhrgebiet.
>
> Heutzutage werden Nachtspeicheröfen aufgrund ihres schlechten Wirkungsgrades und ihrer schlechten Umweltauswirkungen nicht mehr verbaut, dürfen aber noch betrieben werden (Stand 2023).

![](img/DemandSideManagement/Zaehler.jpeg "Abbildung 5: Stromzähler mit zwei Zählwerken für HT und NT. Umsetzung z.B. HT: 7:30-20 Uhr, NT: Restzeit. (eigenes Foto).")

[^1]: Unbundling = Entflechtung der Unternehmen der Energiewirtschaft, hier insbesondere Trennung von Netzbetrieb und Lieferung von Strom

### Zeitabhängige Tarife: Spezialfälle Critical Peak Prizing (CPP) und Extreme Day Prizing (EDP)

Das **Critical Peak Pricing (CPP)** baut auf der Struktur eines ToU-Tarifs auf und erweitert ihn um eine Preisstufe für besonders "kritische" Spitzenlaststunden. Diese neue Preisstufe kann kurzfristig angekündigt werden (ca. einen Tag vorher oder am selben Tag) und ist limitiert auf ca. 50-100 Stunden pro Jahr. Die Höhe der Preisstufe und die maximale Gültigkeit sind im Vorfeld bekannt.

Ähnlich zu CPP ist der Tarif des **Extreme Day Pricing (EDP)**, allerdings mit einer Gültigkeit der neuen Preisstufe  von 24 Stunden. Dabei ist die Anzahl der "kritischen" Tage begrenzt und die Ankündigung erfolgt einen Tag vorher.

**Extreme Day CPP (ED-CPP)** ist eine Variation des CPP, allerdings gelten lediglich die (höchste) Preisstufe sowie zugehörige (niedrigste) off-peak Preise für "kritische" Stunden an bestimmten ("extremen") Tagen. An den anderen Tagen gelten keine TOU-Preise. Als "extrem" können extreme Wetterbedingungen oder Kraftwerksausfall gelten.

### Demand Response (DR)

Demand Response teilt sich auf in **Market Demand Response** und **Physical Demand Response**. Market Demand Response ist preisbasiertes dynamisches Anreizen eines veränderten Lastverhaltens, während Physical Demand Response bindende Signale zur Änderung des Lastverhaltens aus Gründen des stabilen Netzbetriebs sind (verdeutlicht in Abbildung 4).

![](img/DemandSideManagement/DemandResponse.png "Abbildung 4: Market Demand Response (links) und Physical Demand Response (rechts), eigene Darstellung.")

**Market Demand Response**
Beim preisbasierten dynamischen Anreizen eines veränderten Lastverhaltens werden dynamische Tarife eingesetzt, bei denen die Kundenpreise an die Dynamik des Systems angepasst werden. Dabei findet eine Kopplung an Energiemärkte (wie die EPEX Spot) und an Prognosen von Netzengpässen statt.

*Umsetzbarkeit dynamischer Tarife in Deutschland*

Anschlussnehmer mit einer Abnahme von weniger als 100.000 kWh/a werden nach Standardlastprofilen behandelt, d.h. es erfolgt keine zeitdifferenzierte Zählung des Verbrauchs.

Ein Auszug aus der Stromnetzzugangsverordnung [StromNZV](https://www.gesetze-im-internet.de/stromnzv/__12.html), §12:
"Soweit es für die Umsetzung eines variablen Tarifs im Sinne von § 40 Absatz 5 Satz 1 des Energiewirtschaftsgesetzes erforderlich ist, haben Netzbetreiber Netznutzern eine Bilanzierung und Abrechnung auf Basis von Zählerstandsgängen für diejenigen Einspeise- und Entnahmestellen zu ermöglichen, deren Einspeise- und Entnahmeverhalten mit intelligenten Messsystemen im Sinne des Messstellenbetriebsgesetzes ermittelt wird."

Während im industriellen Bereich Vereinbarungen schon jetzt möglich sind, werden dynamische Tarife im Privatbereich also erst mit Smart Metern möglich.

*Akzeptanz dynamischer Tarife bei Privatkunden*

Privatkund:innen lehnen dynamische Tarife, die an die Dynamik von Energiemärkten gekoppelt werden, in großen Teilen ab. Die Hauptprobleme sind die Unvorhersagbarkeit und Unberechenbarkeit von Märkten. Erst massive Einsparpotentiale führen zu erhöhtem Interesse. Kostengarantien könnten einen Weg darstellen, die Kund:innen mit dynamischen Tarifen vertraut zu machen [Schlereth18](https://doi.org/10.1016/j.ejor.2018.03.033).

In anderen Ländern ist dies bereits etabliert. In Italien gibt es beispielsweise seit 2010 ein verpflichtendes ToU und dort ist ebenfalls Smart Metering im Einsatz.

Finanzielle Anreize können auch für die Anpassung des Verhaltens für Belange des stabilen Netzbetriebs geboten werden (Market DR). Das ersetzt NICHT Methoden für die Sicherung des Netzbetriebs in kritischen Situationen! Dynamische Tarife stellen keine Lösung für das Problem der Netzstabilisierung dar, können das Problem aber ggf. verkleinern.

**Physical Demand Response**

Die Maßnahmen des Physical Demand Response stellen bindende Vorgaben zur Beeinflussung von Lasten dar. Eine Parallele dazu im Erzeugungsbereich ist das Einspeisemanagement. Dabei ist load shedding der Abwurf von Lasten und direct load control ist die Beeinflussung von Prozessen auf Kundenseite. Dabei werden beispielsweise steuerbare Kundengeräte bei Spitzenlast ein- oder abgeschaltet, um einen Beitrag zur Netzstabilisierung zu leisten.


## Quiz 

**Aufagbe:** Ordnen Sie die DSM-Typen auf der Zeitachse ein.

*Hinweis:* SR = Spinning Reserve (aus dem Bereich der Frequenzhaltung; hier nicht weiter ausgeführt)

<iframe src="https://wp.uni-oldenburg.de/oer-fuer-die-energieinformatik-sose2023/wp-admin/admin-ajax.php?action=h5p_embed&id=10" width="90%" height="840" frameborder="0" allowfullscreen="allowfullscreen" title=""></iframe>

## Literaturverzeichnis

- Peter Palensky, D. D. (03. 08 2011). Demand Side Management: Demand Response, Intelligent Energy Systems, and Smart Loads. IEEE Transactions on Industrial Informatics.
- [Schlereth, Christian; Skiera, Bernd; Schulz, Fabian (2018): Why do Consumers prefer Static instead of Dynamic Pricing Plans? An Empirical Study for a better Understanding of the Low Preferences for Time-Variant Pricing Plans. March 2018, European Journal of Operational Research](https://doi.org/10.1016/j.ejor.2018.03.033)
- [StromNZV](https://www.gesetze-im-internet.de/stromnzv/__12.html)

## Impressum

![](img/logoblock.png)

**Titel:**	Einführung in die Energieinformatik - Demand Side Management

**Autor\*in:**	Prof. Dr. Astrid Nieße

**Herausgeber:**	Carl von Ossietzky Universität Oldenburg, [C3L – Center für lebenslanges Lernen](www.uol.de/c3l)

**Copyright:**	CC-BY 4.0

Dieses Werk ist lizenziert unter einer Creative Commons Namensnennung 4.0 Lizenz. Ausgenommen von dieser Lizenz sind Organisationslogos und falls gekennzeichnet einzelne Abbildungen oder sonstiges Drittmaterial sowie Bilder, auf denen Personen gezeigt werden.

**Zitierhinweis:**	Nieße, A. (2023): Einführung in die Energieinformatik - Demand Side Management. Carl von Ossietzky Universität Oldenburg, abrufbar unter www.twillo.de 
