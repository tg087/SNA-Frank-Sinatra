Codebuch Frank Sinatra
================
Tom Geyer
2024-06-25

# Codebuch SNA Projekt:*Frank Sinatra und die Mafia*

## Informationen zum Netzwerk

Das Netzwerk umfasst die Verbindungen zwischen **Frank Sinatra** und
verschiedenen Akteuren innerhalb der **italienisch-amerikanischen
Mafia** von 1943 bis 1985. Es beinhaltet die sozialen und geschäftlichen Beziehungen von
Sinatra und den Mitgliedern der organisierten Kriminalität und der Unterhaltungsbranche.
Datengrundlage bilden historische Dokumente wie die veröffentlichten
**FBI-Akten** von Fällen rund um Sinatra und Mafia-Akteure. Hinzu kommen
Zeitungsberichte sowie **Fachliteratur** zur Geschichte der
italienisch-amerikanischen Mafia.

Bei diesem Netzwerk handelt es sich um ein **two-mode-Netzwerk**, mit
**gerichteten** und unterschiedlich **gewichteten Beziehungen**. Als
Akteure treten sowohl die Personen, als auch die Organisationen
(Mafia-Clans/Familien) auf.

## Edge-Attribute

**from**  

Knoten von welchem die Interaktion/Beziehung ausgeht

**to**  

Knoten welcher Interaktion/Beziehung “empfängt”

**weight**  

Bei dieser Kategorie geht es um die Beziehungsstärke basierend auf der Häufigkeit von Zusammenarbeit oder Treffen zwischen den beiden Akteuren. Diese Kategorie ist essentiell um nicht nur eine Beziehung nachzuweisen sondern auch die Intensität zu analysieren.

Hier haben wir in folgende Kategorien unterteilt: 

1 = schwache Beziehung  
2 = starke Beziehung  
3 = sehr starke Beziehung  

Eine Beziehung wurde als schwach definiert wenn Personen im Zusammenhang nur einmalig genannt wurden und diese nicht speziell als eng beschrieben wurde. 

Eine Starke Beziehung wurde definiert wenn dieselben Personen mehr als einmal oder bis zu drei Mal Kontakt miteinander hatten.

Eine sehr starke Beziehung lag bei uns dann vor wenn Personen mehr als drei Mal in Zusammenhang genannt wurden oder es ausdrücklich in unseren Quellen notiert war wie zum Beispiel durch Freundschaft oder auch Verwandtschaft.


**family**  

Die Kategorie family beschreibt, ob zwischen den Akteuren eine familiäre Beziehung bestand. Diese Kategorie war interessant, um zu analysieren, ob Sinatra möglicherweise familiäre Verbindungen zur Mafia hatte oder nicht. Außerdem war es spannend, die Verwandtschaftsverhältnisse innerhalb des Mafia-Netzwerks zu identifizieren.

Die Kategorie family wurde durch die Beantwortung der Frage unterteilt: Sind die Personen miteinander verwandt?

1 = ja  
2 = nein  
  
**work**  

Diese Kategorie bezieht sich auf die Art der geschäftlichen Zusammenarbeit zwischen den Akteuren. Sie war besonders relevant für unser Netzwerk, da wir analysieren konnten, wie viele geschäftliche Zusammenarbeiten stattfanden und ob überhaupt welche innerhalb von Sinatras Netzwerk zur Mafia und innerhalb der Mafia existierten. Falls geschäftliche Aktivitäten nachweisbar waren, wurde außerdem zwischen legalen und illegalen Tätigkeiten unterschieden.

Die Kategorien:  
1 = legal  
2 = illegal  
3 = keine  

**activity**  

Activity beschreibt die Art der Aktivität, die die beiden Knoten verbindet. Diese Kategorie bot uns die Möglichkeit, verschiedene Arten von Interaktionen oder Beziehungen zwischen Frank Sinatra und der Mafia präzise zu klassifizieren. Dadurch konnten wir feststellen, ob die Verbindungen beispielsweise rein sozialer Natur waren, wie durch Freundschaften, wirtschaftlich motiviert, wie durch Profit, oder kriminell belastet, wie etwa durch Drohungen, Überfälle oder Mord.

Drohung, Überfall und Mord wurden aus den Akten entnommen, wenn über diese offenkundig berichtet wurde.

