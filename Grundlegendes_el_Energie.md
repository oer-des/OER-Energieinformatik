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

# Grundlegendes zur elektrischen Energie

![](img/logoblock.png)

**Lernziele**

Nach Bearbeitung dieses Objekts...

- kennen Sie geschichtliche Entwicklungen im Zusammenhang mit elektrischer Energieversorgung
- können Sie Größen wie Arbeit, (elektrische) Energie, Leistung, Effizienz und Wirkungsgrad einordnen
- wissen Sie, was eine kWh ist
- kennen Sie den Unterschied zwischen Kabeln und Leitungen	
- verstehen Sie den Zusammenhang zwischen Wechselstrom, Wirkleistung und Blindleistung

## Ein paar erste Grundlagen
Nachfolgend werden ein paar historische Hintergründe zur elektrischen Energieversorgung vorgestellt.

### Geschichte der Glühlampe

Thomas Alva Edison

- \* 1847 Ohio	
- Verbesserung der Glühlampe
- Wirtschaftliche und technische Relevanz erkannt
- Patent
- 1882: 1. Strom- und Wärmekraftwerk nähe Wall Street 

![Edison](img/Grundlegendes_el_Energie/edison.jpg "Abbildung 1: Thomas Alva Edison, [Wellcome Collection](https://wellcomecollection.org/works/c75vbyan)")

Die Glühlampe wurde zwar nicht von Edison erfunden, aber erheblich verbessert und er war der erste, der den Bedarf an elektrischer Energieversorgung für die Verbreitung elektrischer Konsumgüter erkannte.

Das elektrische Licht wurde als Schlüsselprodukt für seine Finanzierung und die Bereitschaft der Eigentümer, Kabel zu verlegen, angesehen.

Die erste Gleichstromstation in der Pearl Street, New York, versorgte die ersten Glühbirnen und stellte eine direkte Konkurrenz zum Gasnetz dar. Thomas Alva Edison hat zahlreiche Patente auf dem Gebiet der Gleichstromtechnik. 

Kohlefaden-Glühlampen (von Edison patentiert) konnten sowohl mit Gleich- als auch mit Wechselstrom betrieben werden. In dieser Zeit der ersten Netze kam es zum sogenannten „Stromkrieg“, bei der um die bessere Eignung von Gleichstrom- oder Wechselstromsystemen für die Versorgung der Öffentlichkeit mit Strom in der Fläche gestritten wurde. Westinghouse bevorzugte Gleichstrom, während durch das Patent von Edison geschützte Glühlampen nur für die Verwendung in lizenzierten Netzen zugelassen waren und ihre Verwendung außerhalb der Netze (und damit auch in Wechselstromnetzen) sogar von den Gerichten blockiert wurde. 

Der sogenannte Stromkrieg trägt die Charakteristika eines typischen Formatkrieges – den Streit um die Macht über technische Normen und Formate, der zur Wahrung wirtschaftlicher Interessen auch über Lizenzen und Patente ausgetragen wird.


### Geschichtliche Entwicklung der elektrischen Energieversorgung 

- 1882: Erstes Gleichstromkraftwerk in der Pearl Street in New York zur Versorgung der ersten Glühbirnen
- 1891: Der erzeugte Drehstrom des 221 kW Generator in Lauffen wurde zunächst hochtransformiert und über 176 km nach Frankfurt a.M. geleitet, wo er anlässlich der Internationalen Elektrotechnischen Ausstellung über 1000 Glühbirnen und einen 74 kW E-Motor antrieb. Ein Verlust von 25% der elektrischen Energie.
- 1915: Errichtung des damals größten Braunkohle Kraftwerk mit 128 MW
- 1922: Erste deutsche 220 KV Freileitung. 	
- 1941 Erster digitaler Großrechner der Welt (Zuse Z3)	
- 1961 Erstes deutsches Versuchskernkraftwerk	
- 1986: GAU in Tschernobyl. Wendepunkt der öffentlichen Wahrnehmung und der Atompolitik	
- 1998 Liberalisierung des Strommarkts. Wendepunkt in der europäischen Energieversorgung. Ziel: Mehr Wettbewerb durch Trennung und Öffnung der „Geschäftsbereiche“	
- 2011 Nuklearkatastrophe von Fukushima und als Folge Beschluss des Atomausstiegs in Deutschland
 
 **Aufgabe:** Ordnen Sie die Ereignisse zeitlich ein (per drag and drop).

