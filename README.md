# KI


# Künstliche Intelligenz – Vorlesung 1 (2024)

## Modul: Künstliche Intelligenz  
**Prof. Dr. Heinrich Jasper**  
**TU Bergakademie Freiberg**  

---

## Zielsetzung des Moduls

- **Erwerb von Kenntnissen und Fertigkeiten** in:
  - Grundlagen der Künstlichen Intelligenz (KI)
    - Begriffsbildung
    - Methoden und Techniken
    - Anwendungsgebiete
    - Historie und Stand der Technik
  - Übungen zur KI
    - Spezielle Themen
    - Einführung in **PROLOG** als Programmiersprache

---

## Begriffsbildung

### Definitionen Künstlicher Intelligenz
- **Systeme, die wie Menschen denken** (Haugeland, 1985)
- **Systeme, die wie Menschen handeln** (Rich & Knight, 1991)
- **Systeme, die rational denken** (Winston, 1992)
- **Systeme, die rational handeln** (Nilsson, 1998)

> **Zusammenfassung:** KI ist eine Informatikanwendung. Sie ist dem neuronalen Netzwerk unseres Gehirns nachempfunden. KI kann einen Ausschnitt menschlicher Intelligenz nachahmen. Das Besondere ist die Fähigkeit zu lernen. Das unterscheidet KI‐Systeme von herkömmlichen Computerprogrammen. Statt einem Programm genau zu sagen, was es tun soll, bekommt das KI‐System eine Aufgabe gestellt, die es selbständig zu lösen hat.

### Wichtige Merkmale
- Lernfähigkeit
- Aufgabenbewältigung ohne genaue Programmierung

---

## Motivation

- **Anwendungsfelder**:
  - Sprachverstehen (Smart Devices, GPTs)
  - Autonome Systeme (Fahrzeuge, Roboter)
  - Militärtechnologien (Drohnen, Kampfmaschinen)
  - Virtuelle Welten (Spiele, VR)
- **Zielsetzung**:
  - Verstehen und Beeinflussung natürlicher Intelligenz
  - Aufbau künstlich intelligenter Systeme
  - Kombination beider Richtungen (Intellektik)

---

## Intelligente Agenten

- Begriffseinführung durch Mind-Maps (Details folgen in späteren Veranstaltungen)

---

## Einordnung der KI

### Forschungsgebiete:
- Kognition / Bildverarbeitung / Sprachverstehen
- Wissensverarbeitung / Problemlösen / Analogien
- Lernen / Autonomie / Interaktion
- Genetik / Evolution

### Technologien und Systeme:
- Suchverfahren
- Funktionale, logische, objektorientierte Programmierung
- Expertensysteme
- Wissensrepräsentation / Logisches Schließen
- Machine Learning: Clustering, Klassifikation, Assoziation
- Robotik / Agentensysteme
- Neuronale Netze
- Genetische Algorithmen

---

## Historische Grundlagen

| Bereich | Wichtige Persönlichkeiten |
| :------ | :------------------------ |
| Philosophie | Aristoteles, Hobbes, da Vinci |
| Mathematik | Boole, Turing, Gödel |
| Betriebswirtschaft | Smith, von Neumann |
| Neurowissenschaften | Broca, Berger |
| Psychologie | Wundt, Craik |
| Technische Informatik | Zuse, Turing |
| Kontrolltheorie | Wiener, McCulloch |
| Linguistik | Chomsky, Skinner |

---

## Entwicklung der KI

### Frühzeit (1943–1955)
- Künstliches Neuron
- Hebb’sche Lernregel
- Turing-Test
- Erste genetische Algorithmen

### Begriffsbildung (1956)
- **Dartmouth Workshop**: Gründung der KI als Forschungsfeld

### Enthusiasmus (1952–1969)
- Entwicklung von GPS (General Problem Solver)
- Programmiersprache **LISP**
- Lernende Programme (z.B. Schach, Geometriebeweiser)

### Erste Ernüchterung (1966–1973)
- Fördermittelrückgang wegen unerfüllter Erwartungen

### Wissensbasierte Systeme (1969–1990)
- Expertensysteme, Regelsysteme, Wissensrepräsentation

### Erfolgreiche KI-Forschung (ab 1980)
- PROLOG, neuronale Netze, autonome Systeme, Agententechnologie

### Zweiter KI-Winter (1990–ca. 2010)
- Enttäuschung über allgemeine KI-Techniken

### Heute (2020+)
- Massive Fortschritte:
  - Autonome Fahrzeuge
  - Sprach- und Bild-KI (z.B. GPT, Stable Diffusion)
  - Integration in Alltagsgeräte (Waschmaschinen, Kreditsysteme)
- Große Herausforderungen:
  - Ethische und gesellschaftliche Fragen
  - Verständnis von Intelligenz und Rationalität

---

## Aktuelle Anwendungen

- Autonome Computer- und Fahrzeugsysteme
- Diagnosesysteme (Medizin, Technik)
- Planungs- und Optimierungssysteme
- Robotik
- Sprachverstehen und Übersetzung
- Wissensverarbeitung und Ontologien
- Semantische Suchen
- Emotionale Agenten
- Bio-/Neurologische Analogien
- Theoretische Forschung zu KI-Grundlagen

---


# VL2 - Intelligente Agenten – Zusammenfassung

## Allgemeines Modell

- **Definition**: Intelligente Agenten sind Systeme, die wirklich als intelligent bezeichnet werden können.
- **Grundstruktur**:
  - **Agent** interagiert mit der **Umgebung**.
  - Nutzt **Sensoren** zur Wahrnehmung und **Aktuatoren** zur Ausführung von Aktionen.

```
Agent <-> Umgebung
(Sensoren zur Wahrnehmung, Aktuatoren für Aktionen)
```

## Rationaler Agent

- **Ziel**: Auswahl von Handlungen, die die Leistungsbewertung maximieren.
- **Leistungsbewertung**: 
  - Definiert, was ein "gutes" Verhalten ist.
  - Bewertet den Erfolg eines Agenten.
- **Wichtige Aspekte**:
  - Rationalität bedeutet nicht Allwissenheit oder Perfektion.
  - Lernen ist zentral für die Verbesserung der Leistung.

## Arbeitsumgebungen von Agenten (Beispiele)

| Agententyp | Leistungsbewertung | Umgebung | Aktuatoren | Sensoren |
|:---|:---|:---|:---|:---|
| Medizinisches Diagnosesystem | Gesunder Patient, minimale Kosten/Klagen | Patient, Krankenhaus, Team, Medikamente | Fragen, Untersuchungen, Diagnosen, Empfehlungen | Tastatureingaben, Symptome, Befunde |
| Satellitenbildanalyse | Korrekte Bildkategorisierung | Downlink vom Satelliten | Anzeige der Kategorisierung | Farbpixelarrays |
| Packroboter für Teile | Prozentsatz korrekter Teile | Fließband mit Teilen, Behälter | Arm und Greifhand | Kamera, Winkelsensoren |
| Raffinerie-Controller | Maximale Reinheit/Fördermenge/Sicherheit | Raffinerie, Arbeiter | Ventile, Pumpen, Heizungen, Anzeigen | Temperatur-, Druck-, chemische Sensoren |
| Interaktiver Englischlehrer | Maximale Testergebnisse | Schüler, Prüfungskommission | Übungen, Vorschläge, Korrekturen | Tastatureingabe |

### Weitere Beispiele:
- **Drohne**: Mission auf Planetenoberfläche, Sensor- und Waffensteuerung.
- **Autonomes Fahrzeug**: Gute Fahrt von A nach B, Kommunikation mit Umwelt und anderen Fahrzeugen.

## Kategorisierung von Arbeitsumgebungen

