# Lektion 4 – Der mBot fühlt: Sensoren und „falls … dann“ 👀

**Zeit:** etwa 50 Minuten

## Was du lernst

Heute bekommt dein mBot einen **Sinn**! Mit dem **Ultraschallsensor** kann er
messen, wie weit ein Hindernis entfernt ist – fast wie eine Fledermaus, die im
Dunkeln „sieht“.

Und du lernst die zweite große Idee beim Programmieren: die **Bedingung**, den
Block **„falls … dann“**. Damit kann der Roboter **selbst entscheiden**, was zu
tun ist.

## Was du brauchst

- Deinen mBot, verbunden (siehe **[Vorbereitung](00-vorbereitung.md)**).
- Den **Ultraschallsensor** – das ist das Teil vorne am mBot, das aussieht wie
  **zwei Augen**. Er ist meistens am **Anschluss 3** eingesteckt. Prüfe kurz, ob
  er fest sitzt.

## Die neue Idee: der Sensor und die Bedingung

Ein **Sensor** ist ein Teil, mit dem der Roboter etwas über die Welt erfährt.
Der Ultraschallsensor misst die **Entfernung** zum nächsten Hindernis in
Zentimetern (cm). Hältst du deine Hand nah davor, ist die Zahl klein. Ist alles
weit weg, ist die Zahl groß.

Eine **Bedingung** ist eine Frage mit „Ja oder Nein“:

> *Falls* ein Hindernis näher als 15 cm ist, *dann* piepse.

Das kennst du aus dem echten Leben:
*„**Falls** es regnet, **dann** nimm einen Regenschirm.“*
Wenn es nicht regnet, machst du nichts. Genau so ist der **„falls … dann“**-Block:
Er führt die Befehle darin **nur aus, wenn die Frage mit Ja beantwortet wird**.

## Zuerst: den Sensor testen

Bevor wir programmieren, schauen wir uns die Zahl des Sensors an:

1. Kategorie **Sensoren** → Suche den Block
   **„Ultraschallsensor Anschluss (3) Entfernung (cm)“**.
2. Setze **kein** Programm zusammen, sondern **klicke einfach direkt auf diesen
   Block**. Es erscheint eine kleine Zahl – das ist die Entfernung!
3. Halte deine Hand vor die „Augen“ und klicke wieder. Die Zahl wird **kleiner**.
   Nimm die Hand weg und klicke: Die Zahl wird **größer**. Cool, oder?

So findest du heraus, welche Zahl „nah“ bedeutet. Meistens ist alles unter etwa
**15 cm** ziemlich nah.

## Schritt für Schritt

Wir bauen einen mBot, der **piept und rot leuchtet**, sobald du die Hand (oder
eine Wand) davor hältst.

1. Kategorie **Ereignisse** → **„wenn mBot startet“** in die Mitte ziehen.

2. Kategorie **Steuerung** → **„wiederhole fortlaufend“** darunter. (Der mBot
   soll **die ganze Zeit** aufpassen, deshalb eine Dauerschleife.)

3. Kategorie **Steuerung** → Ziehe **„falls < > dann“** **in** die fortlaufende
   Schleife. Der Block hat vorne eine **sechseckige Lücke < >** – dort kommt
   unsere Frage hinein.

4. Jetzt bauen wir die Frage „Ist es näher als 15 cm?“:
   - Kategorie **Operatoren** → Ziehe den Block **„( ) < ( )“** in die
     sechseckige Lücke des „falls“-Blocks.
   - Kategorie **Sensoren** → Ziehe
     **„Ultraschallsensor Anschluss (3) Entfernung (cm)“** in das **linke** Feld
     des „<“-Blocks.
   - In das **rechte** Feld schreibst du **15**.
   - Zusammen liest sich das: **falls Ultraschall-Entfernung < 15 dann**.

5. In die Öffnung des „falls … dann“ kommen die Befehle, die **nur bei einem
   Hindernis** passieren sollen:
   - Kategorie **Licht & Ton** → **„alle eingebauten LEDs leuchten in der Farbe
     [Rot]“**.
   - Kategorie **Licht & Ton** → **„spiele die Note (C4) für (0.25) Schläge“**.

## Dein fertiges Programm

```
wenn mBot startet
  wiederhole fortlaufend
    falls < (Ultraschallsensor Anschluss (3) Entfernung (cm)) < (15) > dann
      alle eingebauten LEDs leuchten in der Farbe [Rot]
      spiele die Note (C4) für (0.25) Schläge
```

## Probier es aus!

**Live**-Modus, mBot **verbunden**, auf **„wenn mBot startet“** klicken.

Halte langsam deine Hand vor die „Augen“ des mBot: Er **leuchtet rot und
piept**! Nimm die Hand weg – er wird ruhig. Bewege die Hand hin und her und
der mBot reagiert wie ein kleiner Wächter. 🚨

Zum Beenden oben auf **Stopp** ⏹️ klicken.

## Was ist passiert?

Die **fortlaufende Schleife** hat dafür gesorgt, dass der mBot **immer wieder
nachschaut**. Jedes Mal hat der **„falls“**-Block die Frage gestellt:
*„Ist etwas näher als 15 cm?“* Nur wenn die Antwort **Ja** war, hat er geleuchtet
und gepiepst. War die Antwort **Nein**, hat er die Befehle übersprungen.

Das ist der Moment, in dem dein Roboter anfängt, **selbst zu entscheiden**!

## Kleine Herausforderung 🌟

- Lass den mBot **grün** leuchten, wenn nichts in der Nähe ist. Tipp: Du kannst
  auch einen Farb-Block **außerhalb** (direkt über) dem „falls“-Block einbauen –
  er leuchtet dann standardmäßig grün und wird nur bei einem Hindernis rot.
- Ändere die **15** in eine andere Zahl und finde heraus, ab welcher Entfernung
  der mBot reagieren soll.

## Nächste Lektion

Jetzt kann dein mBot fühlen **und** entscheiden. In der letzten Lektion bringen
wir alles zusammen: In **[Lektion 5](lektion-05-selbststaendig-fahren.md)** fährt
dein mBot **ganz allein** durch den Raum und **weicht Hindernissen aus** – wie
ein echter Roboter-Staubsauger!
