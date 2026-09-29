# Lektion 4 – Die Figur fühlt: „falls … dann“ 🤔

**Zeit:** etwa 45 Minuten

## Was du lernst

Heute lernst du, wie deine Figur **Entscheidungen** trifft. Mit dem Block
**„falls … dann“** tut sie etwas nur dann, **wenn** etwas Bestimmtes
stimmt – zum Beispiel, wenn du eine Taste drückst.

## Was du brauchst

- mBlock auf Deutsch (siehe **[Vorbereitung](00-vorbereitung.md)**).
- Eine Figur auf der Bühne.

## Die neue Idee: Bedingung

Im Alltag entscheidest du ständig:
*„**Falls** es regnet, **dann** nehme ich einen Schirm mit.“*

Das Wort nach „falls“ ist eine **Bedingung**. Sie kann nur **wahr** oder
**falsch** sein: Es regnet – oder es regnet nicht. Ist sie wahr, passiert das,
was im „dann“-Teil steht. Ist sie falsch, wird es übersprungen.

Die Figur hat **Fühler** (in der Kategorie **Fühlen**):

- **„Taste (Leertaste) gedrückt?“**
- **„wird (Mauszeiger) berührt?“**
- **„wird Rand berührt?“**

Diese Blöcke haben eine spitze Form. Sie passen in die spitze Lücke von
**„falls … dann“**.

## Der Trick mit der Schleife

Eine Bedingung wird nur **einmal** geprüft – genau in dem Moment, in dem das
Programm sie erreicht. Damit die Figur **immer wieder** aufpasst, stecken wir
„falls … dann“ in eine **„wiederhole fortlaufend“**-Schleife (die kennst du
aus Lektion 3).

## Schritt für Schritt

Die Katze **bewegt sich nach rechts**, solange du die **Pfeiltaste rechts**
gedrückt hältst, und **miaut**, wenn du die **Leertaste** drückst.

1. Kategorie **Ereignisse** → **„wenn grüne Flagge angeklickt“** in die Mitte.

2. Kategorie **Steuerung** → **„wiederhole fortlaufend“** darunter.

3. Kategorie **Steuerung** → **„falls < > dann“** **in die Schleife**.

4. Kategorie **Fühlen** → **„Taste (Leertaste) gedrückt?“** in die spitze
   Lücke bei „falls“. Klicke auf das Feld und wähle **Pfeil nach rechts**.

5. Kategorie **Bewegung** → **„gehe (10) er Schritt“** in die Öffnung von
   „dann“.

6. Ziehe ein **zweites „falls < > dann“** direkt **unter** das erste (noch in
   der Schleife). Setze **„Taste (Leertaste) gedrückt?“** ein und lass
   **Leertaste** stehen.

7. Kategorie **Klang** → **„spiele Klang (Miau) ganz“** in die Öffnung des
   zweiten „dann“.

## Dein fertiges Programm

```
wenn grüne Flagge angeklickt
  wiederhole fortlaufend
    falls <Taste [Pfeil nach rechts] gedrückt?> dann
      gehe (10) er Schritt
    falls <Taste [Leertaste] gedrückt?> dann
      spiele Klang [Miau] ganz
```

## Probier es aus!

Klicke auf die grüne **Fahne** 🏁. Halte jetzt die **Pfeiltaste rechts**
gedrückt: Die Katze läuft los. Lässt du los, bleibt sie stehen. Drückst du
die **Leertaste**, miaut sie. 🐱

Vergiss nicht, am Ende den roten **Stopp** ⏹️ zu klicken.

## Was ist passiert?

Die Schleife hat **immer wieder** nachgeschaut: „Ist die Taste gedrückt?“
Wenn **ja** (wahr), hat die Katze den „dann“-Teil ausgeführt. Wenn **nein**
(falsch), hat sie nichts getan und sofort wieder nachgeschaut. Das geht so
schnell, dass es dir vorkommt, als würde die Katze sofort reagieren.

## Kleine Herausforderung 🌟

- Baue noch ein „falls“ dazu: **Pfeil nach links** → **„drehe dich nach
  links (5) Grad“**. Jetzt kannst du die Katze steuern!
- Lass die Katze **„Aua!“ sagen**, wenn sie den **Rand** berührt.

## Nächste Lektion

In **[Lektion 5](lektion-05-katz-und-maus.md)** lernst du **„falls … dann …
sonst“** und baust zusammen mit der Schleife ein kleines **Spiel**: Die
Katze jagt den Mauszeiger!