- **Vollständig vs. Teilweise beobachtbar**: Sind alle Informationen der Umgebung verfügbar?
- **Deterministisch vs. Stochastisch**: Gibt es Zufallseinflüsse?
- **Episodisch vs. Sequenziell**: Einzelne Entscheidungen oder verkettete?
- **Statisch vs. Dynamisch**: Verändert sich die Umgebung unabhängig vom Agenten?
- **Diskret vs. Stetig**: Endliche vs. kontinuierliche Zustände.
- **Einzelagent vs. Multiagenten**: Arbeitet der Agent alleine oder kooperativ?

## Struktur eines Agenten

- **Architektur**: Physische Komponenten wie Sensoren, Aktuatoren.
- **Programm**: Logik und Algorithmen, die das Verhalten steuern.

## Typen von Intelligenten Agenten

1. **Einfache Reflex-Agenten**:
   - Entscheidung nur anhand aktueller Wahrnehmung.
   - Realisiert über Bedingungs-/Aktions-Tabellen.

2. **Modellbasierte Reflex-Agenten**:
   - Führen ein Modell der Welt basierend auf bisherigen Wahrnehmungen.
   
3. **Zielbasierte Agenten**:
   - Planen Handlungen, um definierte Ziele zu erreichen.

4. **Nutzenbasierte Agenten**:
   - Bewerten verschiedene Zustände und wählen den besten.

5. **Lernende Agenten**:
   - Verbesserung der Leistung durch Feedback und Lernalgorithmen.

## Reflexagenten – Probleme

- **Table-Driven Agent**:
  - Realisierung über eine Tabelle, die Wahrnehmungen Aktionen zuordnet.
  - Unpraktikabel: Bei großer Datenmenge explodiert die Größe der Tabelle exponentiell.

- **Beispiel**:
  - Sensor liefert 27 MB/Sekunde, 1 Stunde Fahrzeit ⇒ gigantische Tabelle (mehr als Atome im beobachtbaren Universum).

## Agenten und Wissen

- **Wissensbasiertes System**:
  - Enthält eine **Wissensbasis**, ein **Inferenzsystem**, ein **Wissensmodell** und nutzt eine **Modellierungssprache**.

- **Verhaltensbasiertes System**:
  - Direktes Handeln durch Regeln, ohne tiefgreifende Wissensrepräsentation.

### Übersicht:

| Kategorie | Beschreibung |
|:---|:---|
| Künstlich-intelligente Systeme | Überbegriff |
| Wissensbasierte Systeme | Nutzung von explizitem Wissen |
| Verhaltensbasierte Systeme | Direkte Aktion ohne tiefes Wissen |
| Expertensysteme | Spezialwissen + Schlussfolgern auf engen Aufgabengebieten |

## Expertensysteme (XPS)

- **Ziel**: Simulation des Fachwissens und der Problemlösungsstrategien von Experten.
- **Vorgehen**:
  - Wissen wird formalisiert und maschinell nutzbar gemacht.
  - Wissensingenieur implementiert die Problemlösungsstrategien.
  
- **Vorteil**:
  - Änderung und Wartung einfacher als bei konventionellen Programmen durch klare Trennung von Wissen und Strategie.

## Komponenten eines Expertensystems

- **Benutzungsschnittstelle**: Interaktion mit dem Benutzer.
- **Interviewerkomponente**: Aufnahme neuer Fakten.
- **Erklärungskomponente**: Begründung von Entscheidungen.


- **Inferenzsystem**: Schlussfolgerung von neuen Erkenntnissen.
- **Wissensakquisitionskomponente**: Integration neuen Wissens.
- **Wissensbasis**: Zentrale Sammlung von Fakten und Regeln.
- **Wissensmodell** (Knowledge Representation Model): Die Art und Weise, wie Wissen im System dargestellt wird.
  - Beispiele:
  - Regeln (Wenn-Dann-Form)
  - Frames (Objekte mit Attributen)
  - Ontologien (strukturierte Begriffe und Relationen)
  - Semantische Netze oder Logikbasierte Modelle
- **Modelierungssprache**: Eine formale Sprache zur Darstellung von Wissen.
  - Beispiele:
  - Prolog
  - OWL (Web Ontology Language)
  - LISP, CLISP


# VL3 Exkurs: PROLOG – Logikprogrammierung in der Künstlichen Intelligenz

## 🎯 Ziel
- Wissensverarbeitung mittels **Logikprogrammierung**
- Einführung in die Programmiersprache **PROLOG** (*Programming in Logic*)

## 📚 Historischer Hintergrund

| Forscher        | Beitrag                                                                 |
|----------------|--------------------------------------------------------------------------|
| Frege (~1880)  | Begriffswelt als mathematische Sprache                                   |
| Herbrand, Skolem, Gödel (1920–1935) | Mathematischer Beweisaufbau                         |
| Robinson (1965)| Resolution (Schlussfolgerung aus Axiomen)                                |
| Colmerauer (1972)| Entwicklung von PROLOG mit Resolution & Unifikation                    |
| Kowalski (~1982)| „Algorithm = Logic + Control“                                           |

## 🔤 Grundelemente von PROLOG

### 1. **Fakten**
```prolog
auto.
name(bernd).
vater_von(bernd, erwin).
```

### 2. **Regeln**
```prolog
vorfahr_von(X,Y) :- vater_von(X,Y).
vorfahr_von(X,Y) :- mutter_von(X,Y).
```

### 3. **Abfragen**
```prolog
?- vater_von(bernd, X).
X = erwin.
```

## 🔍 PROLOG-Prinzipien

### a) Fakten
```prolog
fleisch(schnitzel).
fisch(aal).
verheiratet(bernd, ilse).
```

### b) Anfragen
```prolog
?- fleisch(schnitzel).  % yes
?- fleisch(aal).        % no
?- fisch(X).            % X = aal; X = scholle
```

### c) Regeln
```prolog
gesund(X) :- obst(X).
obst(apfel).
```

### d) Suchstrategie
- Tiefensuche mit Backtracking
- Regelreihenfolge wichtig!
- Achtung: Kann zu Nicht-Terminierung führen.

## 🧱 Objekte in PROLOG

### a) Atome, Zahlen, Strukturen
```prolog
geboren(fritz, 1, 10, 1938).
geboren(fritz, datum(1,10,1938)).
```

### b) Operatoren
```prolog
1 + 3 * 4  => +(1, *(3,4))
```

### c) Listen
```prolog
[]
[1]
[x,y]
[a|[b|[c]]]
```

### d) Variablen
```prolog
Vater
_vater
_
```

### e) Terme
```prolog
?- istVatervon(zeus, ares). % yes
?- 2+3 = 5.                 % no
```

## 🧠 Fakten und Regeln

### 3. **Fakten**
```prolog
katze(mieze).
```

### 4. **Regeln**
```prolog
tier(X) :- katze(X), lebt(X).
```

## 🔁 Resolutionsprinzip
- Unifikation:	Struktureller Vergleich zweier Terme
- Substitution:	Bei erfolgreicher Unifikation werden die Variablen durch konkrete Werte ersetzt. Das nennt man Substitution.
- Resolution:	Anwendung von Regeln/Fakten durch Unifikation + Substitution
- Backtracking:	Rückverfolgung zur nächsten Alternative bei Fehlschlag



## 🔁 PROLOG-Prozeduren & Programme

### Definition:
- Programm = Klauseln (Fakten + Regeln)
- Prozedur = gleiche Kopf-Funktoren
- Anfrage = spezielle Klausel

## 📊 Semantik von PROLOG

- Semantik = Beweise im SLD-Resolutionsbaum \\
SLD: Selektive lineare Definite-Clause-Resolution

Auflösung erfolgt durch sukzessives Ersetzen von Zielen durch Regelköpfe

Backtracking, sobald keine Regel anwendbar ist

Liefert Beweise in Form eines Herleitungsbaums

## ✅ Zusammenfassung

