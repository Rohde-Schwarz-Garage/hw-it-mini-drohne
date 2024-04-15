# Einrichten Fernbedienung

## Einlegen der Batterien und Aktivieren der selbstständigen Zentrierung

Nach dem Entfernen der gummierten Griffschalen kannst du die mit einem Torx 7 oder 2mm Innensechskantschlüssel die Selbstständige Zentrierung des Schubreglers aktivieren. Drehe hierfür die markierte Schraube entgegen dem Uhrzeigersinn bis sich der dazugehörige Gimbal federgestützt in der Mittelposition hält.

Nun kannst du die zwei 18650 Li-Ion Batterien einlegen. Achte dabei auf die **korrekte Polung**, wie sie in dem Bild markiert ist.

![Image](/rsc/01_img/03_RemoteSetup/RemoteBatteries.png)


## Übersicht der wichtigen Tasten

In der Anleitung wirst du nicht alle Tasten brauchen, aber es ist nützlich, sich einen groben Überblick über die allgemeinen Funktionen zu verschaffen:

![Image](/rsc/01_img/03_RemoteSetup/RemoteManual.png)


## Einrichten Fernbedienung

Damit die Fernbedienung das tut, was du möchtest, muss sie konfiguriert werden. Die nötigen Konfigurationen liegen schon auf dem PC, die folgenden Schritte zeigen dir, wie du diese auf die Fernbedienung ziehen kannst.

Schalte den PC und die Fernbedienung an.

Als Nächstes nimmst du das USB-C Kabel und verbindest den PC und die Fernbedienung miteinander. Achte darauf, dass du das Kabel oben bei der Fernbedienung einsteckst.

Beim Einstecken sollte ein Fenster mit drei verschiedenen Auswahlmöglichkeiten erscheinen. Wähle mit dem Drehrad rechts die Option „USB-Storage“ und drücke das Drehrad. Wenn du versehentlich etwas anderes ausgewählt hast, steck das Kabel einfach wieder ein und aus und wiederhole den Vorgang

![Image](/rsc/01_img/03_RemoteSetup/RemoteUSB.png)

Klicke [hier](/rsc/03_software/02_edgetx) und lade dir den Ordner 02_edgetx herunter.  Markiere nun alle darin enthaltenen Ordner kopiere alles (STRG+C oder Rechtsklick -> Kopiersymbol).

Wähle nun links unten das USB-Laufwerk der Fernbedienung aus.

![Image](/rsc/01_img/03_RemoteSetup/RemoteDrive.png)

Dort siehst du die gleichen Ordner wie auf dem Desktop. Füge die in kopierten Ordner nun ein (STRG+V oder Rechtsklick -> Einfüge Symbol). Sollte ein Fenster für das Ersetzen der Dateien auftauchen, wähle „Dateien im Ziel ersetzen“.

![Image](/rsc/01_img/03_RemoteSetup/RemoteReplace.png)
Warte nun, bis der Vorgang abgeschlossen wurde.

Glückwunsch, du hast die benötigte Konfiguration auf die Fernbedienung übertragen. Im weiteren Verlauf wirst du nun einige Zusatzeinstellungen vornehmen.

## Konfiguration Übertragungsmodul

Damit sich die Fernbedienung mit der Drohne verbinden kann, müssen wir das Übertragungsmodul konfigurieren.

Solltest du an irgendeinem Punkt nicht weiterkommen liegt es möglicherweise an nicht installierten Treibern. In diesem Fall gehst du vor wie in 1.4.1 beschrieben und installierst die Treiber per *Zadig*.

Zuerst starten wir die Fernbedienung mit einem langen Druck auf den Power Button bis das *EdgeTX*-Logo erscheint. Verbinde anschließend die Fernbedienung per USB-Kabel mit dem PC. Nimm dazu den oberen Anschluss an der Fernbedienung.

Es sollte dann folgende Anzeige auf der Fernbedienung erscheinen. Wähle mit dem Drehrad durch Drehen *USB-Serial (VCP)* (1) aus und bestätige durch Drücken des Drehrads.

![Image](/rsc/01_img/03_RemoteSetup/RemoteUSBSerial.png)




## [Klicke hier, um zurück zur Übersicht der Kapitel zu kommen!](/README.md#kapitel)