<iframe src="https://wp.uni-oldenburg.de/oer-fuer-die-energieinformatik-sose2023/wp-admin/admin-ajax.php?action=h5p_embed&id=3" width="100%" height="840" frameborder="0" allowfullscreen="allowfullscreen" title=""></iframe>


## Wichtige Größen und Begriffe

**Aufgabe:** Ziehen Sie die Begriffe in die korrekte Lücke im Text. 


<iframe src="https://wp.uni-oldenburg.de/oer-fuer-die-energieinformatik-sose2023/wp-admin/admin-ajax.php?action=h5p_embed&id=4" width="100%" height="840" frameborder="0" allowfullscreen="allowfullscreen" title=""></iframe>


### Was ist eine kWh? 

Energie wird häufig durch E (u.a. bei elektrischer Energie), W (u.a. bei mechanischer Energie) oder durch Q (Wärme) gekennzeichnet. 

Die typische Maßeinheit für Energie ist das Joule (J). Elektrische Energie wird häufig auch in Kilowattstunden (kWh) angegeben:

1 kWh = 3600 kJ 

Aus historischen Gründen ist es in der Energieversorgung auch üblich Energie in Megatonnen Öleinheiten (MTÖE) oder in Steinkohleeinheiten (SKE) anzugeben: 

1 SKE = 8, 14 kWh

**Quiz:** Was entspricht einer kWh?

<iframe src="https://wp.uni-oldenburg.de/oer-fuer-die-energieinformatik-sose2023/wp-admin/admin-ajax.php?action=h5p_embed&id=5" width="100%" height="840" frameborder="0" allowfullscreen="allowfullscreen" title=""></iframe>

### Leistung und elektrische Energie 

Die Leistung P ist die pro Zeit aufgebrachte Energie:

$$ P(t) = \frac{\delta W(t)}{\delta t} $$

$$ W(t) = \int P(t) dt $$
	 
Die Leistung wird in Watt (W) gemessen. Beim elektrischen Strom berechnet sich die Leistung wie folgt (Gleichstrom): 

$$ P = U ∗ I $$

Dabei bezeichnet U die Spannung in Volt (V) und I den Strom in Ampere (A).

