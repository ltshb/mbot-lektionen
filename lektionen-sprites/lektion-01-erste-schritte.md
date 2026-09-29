# Lektion 1 – Erste Schritte: Sprechen und Klingen 💬🎵

**Zeit:** etwa 30 Minuten

## Was du lernst

Heute lernst du die allerwichtigste Idee beim Programmieren:
Ein Programm ist eine **Liste von Befehlen**, die die Figur **nacheinander**
abarbeitet – einen nach dem anderen, von oben nach unten.

Außerdem lernst du das **Start-Ereignis** kennen: den Block, der sagt
*„Hier fängt das Programm an.“*

## Was du brauchst

- mBlock im Browser, auf Deutsch (siehe **[Vorbereitung](00-vorbereitung.md)**).
- Eine Figur auf der Bühne (die Katze reicht).

## Die neue Idee: Befehle nacheinander

Stell dir vor, du erklärst einem kleinen Kind, wie man ein Butterbrot macht:

1. Nimm das Brot.
2. Streiche Butter darauf.
3. Leg es auf den Teller.

Die **Reihenfolge** ist wichtig! Butter zuerst, dann auf den Teller – nicht
andersherum. Genau so ist es bei deiner Figur: Sie macht die Befehle in der
Reihenfolge, in der du sie **untereinander** steckst.

## Schritt für Schritt

Wir bauen ein Programm, bei dem die Katze **Hallo sagt**, kurz **wartet**,
dann etwas anderes sagt und dazu einen **Klang** abspielt.

1. Klicke links auf die Kategorie **Ereignisse**. Ziehe den Block
   **„wenn grüne Flagge angeklickt“** in die weiße Fläche in der Mitte. Das
   ist der Hut, unter dem unser Programm hängt.

2. Klicke auf die Kategorie **Aussehen**. Ziehe den Block
   **„sage ( ) für ( ) Sekunden“** direkt **unter** den Start-Block, sodass er
   einrastet. Schreibe **Hallo! Ich bin die Katze.** in das erste Feld und
   **2** in das zweite.

3. Klicke auf die Kategorie **Steuerung**. Ziehe **„warte ( ) Sekunden“**
   darunter. Schreibe eine **1** in das Feld.

4. Gehe wieder zu **Aussehen**. Ziehe noch einmal
   **„sage ( ) für ( ) Sekunden“** darunter. Schreibe **Miau!** und **1**.

5. Klicke auf die Kategorie **Klang**. Ziehe den Block
   **„spiele Klang ( ) ganz“** darunter und wähle einen Klang aus, zum
   Beispiel **Miau**.

## Dein fertiges Programm

```
wenn grüne Flagge angeklickt
  sage [Hallo! Ich bin die Katze.] für (2) Sekunden
  warte (1) Sekunden
  sage [Miau!] für (1) Sekunden
  spiele Klang [Miau] ganz
```

## Probier es aus!

Klicke auf die grüne **Fahne** 🏁 über der Bühne.

Die Katze sagt zuerst „Hallo!“, wartet, sagt „Miau!“ und miaut wirklich.
(Mach den Ton am Computer an!) Geschafft – dein erstes Programm! 🎉

## Was ist passiert?

Die Figur hat deine Befehle **von oben nach unten** abgearbeitet. Genau wie
beim Butterbrot war die **Reihenfolge** entscheidend. Der Block „wenn grüne
Flagge angeklickt“ war das Signal: *„Jetzt geht's los!“*

## Kleine Herausforderung 🌟

Baue ein kleines **Gespräch**: Die Katze sagt etwas, wartet, sagt etwas
anderes, wartet wieder … Denk dir eine kurze Geschichte aus!

Und trau dich: Ändere die Wörter und die Zahlen und schau, was passiert.

## Nächste Lektion

In **[Lektion 2](lektion-02-die-figur-bewegt-sich.md)** bringen wir die Figur
dazu, sich zu **bewegen** – sie läuft über die Bühne!
