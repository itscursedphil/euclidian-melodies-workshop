---
theme: default
title: Euclidian Melodies
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
class: text-center
transition: slide-left
---

# Euclidian Melodies

Algorithmic sequencing techniques

---

# Topics

- Euclidian Rhythms
- Generative Sequencing / Algorithmic Sequencing
- CV
- Euclidian Melodies

---
layout: center
---

# Euclidian Rhythms

<!--
- Fragestellung
  - Wer kennt Euklidische Rhythmen bereits?
  - Wer nutzt sie zum Musik machen?
-->

---

# TL;DR

- Algorithmus zum Generieren von Rhythmen
- Schläge werden über die Länge des Rhythmus möglichst gleichmässig verteilt
- Parameter:
  - Länge des Rhythmus _(Steps)_
  - Anzahl der Schläge des Rhythmus _(Hits/Trigs)_
  - Verschiebung des Rhythmus _(Offset)_
- Verschiedene Rhythmen unterschiedlicher Längen können miteinander kombiniert werden

---

# Hintergrund

- 2004 von **Godfried Toussaint** entdeckt
- 2005 erstmals von ihm im Paper **“The Euclidean Algorithm Generates Traditional Musical Rhythms”** beschrieben
- beschreibt Algorithmus zur Generierung von Euclidischen Rhythmen und deren Anwendung

---

# Historischer Zuammenhang

- entstehende Rhythmen bilden fast alle wichtigen Rhythmen der Weltmusik ab (ausser einigen indischen Talas)
- Beispiele:
  - **Bossa Nova** _(Brasilien)_: 5 Hits/16 Steps `[x - - x - - x - - x - - x - - -]`
  - **Cumbia** _(Kolumbien)_: 3 Hits/4 Steps `[x - x x]`
  - **Tresillo** _(Cuba)_: 3 Hits/8 Steps `[x - - x - - x -]`
  - **Cinquillo** _(Cuba)_: 5 Hits/8 Steps `[x - x x - x x -]`
  - **Asak** _(Turkei)_: 4 Hits/9 Steps `[x - x - x - x - -]`
  - **Mpre** _(Ghana)_: 7 Hits/12 Steps `[x - x x - x - x x - x -]`
  - **Samba** _(Brasilien)_: 7 Hits/16 Steps (Start auf 15) `[x - x - - x - x - x - - x - x -]`

<!--
Beispiele zeigen: https://dbkaplun.github.io/euclidean-rhythm/
-->

---

# Mathematik

- Bezeichnung “Euklidische Rhythmen” auf Basis des griechischen Mathematiker **Euclid** _(300 v. Chr.)_
- Entdeckte Algorithmus um mathematisch den größten gemeinsamen Teiler von zwei Zahlen zu errechnen
- Euklidische Rhythmen nutzen die Formel, um Schläge in Rhythmus möglichst gleichmäßig zu verteilen (Resultat: Numerisch geteilte Zahlen werden auf ein Grid quantisiert)
- Mathematische Formel im Paper beschrieben: https://cgm.cs.mcgill.ca/~godfried/publications/banff.pdf **\[2\]**

---
layout: image-right
image: images/geo1.png
---

# Geometrie

- Euklidische Rhythmen können auch in einem Kreis dargestellt werden
- Algorithmus berechnet Polygone auf einem festen Raster möglichst gleichmäßig über den Kreis verteilt

---

# Mathemusics

- Mathematik findet sich überall in der Musik
  - Frequenzen (Frequenzkurve Exponentiell)
  - Oberton/Unterton-Reihe
  - FM Synthese/Additive Synthese
  - ...
- Musik auf Basis von mathematischen Konzepten erkunden kann zu spannenden musikalischen Ideen führen

---
layout: center
---

# Polyrhythm / Polymeter

---

# Polyrhythmus

- Unterschiedliche Anzahl von Schlägen wird in 2 oder mehr Rhythmen gleichmäßig **über die gleiche Taktlänge** verteilt _(z.B. linke Hand 3 Schläge, Rechte Hand 4 Schläge)_
- z.B. häufig in Afrikanischer Trommelmusik verwendet

<br />

# Polymeter

