# Lektion 5 – Ganz allein fahren: der Hindernis-Ausweicher 🤖🚧

**Zeit:** etwa 60 Minuten

## Was du lernst

Das ist die große Lektion, in der **alles zusammenkommt**! Dein mBot wird zu
einem echten kleinen Roboter, der **von allein** durch den Raum fährt und
**Hindernissen ausweicht**.

Du lernst die Erweiterung der Bedingung: **„falls … dann … sonst“**. Damit sagst
du dem Roboter: *„Mach das Eine, **sonst** mach das Andere.“* Und du kombinierst
zum ersten Mal **Sensor + Bedingung + Bewegung + Schleife** in einem Programm.

## Was du brauchst

- Deinen mBot mit **Ultraschallsensor** (Anschluss 3), verbunden.
- **Viel Platz auf dem Boden** und ein paar Hindernisse (Bücher, Kartons, eine
  Wand). Am besten kein Tisch – der mBot fährt jetzt frei herum!

## Die neue Idee: „falls … dann … sonst“

In Lektion 4 hast du gelernt: *„**Falls** es regnet, **dann** nimm einen
Schirm.“* Aber was, wenn es **nicht** regnet? Dann willst du vielleicht die
Sonnenbrille nehmen:

> *„**Falls** es regnet, **dann** nimm den Schirm, **sonst** nimm die Sonnenbrille.“*

Der Block **„falls … dann … sonst“** hat deshalb **zwei** Fächer:
- Das obere Fach (**dann**) läuft, wenn die Antwort **Ja** ist.
- Das untere Fach (**sonst**) läuft, wenn die Antwort **Nein** ist.

Für unseren Roboter heißt das:

> **Falls** ein Hindernis nah ist → **dann** ausweichen (drehen).
> **Sonst** (der Weg ist frei) → einfach **weiterfahren**.

## So denkt unser Roboter

Bevor wir bauen, sagen wir den Plan in einfachen Worten (das nennt man den
**Ablauf**):

```
Immer wieder:
    Schau nach vorne.
    Ist ein Hindernis näher als 15 cm?
        JA  -> anhalten, rückwärts, dann wegdrehen
        NEIN -> weiter geradeaus fahren
```

## Schritt für Schritt

1. Kategorie **Ereignisse** → **„wenn mBot startet“** in die Mitte ziehen.

2. Kategorie **Steuerung** → **„wiederhole fortlaufend“** darunter. Der Roboter
   soll ja **die ganze Zeit** fahren und aufpassen.

3. Kategorie **Steuerung** → Ziehe **„falls < > dann … sonst“** in die
   fortlaufende Schleife. (Achte darauf, dass es der Block mit **zwei** Fächern
   ist – mit dem Wort **„sonst“** in der Mitte.)

4. Baue wieder die Frage in die sechseckige Lücke (genau wie in Lektion 4):
   - **Operatoren** → **„( ) < ( )“** in die Lücke.
   - **Sensoren** → **„Ultraschallsensor Anschluss (3) Entfernung (cm)“** ins
     linke Feld.
   - **15** ins rechte Feld.

5. In das **obere Fach („dann“)** kommt das **Ausweichen** (alle aus **Aktion**,
   der Warte-Block aus **Steuerung**):
   - **„anhalten“**
   - **„fahre (rückwärts) mit Tempo (40)% für (0.5) Sek.“**
   - **„fahre (nach rechts drehen) mit Tempo (40)% für (0.6) Sek.“**

6. In das **untere Fach („sonst“)** kommt das **Weiterfahren**:
   - **Aktion** → **„fahre (vorwärts) mit Tempo (40)% für (0.2) Sek.“**

   > **Warum nur 0.2 Sekunden?** So fährt der mBot immer nur ein kleines Stück
   > und schaut dann sofort wieder nach. Dadurch merkt er Hindernisse früh genug
   > und fährt nicht mit Vollgast dagegen.

## Dein fertiges Programm

```
wenn mBot startet
  wiederhole fortlaufend
    falls < (Ultraschallsensor Anschluss (3) Entfernung (cm)) < (15) > dann
      anhalten
      fahre (rückwärts) mit Tempo (40)% für (0.5) Sek.
      fahre (nach rechts drehen) mit Tempo (40)% für (0.6) Sek.
    sonst
      fahre (vorwärts) mit Tempo (40)% für (0.2) Sek.
```

## Probier es aus!

Stell den mBot auf den **Boden** in einen freien Bereich. **Live**-Modus, mBot
**verbunden**, auf **„wenn mBot startet“** klicken.

Dein mBot fährt los! Kommt er einer Wand oder einem Buch zu nah, **hält er an,
fährt zurück und dreht weg** – und sucht sich einen neuen Weg. Er fährt ganz
**allein**! 🎉🎉

Zum Stoppen oben auf **Stopp** ⏹️ klicken.

### Bonus: ohne Kabel fahren lassen

Wenn dein Programm gut läuft, mach es zum echten freien Roboter:

1. Stelle oben von **Live** auf **Hochladen** um.
2. Klicke auf **„Hochladen“** und warte, bis es fertig ist.
3. Zieh das **USB-Kabel ab**. Der mBot fährt jetzt **ganz ohne Computer** los –
   du kannst ihn frei durch das Zimmer fahren lassen! 🏠

## Was ist passiert?

Du hast zum ersten Mal **alles kombiniert**, was du gelernt hast:

- Die **Schleife** lässt den mBot immer wieder nachdenken (Lektion 3).
- Der **Sensor** misst die Entfernung (Lektion 4).
- Die Bedingung **„falls … dann … sonst“** entscheidet zwischen **ausweichen**
  und **weiterfahren**.
- Die **Fahr-Befehle** bewegen den Roboter (Lektion 2), alle **nacheinander**
  in der richtigen Reihenfolge (Lektion 1).

Das ist echtes Roboter-Programmieren. Genau so funktionieren auch große Roboter,
selbstfahrende Autos und Staubsauger-Roboter – nur mit mehr Sensoren.

## Kleine Herausforderung 🌟

- Lass den mBot beim Ausweichen **rot leuchten und piepen**, damit man merkt:
  „Achtung, Hindernis!“
- Manchmal soll der mBot mal nach **links**, mal nach **rechts** ausweichen.
  Suche in der Kategorie **Operatoren** den Block **„Zufallszahl von ( ) bis ( )“**
  und überlege, wie du damit die Drehrichtung überraschend machen kannst.
- Baue eine kleine **Arena** aus Büchern und schau zu, wie sich der mBot allein
  darin zurechtfindet.

## Geschafft! 🏆

Du hast alle fünf Lektionen gemeistert! Du kennst jetzt die wichtigsten Ideen
beim Programmieren:

- **Befehle nacheinander** (Sequenz)
- **Ereignisse** (wann etwas losgeht)
- **Bewegung** mit Einstellungen (Tempo, Zeit)
- **Schleifen** (Wiederholungen)
- **Sensoren** (fühlen)
- **Bedingungen** „falls … dann … sonst“ (entscheiden)

Mit diesen Bausteinen kannst du schon **eine Menge** eigener Roboter-Programme
erfinden. Trau dich, weiter zu experimentieren – jetzt bist du ein
Roboter-Programmierer! 🤖✨

*Es gibt noch mehr zu entdecken (Variablen, der Linienfolge-Sensor, eigene
Blöcke …). Weitere Lektionen folgen – bleib dran!*