- PROLOG: deklarative Sprache zur Wissensverarbeitung
- Prinzipien: Fakten, Regeln, Abfragen, Backtracking, Unifikation
- Anwendung: symbolische KI, Expertensysteme, Sprache



# VL4 🤖 Künstliche Intelligenz – Problemlösung durch Suchen

## 🔍 Problemlösender Agent

- Zielbasiert: Ziel ist durch einen oder mehrere wünschenswerte Zustände definiert.
- Keine Begrenzung der Zustände im Voraus.
- Ziel: Finde eine Aktionsfolge, die zum Ziel führt und führe sie aus.

### Parameter zur Problemformulierung:
- Wie ist das Ziel definiert?
- Welche Zustände sind relevant?
- Welche Aktionen sind möglich?

### Begriffe:
- Suche = Ermittlung der Aktionsfolge
- Agentenmodell: **Formulieren – Suchen – Ausführen**
- **Uninformierte Suche**: keine Information über Qualität der Zustände
- **Informierte Suche**: Bewertung der Zustände möglich

---

## 🧠 Einfacher Problemlöser (Pseudocode)

```pseudo
function EinfacherProblemlöser(percept) returns action
    static: seq ← []
    state ← update_state(state, percept)

    if seq is empty:
        goal ← formulate_goal(state)
        problem ← formulate_problem(state, goal)
        seq ← search(problem)

    if seq not empty:
        action ← first(seq)
        seq ← rest(seq)

    return action
end
```

---

## 📐 Wohldefinierte Probleme

- **Ausgangszustand**
- **Nachfolgerfunktion**: liefert `<Aktion, Nachfolgerzustand>`
- **Zieltest**: prüft Zielzustand
- **Pfadkosten**: Summe der Aktionskosten

**Zustandsraum** = gerichteter Graph

**Optimale Lösung** = Lösung mit minimalen Pfadkosten

---

## ♟️ Beispielprobleme

### 🧩 8-Puzzle

- Zustände: Positionen der Zahlen & Leerfeld
- Nachfolgerfunktion: Bewegung des Leerfelds (oben, unten, links, rechts)
- Zieltest: erreicht Zielanordnung
- Pfadkosten: 1 pro Bewegung

### 👸 8-Damen-Problem

- Ziel: 8 Damen auf Schachbrett, keine bedroht eine andere
- Alternative Zustandsdarstellung reduziert Anzahl zu prüfender Zustände

---

## 🚚 Praktische Probleme

- Routenplanung, Logistik, Handlungsplanung
- Schaltungsdesign
- Roboternavigation
- Internet-Suche

---

## 🌲 Suchbäume und Strategien

### Definition eines Suchbaums:

- Wurzel = Ausgangszustand
- Kinder = Nachfolger gemäß Nachfolgerfunktion
- Strategie bestimmt Reihung der Expansion

```pseudo
function tree-search(Problem, Strategie)
    initialisiere Suchbaum mit Ausgangsknoten
    while true:
        wenn keine Kandidaten: return Fehler
        wähle Knoten laut Strategie
        wenn Ziel erreicht: return Lösung
        sonst: erweitere Knoten
```

---

## 🔄 Uninformierte Suchstrategien

### 1. Breitensuche (BFS)
- Vollständig, optimal
- Zeit- & Speicherkomplexität: O(b^d)

| Tiefe | Knoten    | Zeit         | Speicher    |
|-------|-----------|--------------|-------------|
| 2     | 1,100     | 0,1 Sek      | 1 MB        |
| 6     | 10^7      | 19 Minuten   | 10 GB       |
| 12    | 10^13     | 35 Jahre     | 10 PB       |

---

### 2. Tiefensuche (DFS)
- Nicht vollständig, nicht optimal
- Geringer Speicherbedarf

### 3. Iterative Deepening
- Kombiniert BFS & DFS

### 4. Bidirektionale Suche
- Zwei gleichzeitige Suchen von Start und Ziel
- Komplexität: O(b^(d/2))

### 5. Weitere Strategien
- Uniforme-Kosten-Suche
- Begrenzte-Tiefen-Suche
- Iterative-Tiefen-Suche

---

## 🧠 Informierte Suchstrategien

- Nutzung von Heuristiken h(n)

### Greedy Best-First Search
- Wählt immer den Knoten mit dem kleinsten geschätzten Abstand zum Ziel. h(n)
- Risiko: Sackgassen
- Schnell, aber nicht optimal, da es Abkürzungen übersehen kann.

### A*-Suche
- f(n) = g(n) + h(n)
- g(n): Kosten bisher
- h(n): geschätzte Kosten zum Ziel
- Kombination aus optimal & effizient
- Suche mit Blick auf Vergangenheit und Zukunft.

---

## 🧗 Lokale Suche & Optimierung

### Hillclimbing
- Folge dem besten lokalen Nachfolger mit dem besten Heuristikwert.
- Gefahr: lokales Optimum

### Simulated Annealing
- Erlaubt gelegentlich auch schlechtere Lösungen
- Nutzt Temperaturparameter T und Wahrscheinlichkeit zur Akzeptanz

---

## 🧬 Evolutionäre Algorithmen (EA)

- Simulation biologischer Evolution
- Individuen = Lösungskandidaten
- Fitnessfunktion = Bewertung

### Hauptkomponenten:
- **Rekombination r**: Kombination zweier Individuen
- **Mutation m**: zufällige Veränderung
- **Selektion s**: Auswahl fitter Individuen
- **Abbruchbedingung z**

### Ablaufschema:
```text
Initialisierung: P(0)
Bewertung: f(a_i)
while !Abbruch:
    Rekombination
    Mutation
    Bewertung
    Selektion
    t = t + 1
```

---

## 🧪 Evolutionsstrategien (ES)

- Ein anderer Typ von evolutionärem Algorithmus, entwickelt in Deutschland (Rechenberg, Schwefel).
- 🧠 Besonderheiten:
  - Fokus auf reale Zahlen (nicht Bitstrings!)
  - Stärker betont: Mutation statt Crossover
  - Anpassung der Mutationsstärke über Zeit (selbstadaptiv)
- Besonders gut für kontinuierliche Optimierungsprobleme (z. B. Maschinensteuerung, Robotik)

### Beispiel:
- F(x1,x2) = x1² + x2²
- Individuum = (x1, x2, s1, s2)
- Mutation und Rekombination über Strategieparameter

---

## 🧬 Genetische Algorithmen (GA)

- Bitstring-Repräsentation der Individuen als Genotyp
- Operatoren: **Crossover**, **Mutation**, **Selektion**
- Können auch in Problemen ohne exakte mathematische Beschreibung eingesetzt werden
- Suche im diskreten Raum
- Nutzen: Scheduling (z. B. Flugpläne)
### Crossover:
- Zwei Eltern → Kind durch Bittausch an zufälliger Stelle

### Mutation:
- Flip einzelner Bits mit geringer Wahrscheinlichkeit

---

## 📌 Fazit

- Suche ist zentrales Konzept in der KI
- Informierte Strategien und heuristische Verfahren bieten Effizienzvorteile
- Lokale und evolutionäre Verfahren ergänzen die klassischen Suchalgorithmen bei komplexen Problemen


# VL5 📚 Künstliche Intelligenz – Wissensrepräsentation & Logik

## 🤖 Logisch schließender Agent

ein Agent, der Wissen über die reale Welt enthält, das
- aus der Beschreibung möglicher Zustände, Operationen und Zusammenhänge besteht,
- zur Ableitung von Zustandseigenschaften und Operationsfolgen genutzt werden kann,
- verändert bzw. gelernt werden kann.

### Komponenten:
- **Wissensbasis**: Menge von Sätzen über die reale Welt
- **Inferenzverfahren**: Ableitung neuer Sätze
- **Wissensrepräsentationssprache**:
  - **Syntax**: Repräsentationen im Agenten
  - **Semantik**: Fakten der realen Welt


