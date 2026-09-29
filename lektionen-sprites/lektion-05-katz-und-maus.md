# Lektion 5 – Katz und Maus: „falls … sonst“ 🐱🐭

**Zeit:** etwa 50 Minuten

## Was du lernst

Heute lernst du **„falls … dann … sonst“**. Damit hat deine Figur **zwei
Wege**: einen, wenn die Bedingung stimmt, und einen anderen, wenn sie **nicht**
stimmt. Zusammen mit der Schleife wird die Figur **selbstständig**.

## Was du brauchst

- mBlock auf Deutsch (siehe **[Vorbereitung](00-vorbereitung.md)**).
- Die Katze als Figur.
- Deine Maus (oder das Touchpad) als „Beute“.

## Die neue Idee: sonst

Stell dir vor, du sagst:
*„**Falls** es regnet, **dann** bleibe ich drinnen, **sonst** gehe ich
raus.“*

Es passiert **immer genau eins** von beiden. Nie beides, nie keins.

Bei „falls … dann“ (Lektion 4) hat die Figur bei „falsch“ **nichts** getan.
Mit **„sonst“** tut sie dann etwas **anderes**.

## Schritt für Schritt

Die Katze läuft **immer** auf den Mauszeiger zu. **Falls** sie ihn berührt,
**dann** ruft sie „Gefangen!“, **sonst** läuft sie weiter.

1. Kategorie **Ereignisse** → **„wenn grüne Flagge angeklickt“** in die Mitte.

2. Kategorie **Steuerung** → **„wiederhole fortlaufend“** darunter.

3. Kategorie **Steuerung** → **„falls < > dann … sonst …“** **in die
   Schleife**. (Das ist der Block mit **zwei** Öffnungen.)

4. Kategorie **Fühlen** → **„wird (Mauszeiger) berührt?“** in die spitze
   Lücke bei „falls“.

5. **Dann-Teil** (die Katze hat die Maus): Kategorie **Aussehen** →
   **„sage (Gefangen!) für (1) Sekunden“** in die **obere** Öffnung.

6. **Sonst-Teil** (die Katze jagt noch): Kategorie **Bewegung** →
   **„richte dich zu (Mauszeiger) aus“** in die **untere** Öffnung, und
   direkt darunter **„gehe (5) er Schritt“**.

## Dein fertiges Programm

```
wenn grüne Flagge angeklickt
  wiederhole fortlaufend
    falls <wird [Mauszeiger] berührt?> dann
      sage [Gefangen!] für (1) Sekunden
    sonst
      richte dich zu [Mauszeiger] aus
      gehe (5) er Schritt
```

## Probier es aus!

Klicke auf die grüne **Fahne** 🏁 und bewege die Maus über die Bühne. Die
Katze **jagt** den Mauszeiger! Erwischt sie ihn, ruft sie **„Gefangen!“**.
Bewege die Maus schnell weg – dann läuft sie wieder hinterher. 🎉

Zum Beenden: roter **Stopp** ⏹️.

## Was ist passiert?

Die Schleife hat **immer wieder** gefragt: „Berühre ich den Mauszeiger?“

- **Ja** → die Katze ruft „Gefangen!“ (der „dann“-Weg).
- **Nein** → sie dreht sich zur Maus und macht 5 Schritte (der „sonst“-Weg).

So entscheidet die Katze **ganz allein**, was sie tut – du musst nichts
drücken. Das ist die Grundidee hinter jedem Spiel und jedem Roboter, der
selbstständig handelt.

> **Übrigens:** Beim mBot funktioniert das genauso. Dort fragt der Roboter
> den Ultraschallsensor: „Ist ein Hindernis vor mir?“ – und entscheidet dann
> zwischen Ausweichen und Weiterfahren. Schau dir die
> **[mBot-Lektionen](../lektionen-mbot/README.md)** an!

## Kleine Herausforderung 🌟

- Mach die Katze **schneller** oder **langsamer**, indem du die Schrittzahl
  änderst. Was ist besser zum Spielen?
- Lass die Katze zusätzlich **„Miau“** spielen, wenn sie die Maus fängt.

## Geschafft! 🏆

Du kennst jetzt die fünf wichtigsten Bausteine: **Befehle nacheinander**,
**Bewegung**, **Schleifen**, **Bedingungen** und **„falls … sonst“**. Damit
kannst du schon richtige kleine Spiele bauen. Bravo!
