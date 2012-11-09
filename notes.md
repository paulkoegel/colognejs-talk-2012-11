Solitaire mit Backbone
======================

Vorstellen
----------

Live Demo
---------
- 2 Rommee-Kartensets
- Stapel unsichtbar (Counter bei 'Hit me'-Button)
- Drag &amp; Drop, nur offene Karten
- alternierende Kartenfarbe (nicht suit), absteigende Werte
- Asse mit Doppelklick ablegen, dann 2 usw. ablegen
- wenn's nicht weiter geht: 'Hit me'
- Könige auf leere Spalten legen
- oberste Karten von Ablegestapeln können wieder zurück aufs Spielfeld geholt werden
- Ziel: alle Karten unten ablegen
- Spiel speichern und laden

Komponenten
-----------
- Rails: liefert nur Bilder und App Code aus.
- Gründe für Backbone:
  - besser dokumentiert als Ember, viele Plugins und Forenposts, Erfahrungsberichte
  - Spielprojekt

Backbone Relational
-------------------

- ColumnsCollection - Column: unidirektional
- Column - Card: bidirektional