- Beweis: Aufzeichnung der Anwendung von Schlussregeln eines Inferenzverfahrens
- Theorie: Menge der aus einem Kalkül ableitbaren Formeln
---
## Aussagelogik
Behandelt aussagenlogische Variablen, die entweder wahr oder falsch sind.
Man arbeitet mit einfachen Aussagen und Verknüpfungen wie UND, ODER, NICHT, → (Implikation)

### Hilbert-Axiomensystemen (Aussagelogik):
Das Hilbert-System (benannt nach David Hilbert) ist ein axiomatisches System, das mit:

- einer kleinen Anzahl von Axiomen (Grundformeln), und
  - De Morgen, Verschmelzung, Konjunktion, ...
- wenigen Schlussregeln (v. a. Modus Ponens)

jede gültige Aussage der Aussagenlogik beweisbar machen will.

Eigenschaften: vollständig, **entscheidbar**, wiederspruchsfrei, monoton, unabhängig

## Prädikatenlogik
- Erweitert die Aussagenlogik um Objekte, Eigenschaften und Quantoren.
- Hier kann man über Dinge in der Welt sprechen – nicht nur über Wahrheitswerte.

- Eigenschaften: vollständig, **nicht entscheidbar**, wiederspruchsfrei, monoton, unabhängig
  - nicht entscheidbar: Es gibt kein Verfahren, das für alle Aussagen entscheidet, ob sie gültig sind (wegen der Unendlichkeit von Domänen)


Beide Logiksysteme sind vollständig, widerspruchsfrei, monoton und unabhängig.
Aber nur die Aussagenlogik ist entscheidbar – die Prädikatenlogik nicht.
# VL 6
- Eine **Klausel** ist eine ODER-Verknüpfung (Disjunktion) von Literalen.
  - vollständig, nicht entscheidbar
- Eine **Hornklausel** ist eine spezielle Klausel mit höchstens einem positiven Literal.
- Hornklauseln sind Grundlage von Prolog und ermöglichen effizientes logisches Schließen.
  - Sie ermöglichen einfache Implementierung logischer Systeme wie Expertensysteme oder Regelwerke
  - nicht vollständig, nicht entscheidbar

## Ableitungsstrategien
### Vorwärtsverkettung:
- Startet mit Fakten, leitet neue ab, bis das Ziel erreicht ist.
- Konfliktlösung: Prioritäten, Reihenfolge, Spezifität.
  - Wenn mehrere Regeln gleichzeitig anwendbar sind, spricht man von einem Konflikt. Eine Konfliktlösungsstrategie entscheidet, welche Regel zuerst ausgeführt wird.
### Rückwärtsverkettung:
- Man beginnt mit einer Anfrage oder Hypothese und sucht rückwärts, ob es Regeln und Fakten gibt, mit denen man das Ziel beweisen kann.
- Vergleich: Ähnlich zu Prologs Tiefensuche.

## Regelbasiertes System
Ein regelbasiertes System (auch Produktionssystem genannt) ist ein wissensbasiertes System, das automatisch Schlussfolgerungen zieht und Entscheidungen trifft, indem es Regeln auf bekannte Fakten anwendet.

Ein regelbasiertes System besteht aus
- Datenbasis mit den gültigen Fakten
- Regeln zur Herleitung neuer Fakten / Ausführung von Aktionen
- Regelinterpreter zur Steuerung des Herleitungs-/Ausführungsprozesses

Prinzipielle Abarbeitungsmechanismen eines Regelinterpreters
- Vorwärtsverkettung: feuere Regeln solange, bis sich die Datenbasis (eine Menge von Fakten) nicht mehr ändert
oder Abbruchbedingung erfüllt ist
- Rückwärtsverkettung: Vom Ziel ausgehend, werden Vorbedingungen etabliert; prüfe, ob Vorbedingungen
erfüllbar (Fakten oder Rückfragen beim Nutzer), ansonsten: Vorbedingungen sind das nächste Ziel.


Was ist eine spezifischere Regel?
- Eine spezifischere Regel hat mehr Bedingungen auf der linken Seite (Prämisse) → sie ist eingeschränkter, wird also selten angewendet, aber liefert gezieltere Schlüsse.


## Frames
Idee: Aussagen über ein Objekt strukturiert zusammenfassen
- Ein Frame ist eine Art Datenstruktur, die ein Konzept, Objekt oder eine Situation beschreibt – ähnlich einem Objekt in der Objektorientierten Programmierung.

- Ein Frame besteht aus:
  - Slots (Attribute, Eigenschaften, Fragen)
  - Slot-Filler (Werte, Regeln, andere Frames)

- Sie sind vererbbar und können Prozeduren enthalten (Programme, die Eigenschaften eines Objekts zugeordnet sind)

- Frames eignen sich besonders gut zur repräsentativen Darstellung realer Objekte und sind leicht erweiterbar.
- FRL (Frame Representation Language) ist eine spezielle Repräsentationssprache, die entwickelt wurde, um Frames formal darzustellen und zu verarbeiten

### Kognitive Wurzel:
Der Begriff „kognitive Wurzel“ weist darauf hin, dass Frames auf Beobachtungen der menschlichen Kognition beruhen – also wie Menschen Wissen speichern, organisieren und abrufen.

## Semantische Netze
Ein semantisches Netz ist eine graphbasierte Wissensdarstellung, bei der Konzepte (Knoten) und deren Beziehungen (Kanten) visuell und logisch dargestellt werden.

- Eigenschaften:
  - Knoten = Begriffe/Objekte (z. B. „Hund“, „Tier“)
  - Kanten = Beziehungen (z. B. „ist-ein“, „hat-Teil“, „lebt-in“)
  - Beziehungen sind oft gerichtet: von Subjekt zu Objekt

- Nutzen:
  - Intuitive Visualisierung von Wissen
  - Wird oft für Sprachverarbeitung und Ontologien genutzt

Ein semantisches Netz stellt Wissen in Form eines gerichteten Graphen dar – mit Knoten als Objekten und Kanten als Relationen. Es eignet sich gut zur Vererbung und Konzeptdarstellung.

### KL-ONE
KL-ONE ist eine formale Weiterentwicklung semantischer Netze.
Es ist ein strenges, logikbasiertes Klassifikationssystem, das Begriffshierarchien definiert – also ein Begriffsnetz mit Logikregeln.

- Grundlage für viele moderne Ontologie-Systeme wie OWL


## Constrains Netze
Ein Constraint-Netz ist eine graphische Darstellung eines Constraint-Satisfaction-Problems (CSP).
Es zeigt, welche Variablen vorkommen, welche Wertebereiche (Domänen) sie haben, und welche Einschränkungen (Constraints) zwischen ihnen bestehen.

Nutze:
  - Stundenpläne
  - Sudoku
  - Routenplanung

# VL 7
## Was ist ein Plan-Agent?
![alt text](image.png)

Merkmale:
- Hat ein Modell der Welt (Zustände, Aktionen, Effekte)
- Nutzt logische Repräsentation (z. B. Situationskalkül)
- Wendet Planungsalgorithmen an

## Situationskalkül
Zur formalen Beschreibung von Handlungen und deren Effekten
![alt text](image-2.png)
😰 Herausforderung: Frame-Problem
→ Wie stellt man formell dar, was sich nicht ändert, wenn eine Aktion ausgeführt wird?

Beispiel: Wenn man die Tür öffnet, bleiben Tisch, Stuhl, Fensterzustand etc. gleich – das muss extra berücksichtigt werden.


## Was ist ein Planungsalgorithmus?
Ein Planungsalgorithmus ist ein Verfahren, das eine Reihenfolge von Aktionen erstellt, um einen Zielzustand von einem Startzustand aus zu erreichen. Typische Planalgorithen: A*-Planung, STRIPS

