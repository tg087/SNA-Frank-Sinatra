Codebuch Frank Sinatra
================
Tom Geyer
2024-06-25

# Codebuch SNA Projekt:*Frank Sinatra und die Mafia*

## Informationen zum Netzwerk

Das Netzwerk umfasst die Verbindungen zwischen **Frank Sinatra** und
verschiedenen Akteuren innerhalb der **italienisch-amerikanischen
Mafia**. Es beinhaltet die sozielen und geschäftlichen Beziehungen von
Sinatra und den Mitgliedern der organisierten Kriminalität.
Datengrundlage bilden historische Dokumente wie die veröffentlichten
**FBI-Akten** von Fällen rund um Sinatra und Mafia-Akteure. Hinzu kommen
Zeitungsberichte sowie **Fachliteratur** zur Geschichte der
italienisch-amerikanischen Mafia.

Bei diesem Netzwerk handelt es sich um ein **two-mode-Netzwerk**, mit
**gerichteten** und unterschiedlich **gewichteten Beziehungen**. Als
Akteure treten sowohl die Personen, als auch die Organisationen
(Mafia-Clans/Familien) auf.

## Edge-Attribute

**from** Knoten von welchem die Interaktion/Beziehung ausgeht

**to** Knoten welcher Interaktion/Beziehung “empfängt”

**weight** Beziehungsstärke basierend auf der Häufigkeit von
Zusammenarbeit oder Treffen zwischen den beiden Akteuren 1 = schwache
Beziehung 2 = starke Beziehung 3 = sehr starke Beziehung

**relationship** Art der sozialen Beziehung der beiden Akteure 1 =
Arbeit 2 = Freunde 3 = Familie

**activity** Art der Aktivität die die beiden Knoten verbindet 1 =
Drohung 2 = Überfall 3 = Mord

## Node-Attribute

**id** (eindeutige Codierung jedes Akteurs/Knotens) codiert als Kürzel
bestehend aus den ersten beiden Buchstaben von Vor- und Nachname (Frank
Sinatra -\> frsa)

**name** Name der Person/Organisation

**nickname** Gängigster Spitzname/Mafiabezeichnung der Person

**sex** Geschlecht der Person

1 = weiblich 2 = männlich

**position** Position innerhalb der Mafiastrukturen

1 = Aussenstehender 2 = Handlanger 3 = Oberhaupt

**age_death** Alter der Person bei ihrem Tod (als Zahl angegeben)

**location** Ort an dem die Person tätig/am häufigsten tätig war
