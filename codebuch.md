Codebuch Frank Sinatra
================
Tom Geyer
2024-06-25

# Codebuch SNA Projekt:*Frank Sinatra und die Mafia*

## Informationen zum Netzwerk

Das Netzwerk umfasst die Verbindungen zwischen **Frank Sinatra** und
verschiedenen Akteuren innerhalb der **italienisch-amerikanischen
Mafia**. Es beinhaltet die sozielen und geschäftlichen Beziehungen von
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
Beziehungsstärke basierend auf der Häufigkeit von Zusammenarbeit oder
Treffen zwischen den beiden Akteuren  
1 = schwache Beziehung  
2 = starke Beziehung  
3 = sehr starke Beziehung  

**friendship**  
Besteht zwischen den beiden Akteuren eine freundschaftliche/soziale Beziehung?  
1 = ja  
2 = nein  

**family**  
Besteht zwischen den beiden Akteuren eine familiäre Beziehung?  
1 = ja  
2 = nein  
  
**work**  
Art der geschäftlichen Zusammenarbeit der Akteure  
1 = legal  
2 = illegal  
3 = keine  

**activity**  
Art der Aktivität die die beiden Knoten verbindet  
1 = Drohung  
2 = Überfall  
3 = Mord

**year**  
Jahr in dem die Verbindung zustande kam als Zahl

## Node-Attribute

**id**  
(eindeutige Codierung jedes Akteurs/Knotens)  
codiert als Kürzel bestehend aus den ersten beiden Buchstaben von Vor-
und Nachname (Frank Sinatra -\> frsa) <br>
Wenn sich ids doppeln, wird der dritte Buchstabe des Nachnamens hinzugefügt.

**id_name**  
Name der Person/Organisation

**nickname**  
Gängigster Spitzname/Mafiabezeichnung der Person

**job**  
Haupttätigkeit der Person  
1 = Künstler  
2 = Mafia  
3 = Manager  

**sex**  
Geschlecht der Person  
1 = weiblich  
2 = männlich

**position**  
Position innerhalb der Mafiastrukturen  
1 = Aussenstehender  
2 = Handlanger  
3 = Oberhaupt

**age_death**  
Alter der Person bei ihrem Tod (als Zahl angegeben)

**city**  
Stadt in der die Person tätig/am häufigsten tätig war

**state**  
Bundesstaat in dem die Stadt liegt, codiert nach Abkürzungen siehe:  
<https://github.com/tg087/SNA-Frank-Sinatra/blob/main/abk%C3%BCrzungen_bundesstaaten.csv>

**type**  
Unterscheidung der Art des Akteurs in Person, Familie und Organisation  
1 = Person  
2 = Familie  
3 = Organisation
