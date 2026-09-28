# Lektion 3 – Immer wieder! Die Schleife 🔁

**Zeit:** etwa 45 Minuten

## Was du lernst

Heute lernst du einen der besten Tricks beim Programmieren: die **Schleife**.
Eine Schleife wiederholt Befehle für dich – du musst sie nur **einmal**
hinschreiben. Das spart eine Menge Arbeit!

## Was du brauchst

- Deinen mBot, verbunden (siehe **[Vorbereitung](00-vorbereitung.md)**).
- Etwas Platz auf dem Boden.

## Die neue Idee: die Schleife

Erinnerst du dich an das Viereck aus Lektion 2? Wir haben „fahren + drehen“
**viermal** untereinander gesteckt. Das war viel Arbeit und die Blöcke waren
riesig.

Eine **Schleife** ist wie ein Zauberkasten: Du legst Befehle hinein und sagst
*„mach das 4-mal“* – und der Roboter wiederholt sie ganz von allein.

Denk an ein Lied mit einem Refrain: Du singst den Refrain nicht neu, du sagst
einfach *„und jetzt noch dreimal von vorn!“*. Genau das macht eine Schleife.

Es gibt zwei nützliche Schleifen:

- **„wiederhole ( ) mal“** – wiederholt genau so oft, wie du sagst (z. B. 4-mal).
- **„wiederhole fortlaufend“** – wiederholt **für immer**, bis du das Programm
  stoppst.

## Schritt für Schritt (Teil 1: das Viereck – jetzt mit Schleife)

1. Kategorie **Ereignisse** → **„wenn mBot startet“** in die Mitte ziehen.

2. Kategorie **Steuerung** → Ziehe **„wiederhole ( ) mal“** darunter. Schreibe
   eine **4** hinein. Dieser Block hat eine **Öffnung**, in die andere Blöcke
   hineinkommen (wie eine Klammer, die sie umarmt).

3. Kategorie **Aktion** → Ziehe **„fahre (vorwärts) mit Tempo (50)% für (1) Sek.“**
   **in die Öffnung** der Schleife hinein.

4. Kategorie **Aktion** → Ziehe **„fahre (nach rechts drehen) mit Tempo (50)% für
   (0.5) Sek.“** direkt darunter, ebenfalls **innerhalb** der Schleife.

Das war's! Nur **zwei** Fahr-Blöcke statt acht.

```
wenn mBot startet
  wiederhole (4) mal
    fahre (vorwärts) mit Tempo (50)% für (1) Sek.
    fahre (nach rechts drehen) mit Tempo (50)% für (0.5) Sek.
```

Probiere es aus (Live-Modus, verbunden, auf **„wenn mBot startet“** klicken).
Der mBot fährt wieder ein Viereck – aber dein Programm ist **viel kürzer**! 🎉

## Schritt für Schritt (Teil 2: die Disco-Schleife 🪩)

Jetzt bauen wir etwas, das **für immer** läuft: eine Blink-Disco.

1. Kategorie **Ereignisse** → nimm einen **neuen** Block **„wenn mBot startet“**
   (zieh ihn an eine freie Stelle, weg vom Viereck-Programm).

2. Kategorie **Steuerung** → Ziehe **„wiederhole fortlaufend“** darunter.

3. In die Öffnung steckst du nacheinander (alle aus **Licht & Ton** bzw.
   **Steuerung**):
   - **„alle eingebauten LEDs leuchten in der Farbe [Rot]“**
   - **„warte (0.3) Sekunden“**
   - **„alle eingebauten LEDs leuchten in der Farbe [Blau]“**
   - **„warte (0.3) Sekunden“**

```
wenn mBot startet
  wiederhole fortlaufend
    alle eingebauten LEDs leuchten in der Farbe [Rot]
    warte (0.3) Sekunden
    alle eingebauten LEDs leuchten in der Farbe [Blau]
    warte (0.3) Sekunden
```

Klicke auf diesen Start-Block. Dein mBot blinkt jetzt **rot–blau–rot–blau …**
ohne Ende. 🔴🔵

> **Wie stoppe ich das wieder?** Klicke oben auf das rote **Stopp-Zeichen** ⏹️.
> Bei einer „fortlaufend“-Schleife hört der Roboter sonst nicht auf.

## Was ist passiert?

Die Schleife hat die Befehle **immer wieder** ausgeführt, ohne dass du sie
mehrfach hinschreiben musstest. Bei „wiederhole 4 mal“ hörte sie nach 4 Runden
auf. Bei „wiederhole fortlaufend“ läuft sie weiter, bis **du** auf Stopp
drückst.

Merke dir: **Wenn du dich beim Programmieren wiederholst, brauchst du wahr-
scheinlich eine Schleife.**

## Kleine Herausforderung 🌟

- Mach aus der Disco eine **echte Tanz-Party**: Lass den mBot in der
  fortlaufenden Schleife nicht nur blinken, sondern auch kurz **vor- und
  zurückfahren** oder sich **hin- und herdrehen**.
- Baue mit **„wiederhole ( ) mal“** einen mBot, der genau **10-mal** piept –
  wie ein Countdown.

## Nächste Lektion

Bis jetzt macht der mBot immer genau das, was du vorher festgelegt hast. In
**[Lektion 4](lektion-04-sensoren-und-bedingungen.md)** bekommt er einen
**Sinn**: Mit einem **Sensor** kann er die Welt „fühlen“ und **selbst
entscheiden**, was zu tun ist.
