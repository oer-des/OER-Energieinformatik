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

# Koordinationsaufgaben

**Lernziele**

Nach Bearbeitung dieses Lernobjekts...

- wissen Sie, was Systemdienstleistungen sind
- kennen Sie die Funktionen von Frequenzhaltung und Spannungshaltung sowie deren Unterschiede
- wissen Sie, was ein Bilanzkreis ist
- verstehen Sie, warum ein Bilanzkreismanagement notwendig ist und wissen wie es aufgebaut ist

## Systemdienstleistungen (SDL)

Systemdienstleistungen (SDL) sind Aufgaben, die für die Funktionstüchtigkeit des Systems erforderlich sind. Diese werden von den Netzbetreibern zusätzlich zur Übertragung und Verteilung von elektrischer Energie erbracht.

Die SDL bestimmen die Versorgungsqualität. Dazu gehören die Betriebsführung und die Fähigkeit zum Versorgungswiederaufbau, auf die im Weiteren nicht genauer eingegangen wird.

Eine wichtige SDL ist die Frequenzhaltung, die eng mit der Regelleistung in Verbindung steht und im nächsten Abschnitt ausführlich erläutert wird. Außerdem ist die Spannungshaltung relevant, die weiter unten dargestellt wird. 


### Frequenzhaltung

Die Netzfrequenz ändert sich, wenn die Leistungsbilanz im elektrischen Netz nicht ausgeglichen ist, somit entweder mehr Strom erzeugt als verbraucht oder mehr verbraucht als erzeugt wird. Die Netzfrequenz ist ein schnell reagierender Wert. Eine feste Netzfrequenz ist für eine qualitativ hochwertige Versorgung mit elektrischer Energie sehr wichtig. Die aktuelle Netzfrequenz kann man im Internet nachverfolgen: [Netzfrequenzmessung](www.netzfrequenzmessung.de). 

![Regelbereiche](img/Koordinationsaufgaben/Regelbereiche.png "Abbildung 1: Die verschiedenen Regelbereiche (Darstellung: Sebastian Lehnhoff).")
 
Die Frequenz ist überall im europäischen Verbundnetz gleich. Eine Einspeisung/Verbrauch kann an beliebiger Stelle stattfinden.
Die Leistungsregelung teilt sich in mehrere Phasen ein (siehe Abbildung 1). In Abbildung 1 ist zu sehen, wie die Phasen der Regelung ineinander übergehen und welche Regelung bei welchem Auslöser der Frequenzabweichung greift. Frequency Containment Reserve (FCR) und automatic Frequency Restoration Reserve (aFFR) sind autonome Antworten auf Frequenzänderungen (für Details siehe Lernobjekt "Komponenten"), während die manual Frequency Restoration Reserve (mFFR) manuell durch einen jeweiligen Übertragungsnetzbetreiber (ÜNB) geregelt wird. Die zeitliche Verzögerung zu Beginn ergibt sich aus der Trägheit der reagierenden Systeme (z.B. beim Beschleunigen oder Verlangsamen eines Kraftwerksgenerators).

Die verschiedenen Arten der Regelleistung werden vom Übertragungsnetzbetreiber (ÜNB) auf dem Regelenergiemarkt ausgeschrieben. Im Lernobjekt „Energiemärkte“ werden weitere Details zu den marktlichen Aspekten ausführlicher dargestellt.


### Spannungshaltung
Aufgrund physikalischer Gesetze der Stromleitungen kann mit wachsender Distanz der Einspeise- und Verbrauchspunkte elektrischer Energie zum nächsten Transformator die Netzspannung stärker variieren. In Abbildung 2a und b wird dies veranschaulicht. Das Netz muss sich daher in jedem Punkt, an dem eingespeist (führt zu Erhöhung der Spannung) oder verbraucht (führt zu niedrigerer Spannung) wird, innerhalb des zulässigen Spannungsbandes (rote und blaue Linie) bewegen. Werden Ober- oder Untergrenzen durch zu viel Einspeisung bzw. zu hohen Verbrauch über- bzw. unterschritten (siehe Abbildung 2a ganz rechts), greift die Spannungshaltung ein, um die Spannung entsprechend wieder in den erlaubten Bereich zu bringen (siehe Abbildung 2b). Hier stehen unterschiedliche Mechanismen zur Verfügung. Als Beispiel sei die Anpassung von Verbrauch und Erzeugung sowie die Veränderung der Eingangsspannung genannt.  

Das Spannungsniveau hat weiterhin eine direkte Wechselwirkung mit der lokalen Blindleistungsbilanz. Die Netzbetreiber haben die Blindleistungsbilanz ihres Netzes auszugleichen und gleichzeitig zulässige Spannungsbänder einzuhalten. Blindleistung kann durch regelbare Transformatoren und die Regelung der Wirkleistung von Erzeugungs- bzw. Verbrauchsanlagen ausgeglichen werden. Für Großkunden bestehen bei hohen Blindleistungsbedarfe gesonderte vertragliche Vereinbarungen.

 
![Spannungshaltung1](img/Koordinationsaufgaben/Spannungshaltung_a.png "Abbildung 2a: Beispiel zur Spannungshaltung, Spannungsband wird verletzt (eigene Darstellung).")
 