> Mehr Details zu elektrischer Arbeit und Leistung:
>
> [LEIFIphysik](https://www.leifiphysik.de/elektrizitaetslehre/elektrische-arbeit-und-leistung/grundwissen/elektrische-arbeit-und-leistung)

### Effizienz und Wirkungsgrad
Der 2. Hauptsatz der Thermodynamik sagt:

> In einem geschlossenen adiabaten System kann die Entropie nicht geringer werden.

Energie kann nicht vernichtet, sondern nur umgewandelt werden. Es wird daher zwischen nutzbarer Energie und Verlustenergie unterschieden, die in ihrer Summe der eingesetzten Energie entsprechen. Der Wirkungsgrad ergibt sich als Quotient von nutzbarer Energie und eingesetzter Energie: 

$$ \eta = \frac{E_{nutz}}{E_{ein}} $$

Wobei $E_{nutz}$ die nutzbare Energie und $E_{ein}$ die eingesetzte Energie ist.

### Kabel vs. Leitungen

Unter **Kabel** werden meistens die erdverlegten Leitungen verstanden, während Freileitungen allgemein als **Leitungen** bezeichnet werden.

## Wechselstrom

Unsere Stromversorgung basiert auf Wechselstrom. Beim Wechselstrom weisen sowohl Spannung als auch Strom einen sinusförmigen Verlauf auf. In den meisten Ländern liegt die Netzfrequenz bei 50 Hz.

Bereits an dem Beispiel in Abbildung 3 kann man sehen, dass die Verläufe zwischen Strom und Spannung um den Phasenwinkel φ verschoben sind. Zur Darstellung von Wechselstrom wird allerdings häufig die komplexe Zeigerdarstellung verwendet.

![Wechselstrom](img/Grundlegendes_el_Energie/wechselstrom.png "Abbildung 3: Mögliche Zeitverläufe für Strom und Spannung (eigene Darstellung). Gezeigt ist die Scheinleistung S sowie der resultierende mittlere Wert der Momentanleistung.")

### Komplexe Zeigerdarstellung

Jeder Zeiger repräsentiert die Amplitude und Phasenlage bei einer festen Frequenz. Ein Zeiger kann Strom, Spannung oder auch Leistung repräsentieren. Für die vereinfachte Darstellung muss die Schwingung monofrequent sein. Die Schwingung wird in die Kreisdarstellung mit einer imaginären und einer reellen Achse übertragen, wie es auch in Abbildung 4 zu sehen ist. Auf diese Weise kann der Phasenverlauf als komplexwertige Darstellung verlustfrei beschrieben werden.

![Zeigerstellung](img/Grundlegendes_el_Energie/zeigerdarstellung.png "Abbildung 4: Funktionsweise der Zeigerdarstellung (eigene Darstellung)")

Die komplexen Zeiger besitzen nun analog zu Vektoren einen Betrag und eine Richtung. Sie können daher graphisch addiert und subtrahiert werden. Im Gegensatz zu Vektoren ist es allerdings auch möglich sie durcheinander zu dividieren. Die Zeiger lassen sich durch Addition translatorisch verschieben und drehen sich in der komplexen Ebene entgegen dem Uhrzeigersinn mathematisch positiv. Die Zeiger können einander entsprechend ihrer Phasenlage vor- und nacheilen. Die komplexen Werte werden häufig mit einem Unterstrich notiert. (z.B. $ \underline{U}, \underline{I}$). 

Zwischen Strom und Spannung in einem Zweig wird häufig auch der Phasenwinkel φ betrachtet. Bei induktiven Elementen (z.B. Spulen) eilt die Spannung dem Strom voraus, der Phasenwinkel ist positiv. Bei kapazitiven Elementen (z.B. Kondensatoren) eilt die Spannung dem Strom nach und der Winkel ist negativ. Beides ist auch in Abbildung 5 gezeigt. Man beachte den mathematisch positiven Drehsinn, d.h. Vorauseilen gegen den Uhrzeigersinn.

![Zeigerrichtung](img/Grundlegendes_el_Energie/zeigerrichtung_Sebastian_Lehnhoff.png "Abbildung 5: Darstellung von dem Phasenwinkel φ zwischen Strom und Spannung (Darstellung: S. Lehnhoff)")


### Leistung

Aus der Multiplikation von Spannung und konjugiert komplexem Strom ergibt sich nun eine Leistung, die als Scheinleistung (S) bezeichnet wird und deren Einheit VA (Voltampere) ist: 

$$ \underline{S} = \underline{U} * \underline{I^{*}} $$

Betrachtet man nun einen normalen Widerstand, so sind dort Strom und Spannung in Phase, sprich der Phasenwinkel ist 0◦ . An diesem Widerstand tritt reine **Wirkleistung (P)** auf. Das Verhalten ist wie im Gleichstromfall. Damit ist der Realteil der Scheinleistung die Wirkleistung, die wie die Leistung im Gleichstromfall die Einheit W (Watt) hat. 

An Kapazitäten und Spulen stehen Strom und Spannung orthogonal zueinander und es tritt nur **Blindleistung (Q)** auf, die je nach Element und Winkel kapazitiv oder induktiv ist. Die Blindleistung wird in der Einheit var (Voltampere reaktiv) angegeben, ist orthogonal zur Wirkleistung und entspricht dem Imaginärteil der Scheinleistung.

Der Betrag der Scheinleistung setzt sich nun aus einem Wirkleistungsanteil und einem Blindleistungsanteil zusammen. Es gilt der folgende Zusammenhang:

$$ S^2 = P^2 + Q^2 $$

Der Phasenwinkel φ zwischen Spannung und Strom lässt sich auch zwischen P und S wiederfinden, woraus sich die folgenden Beziehungen ergeben:

$$ S = \frac{P}{cos(\varphi)} $$

$$ P = S * cos(\varphi) $$

cos(φ) wird auch als **Verschiebungsfaktor** bezeichnet.

### Blindleistung und Wirkleistung aus technischer Perspektive
Im vorherigen Abschnitt wurde die Blindleistung Q als der Imaginärteil der komplexen Scheinleistung S eingeführt. Aber was bedeutet das auf technischer Ebene? Hilfreich für das Verständnis ist erneut Abbildung 1: 

Links zu sehen sind Spannung und Strom in Phase. Entsprechend ist die resultierende Leistung grundsätzlich positiv - es gibt einen gerichteten Leistungsfluss im System, bspw. von Kraftwerk zum Verbraucher. Das ist reine Wirkleistung (S = P). Rechts sehen wir einen Phasenwinkel von 90° und somit reine Blindleistung (S = Q). Durch die Phasenverschiebung ergibt sich kein gerichteter Leistungsfluss, sondern eine sinusförmige Schwingung. Blindleistung ist also Leistung, die im System oszilliert! Deswegen gilt Blindleistung als nicht nutzbar. Die Oszillation ergibt sich aus kleinen Energiespeichern im System (Kapazitäten und Induktivitäten), die mit einer Frequenz von 50 Hz immer wieder ge- und entladen werden. Trotzdem hat Blindleistung Auswirkungen auf das System, bspw. durch Erhöhen oder Absenken des lokalen Spannungsniveaus. Weiterhin belastet der zusätzliche schwingende Leistungsfluss die Leitungen im System, sodass der maximal mögliche Wirkleistungsfluss über die Leitung reduziert ist. 

Im Gegensatz zu unserem vereinfachten Beispiel treten Wirk- und Blindleistung üblicherweise gemeinsam auf und überlagern sich. Entsprechend ist das richtige Management der Blindleistungsflüsse im System eine wichtige Aufgabe der Netzbetreiber.

> **Mehr Wissen über Wirk- und Blindleistung**
>
> **Zum Nachlesen:** K. Heuck, K.-D. Dettmann, S. Schulz: Elektrische Energieversorgung (Erzeugung, Übertragung und Verteilung elektrischer Energie für Studium und Praxis), Springer Vieweg, 9. Auflage, 2013
>
> **Einfacher Einstieg zu Blindleistung:** [Übersicht zu Blindleistung](https://www.sma.de/partner/expertenwissen/sma-verschiebt-die-phase.html)
>
> **Gründlich**: Hofmann, Lutz: Elektrische Energieversorgung Band 1 & 2. Berlin, De Gruyter Oldenbourg, 2019, [DOI Band 1](https://doi.org/10.1515/9783110548532) \| [DOI Band 2](https://doi.org/10.1515/9783110548600)



## Literaturverzeichnis

[Wellcome collection. (25. 04 2023)](https://wellcomecollection.org/works/c75vbyan)

 Hofmann, Lutz: Elektrische Energieversorgung Band 1 & 2. Berlin, De Gruyter Oldenbourg, 2019, [DOI Band 1](https://doi.org/10.1515/9783110548532) \| [DOI Band 2](https://doi.org/10.1515/9783110548600)

[Übersicht zu Blindleistung](https://www.sma.de/partner/expertenwissen/sma-verschiebt-die-phase.html)

K. Heuck, K.-D. Dettmann, S. Schulz: Elektrische Energieversorgung (Erzeugung, Übertragung und Verteilung elektrischer Energie für Studium und Praxis), Springer Vieweg, 9. Auflage, 2013

## Impressum

![](img/logoblock.png)

**Titel:**	Einführung in die Energieinformatik - Grundlegendes zur elektrischen Energie

**Autor\*in:**	Prof. Dr. Astrid Nieße

**Herausgeber:**	Carl von Ossietzky Universität Oldenburg, [C3L – Center für lebenslanges Lernen](www.uol.de/c3l)

**Copyright:**	CC-BY 4.0

Dieses Werk ist lizenziert unter einer Creative Commons Namensnennung 4.0 Lizenz. Ausgenommen von dieser Lizenz sind Organisationslogos und falls gekennzeichnet einzelne Abbildungen oder sonstiges Drittmaterial sowie Bilder, auf denen Personen gezeigt werden.

**Zitierhinweis:**	Nieße, A. (2023): Einführung in die Energieinformatik - Grundlegendes zur elektrischen Energie. Carl von Ossietzky Universität Oldenburg, abrufbar unter www.twillo.de 