Profit wurde angenommen, sobald die Personen – unabhängig davon, ob durch legale oder illegale Geschäftsverhältnisse – miteinander in Kontakt standen.

Freundschaft und Kontakt unterschieden wir wie folgt: Kontakt wurde definiert, wenn die Personen weniger als dreimal in Zusammenhang miteinander genannt wurden. Freundschaft wurde benutzt, wenn die Personen dreimal oder öfter in Zusammenhang genannt wurden oder wenn in den Akten ausdrücklich auf eine enge Beziehung, wie durch Freundschaft oder Verwandtschaft, hingewiesen wurde.

Die Kategorien bei activity: 

1 = Drohung  
2 = Überfall  
3 = Mord  
4 = Profit  
5 = Freundschaft  
6 = Kontakt

**year**  

Die Kategorie year stellt das konkrete Jahr dar, in dem die Verbindung zwischen den verschiedenen Personen in Sinatras Netzwerk zustande kam. Diese Kategorie zeigt somit die zeitliche Entwicklung der Verbindungen auf. Die Wahl eines genauen Jahres war hier von Vorteil, da sie die Analyse präziser und aussagekräftiger gestaltete.

Durch diese Einteilung konnten wir untersuchen, wie sich die Verbindungen zwischen Sinatra und der Mafia im Laufe der Zeit verändert haben. Dadurch ließ sich erkennen, ob die Kontakte zur Mafia in bestimmten Zeitabschnitten seines Lebens intensiver waren als in anderen.

## Node-Attribute

**id**  

(eindeutige Codierung jedes Akteurs/Knotens)  
codiert als Kürzel bestehend aus den ersten beiden Buchstaben von Vor-
und Nachname (Frank Sinatra -\> frsa) <br>
Wenn sich ids doppeln, wird der dritte Buchstabe des Nachnamens hinzugefügt.

**id_name**  

Name der Person/Organisation

**nickname**  

Diese Kategorie stellte den gängigsten Spitznamen oder die gängigste Mafiabezeichnung der jeweiligen Personen dar. Besonders in unserem Netzwerk, in dem die meisten Personen der Mafia zuzuordnen sind, war dies essenziell zu wissen. In den FBI-Akten wurden Mafia-Bosse oder Mitglieder häufig mit ihren Spitznamen bezeichnet, da diese oft bekannter waren als ihre Geburtsnamen. Bekannte Beispiele zur Verdeutlichung sind:

Lucky Luciano (eigentlich Salvatore Lucania)

Al Capone (eigentlich Alphonse Gabriel Capone)

Frank Costello (eigentlich Francesco Castiglia)

Da die unterschiedlichen Personen oft eine Vielzahl an Spitznamen besaßen und nicht immer nur einen eindeutigen Spitznamen hatten, war es notwendig, einen einheitlichen Spitznamen auszuwählen, um Missverständnisse zu vermeiden. Wir entschieden uns, jeweils den gängigsten Spitznamen zu verwenden.

Den gängigsten Spitznamen ermittelten wir, indem wir alle bekannten Spitznamen der jeweiligen Personen filterten nach der häufigkeit. Der am häufigsten genannte Spitzname wurde dann einheitlich verwendet.

**job**  

Diese Kategorie stellte die Haupttätigkeiten der jeweiligen Personen aus Sinatras Netzwerk dar. Sie zeigte speziell auf, dass Sinatra laut den FBI-Akten vermutlich mit Mafia-Mitgliedern in Verbindung stand. Dies würde seine Behauptungen widerlegen, niemals Kontakt zur Mafia gehabt zu haben, und ist daher zentral für unsere Forschungsfrage.


Die Haupttätigkeit der Personen in die wir unterteilten sind: 

1 = Künstler  
2 = Mafia  
3 = Manager  
4 = Sonstiges

**sex**  

Diese Kategorie bezieht sich auf das Geschlecht der jeweiligen Person. Aufgrund des zeitlichen Kontexts unserer Analyse war es nicht erforderlich, eine weitere Unterscheidung, wie beispielsweise divers, vorzunehmen. Außerdem wollten wir mit dieser Unterscheidung ermitteln ob die Mafia Mitglieder rund um Sinatra nur männlich oder auch weiblich waren.

Unsere Kategorien:

1 = weiblich  
2 = männlich

**position**  