- Gegeben: Start-, Zielzustand, Operationen
- Erzeugen eines Intialen Planes
- Suche im Zustandsraum → finde Pfad von Start → Ziel
- Erzeuge Aktionsfolge (Plan)
- Überprüfe während Ausführung: Ist der aktuelle Zustand wie erwartet?
- Bei Abweichung: Replanung

## Initialer Plan
Ein initialer Plan ist der erste Vorschlag oder Ablauf von Aktionen, der erstellt wird, um ein bestimmtes Ziel zu erreichen.

Ein Agent kann erkennen, dass der initiale Plan nicht mehr gültig ist, wenn:
| Methode                               | Beschreibung                                                                                         |
| ------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| **Planüberprüfung (Plan Monitoring)** | Während der Ausführung prüft der Agent regelmäßig, ob alles wie geplant läuft.                       |
| **Soll-Ist-Vergleich**                | Der Agent vergleicht erwartete Zustände mit aktuellen Zuständen.                                     |
| **Fehlschlag beim Ausführen**         | Wenn eine Aktion nicht möglich ist (z. B. Tür ist blockiert), erkennt der Agent: Plan ist gebrochen. |
| **Sensorfeedback**                    | Neue Informationen machen den Plan veraltet oder falsch.                                             |

In solchen Fällen wird ein neuer Plan erzeugt = Replanung

# VL 8
## Lernender Agent
Ein Agent, der seine Eingaben nicht nur zur Steuerung seiner unmittelbaren Ausgaben verwendet sondern auch zur Veränderung (Verbesserung) seiner zukünftigen Verhaltensweise.

- Formen des Lernens:
  - Speichern von Erfahrungen, Klassifizierung, Verallgemeinerung, Theoriebildung.
  - Beispiele: Navigation, Schach, Sprachverarbeitung.

- Komponenten:
  - Problemlöser: Steuert das aktuelle Verhalten.
  - Lernkomponente: Passt Wissen anhand von Rückmeldungen an.
  - Kritiker: Bewertet Erfolg/Misserfolg.
  - Problemgenerator: Erzeugt Trainingsdaten oder Testfälle.

- Lernarten:
  - Überwacht (gelabelte Daten), Verstärkend (Belohnung/Strafe), Unüberwacht (Clustering).

### Aufgabenstellungen und Algorithmen
- **Vorhersage** (Regressionsaufgaben):
    Ziel: Funktion f(x)f(x) approximieren (z. B. mittels linearer Regression).
    - Lernkurve: Anzahl korrekt bearbeiteter Testbeispiele bei gegebener Anzahl von
Trainingsbeispielen
    - Fehlerfunktion e(h) = P(h(x) ≠ f(x)) ist zu minimieren
- **Klassifikation**: beobachtete Situation (Sensordaten) einer gegebenen Klasse zuordnen.
  - Arten von Classifiern
    - Entscheidungsbäume
    - Regessionsbäume etc. (a.a.O.)
    - Semantische Netze etc. (a.a.O.)
    - Multidimensionale Zuordnungen

  - **Entscheidunsbäume**: Ein Entscheidungsbaum ist ein baumartiges Klassifikationsmodell, das rekursiv Attribute auswählt, um Daten in Klassen zu unterteilen. Die Attributauswahl basiert z. B. auf Informationsgewinn (Entropie).

    - 🎯Vorteile von Entscheidungsbäumen
      - Einfach zu verstehen und interpretieren
      - Können symbolisches Wissen erzeugen
      - Arbeiten gut mit kategorischen und numerischen Daten
      - Keine Annahme über Datenverteilung nötig

    - ⚠️ Nachteile
      - Overfitting, wenn Baum zu tief ist
      - Instabil gegenüber kleinen Änderungen in den Daten
      - Pruning (Beschneiden) notwendig, um Generalisierung zu verbessern


  - **kNN (k-Nearest Neighbors)**: kNN ist ein klassifikationsbasiertes Lernverfahren, das eine neue Eingabe auf Basis der k nächsten Trainingsbeispiele klassifiziert. Es ist einfach, nicht-parametrisch, aber rechenintensiv beim Vorhersagen.

  Wie funktioniert kNN?
  - Du hast eine Menge gelabelter Datenpunkte (Trainingsdaten).
  - Für einen neuen, unbekannten Punkt:
    - Berechne den Abstand zu allen Trainingspunkten (z. B. euklidisch).
    - Wähle die k nächstgelegenen Nachbarn.
    - Mehrheitsabstimmung (Voting): Die Klasse, die am häufigsten unter den k Nachbarn vorkommt, wird zugewiesen.

### Clustering:
Clustering ist ein Verfahren des unüberwachten Lernens, bei dem Datenobjekte in Gruppen (Cluster) eingeteilt werden, sodass:

- Objekte innerhalb eines Clusters möglichst ähnlich sind
- Objekte zwischen Clustern möglichst unterschiedlich

✅ Keine Klassenlabels notwendig! \\
Bsp.: Kunden in Gruppen mit ähnlichem Kaufverhalten einteilen

#### Wie funktioniert k-Means?
k-Means ist ein iteratives Clustering-Verfahren, das Daten in k Cluster unterteilt. \\
Ziel: Minimierung der Summe der Abstände zwischen Datenpunkten und ihrem jeweiligen Cluster-Zentrum (Centroid)

🔁 Ablauf des k-Means-Algorithmus:
- Wähle k: Anzahl der Cluster
- Initialisiere k Zentren zufällig
- Zuordnungsschritt (Assignment):
- Weise jeden Punkt dem nächsten Zentrum zu (z. B. nach euklidischer Distanz)
- Update-Schritt:
- Berechne für jeden Cluster das neue Zentrum (Mittelwert der zugewiesenen Punkte)
- Wiederhole 3 & 4, bis sich die Zentren nicht mehr ändern (Konvergenz)

### Lernen logischer Formeln
Ziel: Generierung logischer Hypothesen, die Trainingsdaten konsistent abbilden.
### Lernen besseren Verhaltens
- Künstliche Neuronale Netze (KNN/ANN):
    - Prinzip: Anpassung von Gewichten durch Backpropagation (Fehlerrückführung).
    - Deep Learning: Mehrschichtige Netze für komplexe Mustererkennung (z. B. Bilderkennung).
- Verstärkendes Lernen:
    - Ziel: Maximierung einer Belohnungsfunktion durch Exploration/Exploitation.
    - Beispiel: Robotersteuerung, Spielstrategien (AlphaGo).

# VL 9
## ✅ Was ist ein künstliches Neuron?

Ein **Neuron** ist die kleinste Recheneinheit in einem neuronalen Netz.  
Es empfängt Eingaben, multipliziert sie mit Gewichten, addiert einen Bias und gibt das Ergebnis über eine **Aktivierungsfunktion** weiter.

### 🔧 Aufbau eines Neurons:

![alt text](image-4.png)

- Eingaben: `x₁, x₂, ..., xₙ`
- Gewichte: `w₁, w₂, ..., wₙ`
- Bias: `b` (Verschiebung der Aktivierung)
- Suchfunktion: `z = ∑(wᵢ * xᵢ) + b` Die Suchfunktion ist die gewichtete Summenbildung der Eingabewerte.
Sie bestimmt, wie stark ein Neuron aktiviert wird, bevor die Aktivierungsfunktion angewendet wird.
- Aktivierungsfunktion: `a = f(z)` Die Aktivierungsfunktion nimmt den Ausgabewert der Suchfunktion und entscheidet, wie stark das Neuron feuert (also welchen Wert es weitergibt).

### 🎛️ Typische Aktivierungsfunktionen:

