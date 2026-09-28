# Lektion 2 – Der mBot fährt 🚗

**Zeit:** etwa 45 Minuten

## Was du lernst

Heute bringst du deinen mBot dazu, sich zu **bewegen**: vorwärts fahren,
drehen und anhalten. Dabei lernst du eine wichtige Sache kennen: Manche Blöcke
haben **Felder zum Einstellen** – zum Beispiel **wie schnell** und **wie lange**
der mBot fährt.

## Was du brauchst

- Deinen mBot, verbunden mit dem Computer (siehe **[Vorbereitung](00-vorbereitung.md)**).
- **Platz auf dem Boden!** Am besten ein freier Tisch oder der Fußboden, wo der
  mBot ein Stück fahren kann, ohne herunterzufallen.

> ⚠️ **Achtung:** Lass den mBot nicht von der Tischkante fallen. Auf dem Boden
> ist es am sichersten.

## Die neue Idee: Blöcke mit Einstellungen

In Lektion 1 haben unsere Befehle einfach nur *etwas gemacht*. Fahr-Blöcke sind
schlauer: Du kannst ihnen sagen, **wie schnell** (das nennt man **Tempo**, in
Prozent von 0 bis 100) und **wie lange** (in Sekunden) sie fahren sollen.

Denk an ein Rennauto: Du kannst nicht nur „fahr!“ sagen, sondern auch
„fahr **halb so schnell** und das **2 Sekunden lang**“. Genau diese Zahlen
stellst du in den Feldern der Blöcke ein.

## Schritt für Schritt

Wir lassen den mBot ein **Viereck** abfahren: immer ein Stück geradeaus, dann
eine Vierteldrehung, und das viermal.

1. Kategorie **Ereignisse** → Ziehe **„wenn mBot startet“** in die Mitte.

2. Kategorie **Aktion** → Ziehe
   **„fahre (vorwärts) mit Tempo ( )% für ( ) Sek.“** darunter.
   Stelle das Tempo auf **50** und die Zeit auf **1** Sekunde.

3. Kategorie **Aktion** → Ziehe noch einen Fahr-Block darunter, aber wähle im
   ersten Feld **„nach rechts drehen“** aus. Tempo **50**, Zeit **0.5** Sekunden.
   (Mit 0.5 Sekunden dreht sich der mBot etwa um eine Vierteldrehung – so wie
   die Ecke eines Vierecks. Vielleicht musst du die Zahl später ein bisschen
   anpassen.)

4. Jetzt haben wir **eine Seite und eine Ecke**. Ein Viereck hat vier Seiten.
   Klicke mit der rechten Maustaste auf den Fahr-Block und den Dreh-Block und
   wähle **„Duplizieren“** – oder ziehe einfach noch dreimal die gleichen zwei
   Blöcke dazu, sodass du **viermal** „fahren + drehen“ hast.

5. Zum Schluss soll der mBot anhalten. Kategorie **Aktion** → Ziehe den Block
   **„anhalten“** ganz unten an.

## Dein fertiges Programm

```
wenn mBot startet
  fahre (vorwärts) mit Tempo (50)% für (1) Sek.
  fahre (nach rechts drehen) mit Tempo (50)% für (0.5) Sek.
  fahre (vorwärts) mit Tempo (50)% für (1) Sek.
  fahre (nach rechts drehen) mit Tempo (50)% für (0.5) Sek.
  fahre (vorwärts) mit Tempo (50)% für (1) Sek.
  fahre (nach rechts drehen) mit Tempo (50)% für (0.5) Sek.
  fahre (vorwärts) mit Tempo (50)% für (1) Sek.
  fahre (nach rechts drehen) mit Tempo (50)% für (0.5) Sek.
  anhalten
```

## Probier es aus!

Stell den mBot auf den Boden, sorge für **Live**-Modus und dass er
**verbunden** ist. Klicke auf **„wenn mBot startet“**.

Dein mBot fährt jetzt ein Viereck ab und bleibt am Ende stehen! 🟦

## Was ist passiert?

Der mBot hat vier Mal das Gleiche gemacht: ein Stück fahren, dann drehen. Vier
Seiten, vier Ecken – fertig ist das Viereck. Die **Zahlen** in den Blöcken haben
bestimmt, wie weit er fährt und wie weit er sich dreht.

Ist dein Viereck krumm geworden? Kein Problem! Ändere die **0.5** beim Drehen in
eine etwas größere oder kleinere Zahl, bis die Ecken schön werden. Genau so
arbeiten echte Programmierer: ausprobieren und anpassen.

## Kleine Herausforderung 🌟

- Lass den mBot statt eines Vierecks ein **Dreieck** fahren (Tipp: ein Dreieck
  hat nur **drei** Ecken, und die Drehung muss dann etwas größer sein).
- Oder baue eine **Extra-Runde**: Lass ihn nach dem Viereck **rückwärts** wieder
  zum Start zurückfahren.

## Nächste Lektion

Ist dir aufgefallen, wie oft wir die **gleichen** Blöcke kopiert haben? Das war
ganz schön viel Arbeit! In **[Lektion 3](lektion-03-wiederholungen.md)** lernst
du einen Trick, mit dem der Roboter Dinge **von allein wiederholt** – mit nur
einem einzigen Block.