Diese Kategorie beschreibt die Position einer jeweiligen Person innerhalb der Mafiastrukturen.

Die Unterteilung erfolgte wie folgt:

Außenstehender: Definiert als Person, die keinerlei Verbindung zur Mafia hatte.

Handlanger: Bezeichnete eine Person, die der Mafia zugehörig war und für diese tätig wurde, jedoch nicht als Oberhaupt in den FBI-Akten erwähnt wurde.

Oberhaupt: Eine Person, die der Mafia zugeordnet wurde und speziell als Oberhaupt oder Chef einer Mafia-Organisation in den Akten erwähnt war.

Durch diese Kategorie konnten wir zusätzlich filtern, wie tiefgreifend Sinatras Verbindungen zur Mafia und Kriminalität tatsächlich gewesen sein mussten. Besonders Verbindungen zwischen Sinatra und Mafia-Oberhäuptern lieferten Hinweise darauf, dass er nicht nur Kontakte zur Mafia hatte, sondern dass diese auch tiefgreifend und verwurzelt waren.

Unsere Kategorien:

1 = Aussenstehender  
2 = Handlanger  
3 = Oberhaupt

**age_death**  

Alter der Person bei ihrem Tod (als Zahl angegeben)

**city**  

Die Kategorie City gibt an, in welcher Stadt die jeweiligen Personen am häufigsten tätig waren. Diese Information hilft uns, Sinatras Verbindungen zur italienisch-amerikanischen Mafia besser zu verstehen, da sie zeigt, in welchen Städten diese Beziehungen besonders stark ausgeprägt waren oder wo es vermehrt Kontakte zwischen Sinatra und der Mafia gegeben haben soll.

Darüber hinaus ermöglicht diese Kategorie die Analyse von Mustern innerhalb der Mafia, beispielsweise welche Mitglieder oder Familien besonders stark in bestimmten Städten vertreten waren und wo sie hauptsächlich tätig waren.

Zudem liefert sie Aufschluss darüber, ob Sinatra vor allem lokal in einer bestimmten Stadt mit Mafia-Mitgliedern in Verbindung stand oder ob er Teil eines größeren, überregionalen Netzwerks war.

Außerdem können wir erkennen, welche Städte eine zentrale Rolle in Bezug auf Sinatra und die Mafia gespielt haben und ob Sinatra sich vermehrt in Städten aufhielt, die als Mafia-Hochburgen bekannt sind, wie beispielsweise Las Vegas oder New York.

**state**  

Bundesstaat in dem die Stadt liegt, codiert nach Abkürzungen siehe:  
<https://github.com/tg087/SNA-Frank-Sinatra/blob/main/abk%C3%BCrzungen_bundesstaaten.csv>

**type**  

Diese Kategorie unterscheidet die Art des Akteurs und gibt an, ob es sich um eine Person oder eine Mafia-Familie handelt. Mit der Kategorie Type wird klar, ob eine Verbindung direkt mit einer bestimmten Person, wie beispielsweise Frank Sinatra und Lucky Luciano, bestand oder ob sie einer Mafia-Familie, wie der Genovese-Familie, zugeordnet werden kann.

Diese Einteilung ermöglichte es uns unter anderem, zu analysieren, welche Mafia-Familien miteinander in Kontakt standen. Darüber hinaus konnten wir beobachten, wie einzelne Mafia-Personen mit bestimmten Mafia-Familien in Verbindung standen und welchen Familien sie zugehörig waren.

Zusätzlich bot die Kategorie die Möglichkeit, zu untersuchen, ob Sinatra nur mit einzelnen Mafia-Personen oder auch mit mächtigen, einflussreichen und kriminell organisierten Familien in Kontakt stand. Diese Informationen lieferten wertvolle Hinweise darauf, wie tiefgreifend und mächtig das kriminelle Netzwerk um Sinatra gewesen sein muss.

Bei den Mafia-Familien konzentrierten wir uns auf die sogenannten Big Five, also die fünf größten italo-amerikanischen Mafia-Familien. Diese sind:
die Bonanno-Familie, die Colombo-Familie, die Gambino-Familie, die Genovese-Familie und die Lucchese-Familie.
Diese fünf Familien waren zu Sinatras Zeit besonders bekannt für ihre dominierende Rolle im organisierten Verbrechen.

Unsere Kategorien: 

1 = Person  
2 = Familie