- 2 oder mehr Rhythmen **unterschiedlicher Taktlängen** laufen parallel
- Abstand zwischen Schritten ist der gleiche _(z.B. 16th, 8th, ...)_
- Rhythmen verweben sich immer wieder anders miteinander
- z.B. häufig in klassischer Minimal Music verwendet _([Bsp.: Steve Reich “Clapping Music”](https://www.youtube.com/watch?v=lzkOFJMI5i8))_

---

# Anwendung in Euklidischen Rhythmen

- Können beide Techniken nutzen um komplexe Rhythmen zu generieren
- **Polyrhythmus**: Unterschiedliche Taktarten für unterschiedliche Rhythmen
- **Polymeter**: Unterschiedliche Taktlängen für unterschiedliche Rhythmen (häufiger)

---
layout: center
---

# Generative Sequencing / Algorithmic Sequencing

Noten und/oder Rhythmen sind nicht fest komponiert, sondern auf Basis von Parametern wie Zufall, Wahrscheinlichkeit oder Regeln generiert

<!--
Fragestellung: Wer arbeitet mit generativen Techniken?
-->

---

# Generatives Sequencing

- (Häufig) Zufallsbasiert
- **Melodie**: zufällige Noten auf eine Tonart quantisiert
- **Rhythmus**: Schläge auf Basis von Wahrscheinlichkeit generiert
- "Probleme":
  - Fehlende musikalische Richtung
  - Wiederholung und Entwicklung von Melodie/Rhythmus fehlt
  - Das Ohr hat keinen Anker, an den es sich greifen kann

---

# Algorithmisches Sequencing

- **Algorithmus**: Formel/Feste Abfolge von Regeln, die zu einem Ergebnis führt _(bpsw. mathematische Gleichung)_
- Deterministisch weil regelbasiert: Mit gleichen Parametern immer das gleiche Ergebnis
- Entwicklung von musikalischen Themen bspw. durch Veränderung von Parametern über Zeit

---

# Algorithmic Sequencing vs Generative Sequencing

- Algorithmisch = Generativ und Generativ = Algorithmisch
- Interessant für Happy Accidents und Ideen, auf die man selber nicht gekommen wäre
- Beide Konzepte können aufeinander aufbauen

<!--
Beispiel: Algorithmisch wiederholende Sequenz in der einzelne Töne im Takt zufällig verändert werden
-->

---
layout: center
---

# Different kinds of CV?

<!--
Fragestellung: Welche Arten von CV gibt es?
-->

---

# Different kinds of CV?

<v-clicks>

- Trigger/Gate
- 1v/Octave
- CV
- Audio

</v-clicks>

---
layout: center
---

# Everything is voltage!

---

# Everything is voltage

- Jedes Signal im Modular Synth ist elektrische Spannung
- Einzige Unterschiede:
  - Geschwindigkeit des Signals **(Frequenz)**
  - Stärke des Signals **(Amplitude)**
- **< 20Hz**: Steuerspannung, nicht hörbar, oft unipolar _(0-12v)_
- **\> 20Hz**: hörbare Frequenz, bipolar _(-5v - 5v)_
- Alle Signale kann man summieren, skalieren, verschieben, quantisieren etc.
- Rhythmen können als Oszillator genutzt werden
- Audio Signale können als Steuerspannung genutzt werden

<!--
- Andere Ideen:
  - Audio → Sample & Hold → 1v/Octave
  - Noise (Audio) → Filter Frequency Modulation
  - Maths!
-->

---
layout: center
---

# Euclidian Melodies

---

# Euclidian Melodies

- Trigger/Gates nicht für Rhythmen verwenden, sondern für Melodien
- Modulare Konzepte nutzen, um auf neue Ideen zu kommen
- Gates/Trigger erzeugen rhythmisches CV
- CV bei Gate oft 5v, ansonsten 0v
- Stärke von CV kann skaliert werden, um musikalische Noten wiederzugeben:
  - 1 Volt = 1 Oktave
  - Beispiel: Step mit Hit C5, Step ohne Hit C4
- Mehrere Rhythmen können unterschiedlich skaliert und miteinander kombiniert werden, um Melodien erzeugen
- Vor allem interessant bei verschiedenen Rhythmen mit unterschiedlichen Taktlängen
- Melodie kann von Rhythmus getrennt werden

---
layout: image
image: /images/em1.png
backgroundSize: 54rem
---

---
layout: image
image: /images/em2.png
backgroundSize: 54rem
---

---
layout: image
image: /images/em3.png
backgroundSize: 54rem
---

---
layout: image
image: /images/em4.png
backgroundSize: 54rem
---

---
layout: image
image: /images/em5.png
backgroundSize: 54rem
---

---
layout: image
image: /images/em6.png
backgroundSize: 54rem
---

---
layout: center
---

# Insert bleep bloops here

---

# Beyond Euclidian Melodies

- Andere Rhythmen _(z.B. mit Step Sequencer)_ für Melodiegenerierung nutzen
- Wiederholende Sequenzen algorithmisch mutieren

---

# Footnotes

- **\[1\]** Wikipedia "Euclidian Rhythm": https://en.wikipedia.org/wiki/Euclidean_rhythm
- **\[2\]** Paper _Godfried Toussaint - “The Euclidean Algorithm Generates Traditional Musical Rhythms”_: https://cgm.cs.mcgill.ca/~godfried/publications/banff.pdf
- **\[3\]** Browser Visualisierung: https://dbkaplun.github.io/euclidean-rhythm/
- **\[4\]** Workshop Rack: https://modulargrid.net/e/racks/view/2815388

---
layout: image
image: /images/qrcode.png
backgroundSize: 20rem
---

<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />

<center>https://itscursedphil.github.io/euclidian-melodies-workshop/</center>