| Funktion   | Formel                         | Beschreibung                        |
|------------|--------------------------------|-------------------------------------|
| Sigmoid    | `1 / (1 + e^(-z))`             | Werte zwischen 0 und 1              |
| Tanh       | `(e^z - e^-z) / (e^z + e^-z)`  | Werte zwischen -1 und 1             |
| ReLU       | `max(0, z)`                    | Beliebt, effizient, sparsam         |

---

## 🤖 Neuron vs. Perzeptron

| Merkmal                 | Neuron (modern)                        | Perzeptron (klassisch)              |
|-------------------------|----------------------------------------|-------------------------------------|
| Aktivierungsfunktion    | ReLU, Sigmoid, Tanh (differenzierbar) | Schwellenwertfunktion (0/1-Ausgabe)        |
| Differenzierbar         | ✅ Ja                                  | ❌ Nein                              |
| Für Backpropagation     | ✅ Ja                                  | ❌ Nein                              |
| Komplexe Aufgaben       | ✅ Mehrschichtnetze möglich            | ❌ Nur lineare Trennung              |

**Merksatz:**  
> Das Perzeptron ist die Urform des Neurons mit harter Schwelle.  
> Ein modernes Neuron nutzt differenzierbare Aktivierungsfunktionen und ist trainierbar.

---

## 🧱 Woraus besteht eine Schicht?

Eine **Schicht (Layer)** ist eine **Gruppe von Neuronen**, die gleichzeitig arbeiten und ihre Ausgaben an die nächste Schicht weitergeben.

### 🧩 Typen von Schichten:

1. **Eingabeschicht (Input Layer)**  
   → Nimmt Rohdaten auf

2. **Verborgene Schicht(en) (Hidden Layer)**  
   → Berechnungsschritte mit Aktivierungen

3. **Ausgabeschicht (Output Layer)**  
   → Liefert Klassifikation oder Regressionswert

Ein neuronales Netz besteht aus einer Eingabeschicht (Puffer), einer oder mehreren verborgenen Schichten (Assoziierung) und einer Ausgabeschicht (Antwort).
Die Assoziierungsschicht verarbeitet die Daten und „lernt“ die Merkmale zur Klassifikation oder Entscheidung.

## 🧠 Klausur-Merksätze:

- Ein **Neuron** = gewichtete Summe + Bias → Aktivierungsfunktion
- Das **Perzeptron** ist eine Vorform mit Schwellwertfunktion
- Eine **Schicht** besteht aus mehreren Neuronen – das Netz aus mehreren Schichten


## Was ist Backpropagation?
Backpropagation (Rückwärtsausbreitung) ist ein Trainingsverfahren für neuronale Netze, bei dem die Gewichte so angepasst werden, dass der Fehler (Loss) zwischen dem vorhergesagten und dem tatsächlichen Wert minimiert wird.

Neuronale Netze bestehen aus vielen Schichten – der Fehler der Vorhersage (z. B. falsche Klasse) muss rückwärts durch das Netz propagiert werden, damit jede Gewichtung entsprechend angepasst werden kann.


Anforderungen für Backpropagation:
- Aktivierungsfunktionen müssen differenzierbar sein (z. B. Sigmoid, ReLU)
- Der Fehler muss mit einer Kostenfunktion (Loss Function) messbar sein
- Stützverfahren: Kettenregel der Differentialrechnung

1. Vorwärtsdurchlauf (Forward Pass):
- Eingabedaten durchlaufen das Netz
- Ausgabe wird berechnet
- Fehler wird durch Vergleich mit dem Zielwert (z. B. über MSE oder Cross-Entropy) bestimmt
2. Fehlerberechnung:
- Differenz zwischen Ausgabe und gewünschtem Zielwert = Loss
3. Rückwärtsdurchlauf (Backward Pass):
- Der Fehler wird von der Ausgabeschicht zurück zu den Eingabeschichten propagiert
- Für jedes Gewicht wird der Gradient (Ableitung) des Fehlers berechnet
4. Gewichtsanpassung (Gradient Descent):
- Gewichte werden aktualisiert:

## 🤖 Künstliche Neuronale Netze – Kurzfragen

### ❓ Wie groß soll ein KNN sein?
> So groß wie nötig, aber so klein wie möglich.  
> Zu viele Neuronen → Overfitting  
> Zu wenige → unzureichende Lernfähigkeit

---

### ❓ Wie viele verborgene Schichten benötigt man?
> Für einfache Probleme reicht **eine** Schicht.  
> Komplexere Probleme → **mehrere Schichten (Deep Learning)**  
> Achtung: Mehr Schichten = schwieriger zu trainieren

---

### ❓ Kann ein trainiertes Netzwerk auf beliebige Testdaten generalisieren?
> ❌ Nein.  
> Nur wenn Testdaten **ähnlich verteilt** sind wie die Trainingsdaten.  
> Sonst drohen **Overfitting** oder schlechte Vorhersageleistung.

---

### ❓ Kann man die Funktion \( y = F(X, W) \) eines trainierten Netzes finden?
> ✅ Ja, **theoretisch möglich**, durch vollständiges Einsetzen aller Gewichte und Aktivierungen.  
> ❌ Aber **praktisch unübersichtlich** und nicht interpretierbar bei großen Netzen (nicht transparent).

# 🤖 Deep Learning – RNN, LSTM, CNN & Convolution

## 🔁 Was ist ein RNN (Recurrent Neural Network)?

Ein **RNN** ist ein neuronales Netz, das für **sequenzielle Daten** (z. B. Sprache, Text, Zeitreihen) entwickelt wurde.  
Es nutzt eine **Rückkopplungsschleife**, sodass **Informationen aus früheren Zeitschritten** weitergegeben werden können.

### 🔧 Besonderheiten:
- Jeder Zeitschritt erhält zusätzlich zum Input auch den **Zustand vom vorherigen Schritt**:  
  \( h_t = f(Wx_t + Uh_{t-1} + b) \)
- Ideal für: **Texte, Sprache, Musik, Zeitreihen**

### ❌ Problem:
- **Vanishing/Exploding Gradients** → Schwierigkeiten beim Lernen **langer Abhängigkeiten**

---

## 🧠 Was ist Deep Learning?

**Deep Learning** ist maschinelles Lernen mit **mehrschichtigen neuronalen Netzen** (deep = tief).

### 🔧 Merkmale:
- Besteht aus **vielen Hidden Layers**
- Nutzt **Backpropagation** zur Gewichtsanpassung
- Führt oft zu **automatischer Merkmalsextraktion**
- Erfolgreich bei:  
  - Bildverarbeitung  
  - Sprachverarbeitung  
  - Textklassifikation  
  - Spiel-KI

---

## ⏳ Was ist ein LSTM (Long Short-Term Memory)?

Ein **LSTM** ist eine **erweiterte RNN-Architektur**, die das Problem des **Vanishing Gradients** löst.

### 🔧 Besonderheiten:
- Besteht aus **Speicherzellen**, die Informationen **über viele Zeitschritte speichern** können
- Verwendet **drei Tore**:
  - **Input Gate** – entscheidet, was aufgenommen wird
  - **Forget Gate** – entscheidet, was vergessen wird
  - **Output Gate** – entscheidet, was ausgegeben wird

✅ LSTM kann **langfristige Abhängigkeiten** lernen  
z. B. beim **Übersetzen ganzer Sätze**

---

## 🖼️ Was ist ein CNN (Convolutional Neural Network)?

Ein **CNN** ist ein neuronales Netz, das speziell für **Bild- und Mustererkennung** entwickelt wurde.

### 🔍 Eigenschaften:
- Erkennt **lokale Muster** (z. B. Kanten, Farben) mithilfe von **Convolution-Filtern**
- Nutzt **Pooling-Schichten** zur Reduktion der Datenmenge
- Besteht typischerweise aus:
  - **Convolutional Layer**
  - **Activation Layer** (z. B. ReLU)
  - **Pooling Layer**
  - **Dense (fully connected) Layer**

---