![Spannungshaltung2](img/Koordinationsaufgaben/Spannungshaltung_b.png "Abbildung 2b: Spannungshaltung greift ein und bringt die Spannung zurück in den erlaubten Bereich (eigene Darstellung).")

### Vergleich Systemdienstleistungen 
 
**Frequenzhaltung**

- Systemweit beeinflussbar
- Wirkleistung

**Spannungshaltung**

- Lokal beeinflussbar
- Blindleistungsbilanz ist relevant 
- auch über Wirkleistung beeinflussbar

--> Bereitstellung von Systemdienstleistungen durch neue Akteure 
(dezentrale Kleinanlagen im Gegensatz zu Großkraftwerken) somit differenziert zu betrachten!

 
## Bilanzkreis

**Worum geht es eigentlich?**

Als kontinuierliche Aufgabe in elektrischen Netzen müssen Last und Erzeugung in Einklang gebracht werden (d.h. die Netzfrequenz gleich zu halten, wie in Abbildung 3 angedeutet). Dies soll – ergänzend zur physikalischen Ausgleichsmechanismen im Netz – weiterhin zu jedem Zeitpunkt über die entsprechenden Märkte realisiert werden. Als Planungsaufgabe bzw. Ausgleichsaufgabe wird dies umgesetzt durch: **Bilanzkreismanagement, Regelleistung und Engpassmanagement**.

![Netzfrequenzwaage](img/Koordinationsaufgaben/Netzfrequenzwaage.png "Abbildung 3: Der Ausgleich von Last und Erzeugung beeinflusst die Netzfrequenz (eigene Darstellung).")

### Bilanzkreismanagement
Die Energiemärkte übernehmen die marktseitigen Aspekte der Frequenzhaltung, indem die Übertragungsnetzbetreiber (ÜNB) als Verantwortliche für den Ausgleich von Erzeugung und Verbrauch in ihrer Regelzone zuständig sind. Jeder Lieferant (Marktrolle) muss dafür einen sogenannten Bilanzkreis führen und erhält somit zusätzlich die Rolle eines Bilanzkreisverantwortlichen (BKV). 

Der Bilanzkreis leitet sich aus der Summe der Fahr-/Einsatzpläne ab (siehe Abbildung 4) und bildet die kleinste Energieeinheit, die ausgeglichen sein muss. Dies wird auf einem virtuellen Energiemengenkonto abgebildet, dessen Saldo ausgeglichen werden muss. 


![Bilanzkreis](img/Koordinationsaufgaben/Bilanzkreismanagement.png "Abbildung 4: Ein Bilanzkreis leitet sich aus der Summe der Fahr-/Einsatzpläne ab (eigene Darstellung).")
 
Die für die Fahrpläne prognostizierten Energiemengen der Lieferanten müssen dem ÜNB für jede Viertelstunde des Folgetags gemeldet werden. Innerhalb des Bilanzkreises müssen alle Verbräuche durch Erzeugung oder Energieeinkäufe sowie die gesamte Erzeugung durch Verbrauch oder Energieverkäufe gedeckt sein. 

Für die Bilanzkreisabrechnung werden die tatsächlichen Verbräuche und Erzeugungen viertelstündlich gemessen und ebenfalls gemeldet. Dabei können Abweichungen auftreten (siehe Abbildung 5). Kurzfristige Ungleichgewichte (Summe aller Bilanzkreisabweichungen) werden durch Regelleistung ausgeglichen. Die benötigte Ausgleichsenergie wird den Lieferanten in Rechnung gestellt.

![Bilanzkreisabrechnung](img/Koordinationsaufgaben/Bilanzkreisabrechnung.png "Abbildung 5: Tatsächliche Verbräuche und Erzeugungen für die Bilanzkreisabrechnung (eigene Darstellung).") 

Der gesamte Ablauf ist in Abbildung 6 dargestellt.

![Bilanzkreismanagement_Schritte](img/Koordinationsaufgaben/Bilanzkreismanagementschritte.png "Abbildung 6: Bilanzkreismanagement (eigene Darstellung)")




> **Weitere Erklärungen über elektrische Energieversorgung**
>
> 1.	Heuck, K., Dettmann, K.-D., Schulz, S.: Elektrische Energieversorgung, 9. edn. Springer, Wiesbaden (2013)
> 2.	Crastan, V.: Elektrische Energieversorgung 2, 4. edn. Springer, Berlin (2016) 


**Quiz: Was ist richtig?**


[[ ]] Der Bilanzkreisverantwortliche ist dafür verantwortlich, dass die Strommengen für Erzeugung und Verbrauch zu jedem Zeitpunkt physikalisch ausgeglichen sind. 
[[x]] Der Bilanzkreisverantwortliche hat dafür zu sorgen, dass die Strommengen auch ggfs. erst im Nachhinein (z.B. am Folgetag) innerhalb seines Bilanzkreises ausgeglichen sind.
[[ ]] Bilanzkreise werden gänzlich virtuell und ohne jeden Bezug zur Netzinfrastruktur definiert.
