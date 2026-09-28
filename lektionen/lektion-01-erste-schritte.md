# Lektion 1 – Erste Schritte: Licht und Ton 💡🎵

**Zeit:** etwa 30 Minuten

## Was du lernst

Heute lernst du die allerwichtigste Idee beim Programmieren:
Ein Programm ist eine **Liste von Befehlen**, die der Roboter **nacheinander**
abarbeitet – einen nach dem anderen, von oben nach unten.

Außerdem lernst du das **Start-Ereignis** kennen: den Block, der sagt
*„Hier fängt das Programm an.“*

## Was du brauchst

- Deinen mBot, verbunden mit dem Computer (siehe **[Vorbereitung](00-vorbereitung.md)**).
- mBlock auf Deutsch, mit dem Gerät „mBot“.

## Die neue Idee: Befehle nacheinander

Stell dir vor, du erklärst einem kleinen Kind, wie man ein Butterbrot macht:

1. Nimm das Brot.
2. Streiche Butter darauf.
3. Leg es auf den Teller.

Die **Reihenfolge** ist wichtig! Butter zuerst, dann auf den Teller – nicht
andersherum. Genau so ist es bei einem Roboter: Er macht die Befehle in der
Reihenfolge, in der du sie **untereinander** steckst.

## Schritt für Schritt

Wir bauen ein Programm, bei dem der mBot **rot leuchtet**, kurz **wartet**,
dann **grün leuchtet** und dazu einen **Ton** spielt.

1. Klicke links auf die Kategorie **Ereignisse** (das ist die Farbe für den
   Start). Ziehe den Block **„wenn mBot startet“** in die weiße Fläche in der
   Mitte. Das ist der Hut, unter dem unser Programm hängt.

2. Klicke auf die Kategorie **Licht & Ton**. Ziehe den Block
   **„alle eingebauten LEDs leuchten in der Farbe ( )“** direkt **unter** den
   Start-Block, sodass er einrastet. Klicke auf das Farbfeld und wähle **Rot**.

3. Klicke auf die Kategorie **Steuerung**. Ziehe **„warte ( ) Sekunden“**
   darunter. Schreibe eine **1** in das Feld.

4. Gehe wieder zu **Licht & Ton**. Ziehe noch einmal
   **„alle eingebauten LEDs leuchten in der Farbe ( )“** darunter und stelle
   die Farbe auf **Grün**.

5. Bleibe bei **Licht & Ton**. Ziehe den Block
   **„spiele die Note ( ) für ( ) Schläge“** darunter. Lass die Note so, wie
   sie ist, oder wähle eine aus. Schreibe bei den Schlägen **0.5**.

## Dein fertiges Programm

So sieht dein zusammengestecktes Programm aus:

```
wenn mBot startet
  alle eingebauten LEDs leuchten in der Farbe [Rot]
  warte (1) Sekunden
  alle eingebauten LEDs leuchten in der Farbe [Grün]
  spiele die Note (C4) für (0.5) Schläge
```

## Probier es aus!

Achte darauf, dass oben **Live** eingestellt ist und dein mBot **verbunden**
ist. Klicke jetzt oben auf den Block **„wenn mBot startet“** (oder auf die
grüne Fahne, wenn sie da ist).

Dein mBot leuchtet zuerst **rot**, dann nach einer Sekunde **grün** und macht
**„Piep“**. Geschafft – dein erstes Roboter-Programm! 🎉

## Was ist passiert?

Der Roboter hat deine Befehle **von oben nach unten** abgearbeitet:
erst rot, dann warten, dann grün, dann Ton. Genau wie beim Butterbrot war die
**Reihenfolge** entscheidend. Der „wenn mBot startet“-Block war das Signal:
*„Jetzt geht's los!“*

## Kleine Herausforderung 🌟

Kannst du das Programm zu einer kleinen **Ampel** machen?
Rot → warten → Gelb (probiere die Farbe aus) → warten → Grün. Füge dafür
einfach mehr Farb-Blöcke und Warte-Blöcke hinzu.

Und trau dich: Ändere die Zahlen und die Farben und schau, was passiert!

## Nächste Lektion

In **[Lektion 2](lektion-02-der-mbot-faehrt.md)** bringen wir den mBot dazu,
sich zu **bewegen** – er fährt los!