## 🔎 Was ist eine Convolution (Faltung)?

> Eine **Convolution** ist eine mathematische Operation, bei der ein **kleiner Filter (Kernel)** über das Eingabebild **gleitet** (Sliding Window).  
> Der Filter erkennt dabei **lokale Merkmale** wie Ecken oder Kanten.

### Beispiel:
Ein 3×3-Filter gleitet über ein Bild, multipliziert mit lokalen Pixelwerten und erzeugt so eine **Feature Map**.

✅ Vorteil:
- Weniger Parameter
- Gute Generalisierung
- Lokale Erkennung bei gleichzeitiger Effizienz

---
# <span style="color:red"> Bis hier!</span>
## 🧩 Was ist Pooling (in CNNs)?

**Pooling** ist eine Methode zur **Verkleinerung** der Feature Maps in **Convolutional Neural Networks (CNNs)**.  
Ziel: **wichtigste Informationen behalten**, aber **Größe und Komplexität reduzieren**.

### 📉 Vorteile:
- Spart Rechenleistung
- Verhindert Overfitting
- Sorgt für **Translationstoleranz**

---

## 🔝 Was ist Max Pooling?

Beim **Max Pooling** wird aus jedem Pooling-Fenster (z. B. 2×2) der **größte Wert** ausgewählt.


## 📘 Klausur-Merksätze:

| Begriff | Erklärung |
|--------|-----------|
| **RNN** | Neuronales Netz mit Gedächtnis für Sequenzen. Speichert vorherige Zustände über Rückkopplung. |
| **Deep Learning** | Verwendung tiefer neuronaler Netze mit mehreren Hidden Layers zur Mustererkennung. |
| **LSTM** | Erweiterung von RNN mit „Gedächtnis“ (Zellen + Gates) zur Überwindung des Vanishing Gradient. |
| **CNN** | Netz für Bilderkennung, das über Convolution lokale Muster erkennt und verarbeitet. |
| **Convolution** | Mathematischer Filtervorgang, bei dem Merkmale lokal aus Bildern extrahiert werden. |
| **Pooling** reduziert die Größe der Feature Maps und hebt wichtige Informationen hervor.|
| **Max Pooling** wählt pro Bereich den größten Wert – Fokus auf starke Merkmale.|


## 📚 Was ist ein LLM (Large Language Model)?

Ein **LLM** ist ein großes Sprachmodell, das mit **riesigen Mengen an Textdaten** trainiert wurde, um **Sprache zu verstehen und zu erzeugen**.

### 🔧 Merkmale:
- Basiert meist auf der **Transformer-Architektur**
- Besteht aus **Hunderten Millionen bis Milliarden von Parametern**
- Beherrscht viele Aufgaben:
  - Textgenerierung
  - Zusammenfassung
  - Übersetzung
  - Fragebeantwortung
  - Codevervollständigung

### 🧠 Beispiele:
- GPT (OpenAI)
- BERT (Google)
- LLaMA (Meta)
- Claude (Anthropic)

## 📘 Klausur-Merksätze:

- **LLMs** sind riesige Sprachmodelle, die auf Basis von Transformern trainiert wurden.


# VL 11 und 12
![alt text](image-3.png)

- Bsp.: Medizin, Technik

### unbedingte Wahrscheinlichkeit: a priori
Die unbedingte Wahrscheinlichkeit ist die „einfache“ Wahrscheinlichkeit eines Ereignisses – ohne dass irgendwelche weiteren Informationen bekannt sind.´

### bedingte Wahrscheinlichkeit: a posteriori
Die bedingte Wahrscheinlichkeit ist die Wahrscheinlichkeit eines Ereignisses unter der Bedingung, dass ein anderes Ereignis bereits eingetreten ist.

**Der ZUsammenhang beider wird bei der Bayesschen Regel benutzt**

## Was ist ein kausales Netzwerk?
Ein kausales Netzwerk ist ein gerichteter Graph, der kausale Zusammenhänge zwischen Variablen modelliert.

Man kann es sich als ein Bayessches Netz vorstellen, bei dem die Kanten kausale Beziehungen und nicht nur statistische Abhängigkeiten ausdrücken.

### Unterschied zu einem normalen (Bayesschen) Netzwerk
Ein Bayessches Netz beschreibt bedingte Wahrscheinlichkeiten und statistische Abhängigkeiten.
Ein kausales Netz geht weiter und beschreibt auch, was passiert, wenn man eingreift (interveniert).

## 🔍 1. Grundlagen des probabilistischen Schließens

- **Ziel**: Bewertung von Aussagen mit Wahrscheinlichkeiten, um Unsicherheiten abzubilden.
- **Herkunft der Unsicherheiten**:
  - Repräsentative Statistiken
  - Experteneinschätzungen

### Anwendungsbereich:
- **Diagnostik**:
  - Symptome → mögliche Diagnosen
  - Unsicherheiten durch:
    - Symptomerhebung
    - Symptombewertung
    - Unzulänglichkeiten des Verrechnungsschemas

### Kategorien von Unsicherheit (vereinfachte Einteilung):
- sicher
- wahrscheinlich
- möglich

### Verrechnungsschemata:
- Einfache, oft ad-hoc Repräsentationen
- Kritik: Mangelnde theoretische Fundierung

## 🧠 2. Diagnostik als Klassifikationsproblem

- Zwei disjunkte Mengen:
  - **S** = Symptome
  - **D** = Diagnosen
- Gegeben: Teilmenge der Symptome
- Gesucht: Wahrscheinlichste Diagnose(n)
- Möglichkeit, gezielt **weitere Symptome** zur Verbesserung anzufordern

### Logik:
- **Deduktion**: Aus Diagnose folgt Symptom
- **Abduktion**: Aus beobachteten Symptomen auf Diagnose schließen
- **Problematisch**: Unvollständigkeit, Widersprüche

### Anforderungen an Diagnosesysteme:
- Umgang mit unvollständigem Wissen
- Plausibilitätsprüfung
- Erkennung von Mehrfachdiagnosen
- Kosteneffektive Symptomerhebung

## ⚙️ 3. Grundalgorithmus

1. Start mit **Apriori-Wahrscheinlichkeiten** aller Diagnosen
2. Modifikation durch **Symptom-Diagnose-Wahrscheinlichkeiten**
3. Auswahl der wahrscheinlichsten Diagnose

## 📐 4. Theorem von Bayes

### Grundformel:
$$P(D_i | S) = \frac{P(D_i) \cdot P(S | D_i)}{P(S)}$$

### Beispiel:
- \( P(	ext{Bronchitis}) = 0.05 \)
- \( P(	ext{Husten}) = 0.2 \)
- \( P(	ext{Husten | Bronchitis}) = 0.8 \)
- → \( P(	ext{Bronchitis | Husten}) = 0.2 \)

### Probleme:
- Kombinatorische Explosion bei mehreren Symptomen
- Voraussetzung: Unabhängigkeit der Symptome
- Single-Fault-Annahme: nur eine Diagnose aktiv
- Statistiken müssen fehlerfrei & konstant sein

### Fazit:
> Anwendung des Bayes-Theorems oft theoretisch korrekt, praktisch jedoch zu ungenau.

## 🧮 5. Probabilistische Diagnosebewertung

### Bewertung:
- **Pro**: erwartete + beobachtete Symptome
- **Kontra**: erwartete, aber nicht beobachtete Symptome
- **Erklärungswert**: nicht erwartete, aber beobachtete Symptome

### Zusätzliche Aspekte:
- Prädispositionen
- Differentialdiagnostik

## 📊 6. Erweiterte Modelle zur Unsicherheitsverrechnung

### 🔷 Dempster-Shafer-Theorie
- Unsicherheitsintervalle statt exakter Werte: \[a, b\]
- P(Diagnose | Symptom) statt P(Symptom | Diagnose)
- Vorteile:
  - Repräsentation von Grobdiagnosen
  - Modellierung von Diagnosehierarchien
