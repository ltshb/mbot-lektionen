# Lektion 3 – Immer wieder! Die Schleife 🔁

**Zeit:** etwa 45 Minuten

## Was du lernst

Heute lernst du einen der besten Tricks beim Programmieren: die **Schleife**.
Eine Schleife wiederholt Befehle für dich – du musst sie nur **einmal**
hinschreiben. Das spart eine Menge Arbeit!

## Was du brauchst

- mBlock auf Deutsch (siehe **[Vorbereitung](00-vorbereitung.md)**).
- Eine Figur auf der Bühne.

## Die neue Idee: die Schleife

Erinnerst du dich an das Viereck aus Lektion 2? Wir haben „gehen + drehen“
**viermal** untereinander gesteckt. Das war viel Arbeit.

Eine **Schleife** ist wie ein Zauberkasten: Du legst Befehle hinein und sagst
*„mach das 4-mal“* – und die Figur wiederholt sie ganz von allein.

Denk an ein Lied mit einem Refrain: Du singst den Refrain nicht neu, du sagst
einfach *„und jetzt noch dreimal von vorn!“*.

Es gibt zwei nützliche Schleifen:

- **„wiederhole ( ) mal“** – wiederholt genau so oft, wie du sagst.
- **„wiederhole fortlaufend“** – wiederholt **für immer**, bis du auf Stopp
  drückst.

## Schritt für Schritt (Teil 1: das Viereck – jetzt mit Schleife)

1. Kategorie **Ereignisse** → **„wenn grüne Flagge angeklickt“** in die Mitte.

2. Kategorie **Bewegung** → **„gehe zu x: (-100) y: (-50)“** und
   **„setze Richtung auf (90) Grad“** darunter.

3. Kategorie **Steuerung** → **„wiederhole ( ) mal“** darunter. Schreibe eine
   **4** hinein. Dieser Block hat eine **Öffnung**, in die andere Blöcke
   hineinkommen (wie eine Klammer, die sie umarmt).

4. Kategorie **Bewegung** → **„gehe (100) er Schritt“** **in die Öffnung**.

5. Kategorie **Bewegung** → **„drehe dich nach rechts (90) Grad“** direkt
   darunter, ebenfalls **innerhalb** der Schleife.

Nur **zwei** Bewegungs-Blöcke statt acht!

```
wenn grüne Flagge angeklickt
  gehe zu x: (-100) y: (-50)
  setze Richtung auf (90) Grad
  wiederhole (4) mal
    gehe (100) er Schritt
    drehe dich nach rechts (90) Grad
```

Klicke auf die grüne Fahne 🏁. Die Katze läuft wieder ein Viereck – aber dein
Programm ist **viel kürzer**! 🎉

> **Zu schnell?** Steck **„warte (0.3) Sekunden“** in die Schleife, dann kannst
> du besser zuschauen.

## Schritt für Schritt (Teil 2: der Kreistanz 💃)

Jetzt bauen wir etwas, das **für immer** läuft.

1. Nimm einen **neuen** Block **„wenn grüne Flagge angeklickt“** (an eine freie
   Stelle, weg vom Viereck-Programm).

2. Kategorie **Steuerung** → **„wiederhole fortlaufend“** darunter.

3. In die Öffnung steckst du:
   - **„gehe (10) er Schritt“** (Bewegung)
   - **„drehe dich nach rechts (15) Grad“** (Bewegung)
   - **„wechsle zum nächsten Kostüm“** (Aussehen)
   - **„warte (0.1) Sekunden“** (Steuerung)

```
wenn grüne Flagge angeklickt
  wiederhole fortlaufend
    gehe (10) er Schritt
    drehe dich nach rechts (15) Grad
    wechsle zum nächsten Kostüm
    warte (0.1) Sekunden
```

Die Katze läuft im **Kreis** und bewegt dabei die Beine! 🐱

> **Wie stoppe ich das wieder?** Klicke auf das rote **Stopp-Zeichen** ⏹️.
> Bei einer „fortlaufend“-Schleife hört die Figur sonst nie auf.

## Was ist passiert?

Die Schleife hat die Befehle **immer wieder** ausgeführt. Bei „wiederhole
4 mal“ hörte sie nach 4 Runden auf, bei „fortlaufend“ läuft sie weiter, bis
**du** stoppst. Weil sich die Katze bei jeder Runde ein Stück dreht, ergibt
sich ein Kreis.

Merke dir: **Wenn du dich beim Programmieren wiederholst, brauchst du
wahrscheinlich eine Schleife.**

## Kleine Herausforderung 🌟

- Lass die Katze ein **Sechseck** laufen (6 Seiten, Drehung 60 Grad).
- Baue mit **„wiederhole (10) mal“** eine Katze, die genau 10-mal miaut.

## Nächste Lektion

Bis jetzt macht die Figur immer genau das, was du vorher festgelegt hast. In
**[Lektion 4](lektion-04-fuehlen-und-bedingungen.md)** bekommt sie einen
**Sinn**: Sie kann **fühlen**, ob eine Taste gedrückt wird oder sie etwas
berührt, und **selbst entscheiden**, was sie tut.
