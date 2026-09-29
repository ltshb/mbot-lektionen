# Lektion 2 – Die Figur bewegt sich 🐱➡️

**Zeit:** etwa 40 Minuten

## Was du lernst

Heute lernst du, deine Figur zu **bewegen**: vorwärts gehen, sich **drehen**
und an eine bestimmte Stelle springen. Die Zahlen in den Blöcken (die
**Parameter**) bestimmen, **wie weit** und **wie stark**.

## Was du brauchst

- mBlock auf Deutsch (siehe **[Vorbereitung](00-vorbereitung.md)**).
- Eine Figur auf der Bühne.

## Die neue Idee: Bewegung mit Zahlen

Stell dir vor, du spielst „Schatzsuche“ und sagst einem Freund:
*„Geh 10 Schritte geradeaus, dreh dich nach rechts, geh 5 Schritte.“*

Die **Zahlen** sind wichtig: 10 Schritte sind weiter als 2 Schritte. Auch bei
der Drehung: **90 Grad** ist eine Vierteldrehung (wie eine Ecke im Zimmer),
**180 Grad** ist eine halbe Drehung, also einmal umdrehen.

## Schritt für Schritt

Wir lassen die Katze ein **Viereck** laufen.

1. Kategorie **Ereignisse** → **„wenn grüne Flagge angeklickt“** in die Mitte
   ziehen.

2. Kategorie **Bewegung** → **„gehe zu x: ( ) y: ( )“** darunter. Schreibe
   **-100** und **-50**. So startet die Katze immer an derselben Stelle.

3. Kategorie **Bewegung** → **„setze Richtung auf ( ) Grad“** darunter, mit
   **90** (die Katze schaut nach rechts).

4. Kategorie **Bewegung** → **„gehe ( ) er Schritt“** darunter. Schreibe
   **100**.

5. Kategorie **Bewegung** → **„drehe dich nach rechts ( ) Grad“** darunter.
   Schreibe **90**.

6. Wiederhole Schritt 4 und 5 noch **dreimal**, sodass du vier Mal „gehen“
   und vier Mal „drehen“ hast. (Kopieren geht schnell: mit der rechten
   Maustaste auf einen Block klicken und **„Duplizieren“** wählen.)

7. Kategorie **Steuerung** → Füge zwischen die Bewegungen jeweils
   **„warte (0.5) Sekunden“** ein, damit du zuschauen kannst.

## Dein fertiges Programm

```
wenn grüne Flagge angeklickt
  gehe zu x: (-100) y: (-50)
  setze Richtung auf (90) Grad
  gehe (100) er Schritt
  warte (0.5) Sekunden
  drehe dich nach rechts (90) Grad
  gehe (100) er Schritt
  warte (0.5) Sekunden
  drehe dich nach rechts (90) Grad
  gehe (100) er Schritt
  warte (0.5) Sekunden
  drehe dich nach rechts (90) Grad
  gehe (100) er Schritt
  warte (0.5) Sekunden
  drehe dich nach rechts (90) Grad
```

## Probier es aus!

Klicke auf die grüne **Fahne** 🏁. Die Katze springt nach links unten und
läuft ein **Viereck**. Prima! 🎉

> **Tipp:** Klappt das Viereck nicht ganz? Prüfe, ob du überall **90** und
> überall dieselbe Schrittzahl eingetragen hast.

## Was ist passiert?

Die Figur hat jeden Befehl der Reihe nach ausgeführt. Die **Zahlen** haben
bestimmt, wie weit sie geht und wie stark sie sich dreht. Vier Mal
Vierteldrehung (4 × 90 Grad) ergibt eine ganze Drehung – darum kommt die
Katze wieder am Anfang an.

## Kleine Herausforderung 🌟

- Lass die Katze ein **Dreieck** laufen. Tipp: Die Drehung ist dann nicht 90
  Grad, sondern **120** Grad, und du brauchst nur 3 Seiten.
- Lass sie beim Laufen **sagen**, wo sie gerade ist.

## Nächste Lektion

Dein Viereck war ganz schön lang, oder? In **[Lektion 3](lektion-03-wiederholungen.md)**
lernst du einen Trick, mit dem das Programm **viel kürzer** wird: die
**Schleife**.