- Nachteil: hoher Rechenaufwand (\(2^n\) Diagnosemengen)

## 🏥 7. INTERNIST-Modell (siehe ChatGPT)

- Beruht auf Expertenwissen, keine exakten Wahrscheinlichkeiten
- Bewertungsfaktoren:
  - **Evoking Strength** (0–5)
  - **Frequency** (1–5)
  - **Import Value** (0–5)
- Diagnosen in Gruppen mit ähnlichen Merkmalen
- Bonuspunktesystem bei Mehrfachdiagnosen

## 🦠 8. MYCIN-Modell (siehe ChatGPT)

- Berücksichtigt:
  - positive & negative Evidenz
  - Symptomkombinationen (Regeln)
- Rechnet mit:
  - **Belief** & **Disbelief**
  - Ergebnis = **Certainty Factor**

## 🧪 9. MED1-Modell

- Zweistufiges Modell:
  1. Evidenzsummierung
  2. Klassifikation in 7 Klassen (z. B. wahrscheinlich, gesichert)
- Vorteil: flexible Repräsentation
- Nachteil: komplexe Interpretation

## 🔁 10. Alternative Ansätze

### 🔹 Default-Logik (Reiter)
- Arbeit mit Annahmen, Revision bei neuen Infos

### 🔹 Fuzzy-Logik (Zadeh)
- Wahrheitswerte ∈ [0, 1]
- Operatoren:
  - \( F(\neg A) = 1 - F(A) \)
  - \( F(A \land B) = \min(F(A), F(B)) \)
  - \( F(A \lor B) = \max(F(A), F(B)) \)

## 🧾 11. Zusammenfassung & Fazit

- Kein Modell ist vollständig zufriedenstellend.
- Größtes Problem: Unsichere Datenbasis
- Kompromiss:
  - **Weniger präzise, dafür robuster im Umgang mit Unsicherheiten**
- Modellwahl hängt ab von:
  - Einsatzgebiet
  - Verfügbarkeit von Daten
  - benötigter Genauigkeit

> 🔎 **Empfehlung**: So viel deterministisches Schließen wie möglich – so wenig probabilistisches wie nötig.


# 📘 KI-Vorlesung vom 13&14 – Verständliche und Ausführliche Zusammenfassung

## 🧠 Nicht-monotones Schließen: Was ist das?

### Klassische Logik (monoton):
- Einmal abgeleitete Aussagen bleiben **immer** gültig, selbst wenn neue Informationen dazukommen.

### Nicht-monotone Logik:
- Neue Informationen **können** bereits gezogene Schlussfolgerungen **ungültig** machen.
- Typisches Beispiel aus dem Alltag: Man geht davon aus, dass Vögel fliegen können – bis man einen Pinguin sieht.

### Gründe für nicht-monotones Schließen:
- Erwartungen werden überschrieben.
- Es tauchen Ausnahmen zu Regeln auf.
- Neue Informationen widersprechen alten Annahmen.

## 🔍 Ausnahmen & Negationen

- **Ausnahmen** blockieren das Auslösen einer Regel.
- **Negierte Aussagen** sagen aus, dass eine Aussage **nicht** zutrifft.
- Wichtig: In der **Closed World Assumption** (z. B. in PROLOG) wird "unbekannt" als "falsch" behandelt.

## 🛠 Belief Revision – Wie ändert man Schlussfolgerungen?

### Ziel:
- Wenn sich Informationen ändern, soll das System so reagieren, als hätte es diese Info **schon immer gehabt**.

### Methoden:
1. **Alles neu berechnen** – funktioniert nur bei kleinen Systemen.
2. **Backtracking** – ab dem Punkt neu berechnen, an dem sich etwas geändert hat.
3. **Minimaler Aufwand** – nur die betroffenen Schlussfolgerungen werden korrigiert.

## 🔄 TMS – Truth Maintenance Systems

### Typen:
- **JTMS (Justification-Based)**: Speichert direkte Begründungen.
- **ATMS (Assumption-Based)**: Speichert Basisannahmen.

### Beispiel-Regeln:
- R1: A → B
- R2: B → C
- R3: D ∧ ¬E → C

## 🔁 Zirkuläre Begründungen und Schleifen

- **Problematisch**, wenn sich Schlussfolgerungen gegenseitig stützen (z. B. A → B, B → A).
- **Monotone Schleifen** sind ok – **nicht-monotone** (mit Negationen) führen zu Endlosschleifen.

## 🧩 Strategien zur Schleifenbehandlung

1. **Current Support**: Nur eine Begründung zählt, andere werden ignoriert – spart Rechenaufwand.
2. **Automatische Schleifenerkennung**: 
   - z. B. im ITMS (Immediate-Check TMS)
   - Regeln, die zirkuläre Evidenz liefern könnten, werden markiert und ggf. blockiert.

## 🧱 ATMS – Kontextbasiertes Denken

- Jeder Schlussfolgerung ist ein **Kontext** zugeordnet = Kombination von Basisannahmen.
- **Knotenstruktur**:
  - Basisannahme
  - Gültigkeitskontext
  - Direkte Begründungen

## 🧮 Temporales Schließen

- Aussagen können **zeitabhängig** wahr oder falsch sein.
- Genutzt werden **modale Operatoren** wie:
  - NEXT F: ab nächstem Zustand
  - FUTURE F: irgendwann in der Zukunft
  - GLOBALLY F: immer

## 🩺 Diagnostiksysteme – Überblick

### Wissenstypen:
- Statistisch
- Fallbasiert (ähnliche Fälle vergleichen)
- Heuristisch (Expertenwissen)
- Kausal (Ursache-Wirkung)

### Kontrollstrategien:
- Vorwärtsverkettung
- Rückwärtsverkettung
- Hypothesize-and-Test

## 💉 Beispiel: MED2-System

- Verbindet viele Diagnosestrategien:
  - Verdachtsgenerierung
  - Verdachtsüberprüfung
  - Differentialdiagnostik
  - Therapievorschläge

## 🔧 Konstruktion – Der Unterschied zur Diagnostik

- Ziel: **Lösungen aktiv konstruieren**, nicht nur auswählen.
- Beispiele:
  - Stundenplanerstellung
  - Computer-Konfiguration
  - Molekulargenetische Planung
  - Werkstoffbearbeitung

### Zwei Haupttypen:
1. **Zuordnungsprobleme**: Bestehende Objekte richtig kombinieren.
2. **Transformationsprobleme**: Zustand verändern (z. B. vom Rohling zum fertigen Werkstück).

## 🛠 Planungstechniken

- **Hierarchisches Planen**: Abstrakte Pläne werden schrittweise konkretisiert.
- **Nicht-lineares Planen**: Interaktionen zwischen Teilproblemen werden berücksichtigt.
- **Differenzenmethode**: Differenz zwischen Ist- und Sollzustand bestimmen → passenden Plan generieren.
- **Wissensbasiertes Planen**: Verwendung von vorgefertigten Planskeletten.

## 💻 Beispiel: R1-System

- Konfiguration von DEC-Computern.
- Arbeitet in **6 Phasen** mit einfachen Regeln.
- Probleme:
  - Komplexe Wartung (30 Personen nötig!)
  - Geringe Transparenz der Wissensbasis

---

# ✅ Fazit

- **Nicht-monotones Schließen** spiegelt die Realität besser wider als klassische Logik.
- **Belief Revision Systeme** wie JTMS & ATMS ermöglichen flexible und nachvollziehbare Reaktion auf neue Informationen.
- **Diagnostik** und **Konstruktion** sind zwei zentrale Anwendungen der KI.
- Gute Planung erfordert **Abstraktion**, **Wissensrepräsentation** und oft **heuristische Regeln**.

