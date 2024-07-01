# Navigation und Einrichtung Fernbedienung
![image](https://github.com/Rohde-Schwarz-Garage/.github/blob/main/ressources/graphics/2024_03_13_Trennbanner_GitHub_Grey_Transparent.png?raw=true)

## Einlegen der Batterien und Aktivieren der selbstständigen Zentrierung

Nach dem Entfernen der gummierten Griffschalen kannst du mit einem Torx 7 oder 2mm Innensechskantschlüssel die selbstständige Zentrierung des Schubreglers aktivieren. Drehe hierfür die markierte Schraube entgegen dem Uhrzeigersinn bis sich der dazugehörige Gimbal federgestützt in der Mittelposition hält.

Nun kannst du die zwei 18650 Li-Ion Batterien einlegen. Achte dabei auf die **korrekte Polung**, wie sie in dem Bild markiert ist.

![Image](/rsc/01_img/03_RemoteSetup/RemoteBatteries.png)


## Übersicht der wichtigen Tasten

In der Anleitung wirst du nicht alle Tasten brauchen, aber es ist nützlich, sich einen groben Überblick über die allgemeinen Funktionen zu verschaffen:

![Image](/rsc/01_img/03_RemoteSetup/RemoteManual.png)


# Einrichten Fernbedienung
![image](https://github.com/Rohde-Schwarz-Garage/.github/blob/main/ressources/graphics/2024_03_13_Trennbanner_GitHub_Grey_Transparent.png?raw=true)

Damit die Fernbedienung das tut, was du möchtest, muss sie konfiguriert werden. Die nötigen Konfigurationen liegen schon auf dem PC, die folgenden Schritte zeigen dir, wie du diese auf die Fernbedienung ziehen kannst.

Schalte den PC und die Fernbedienung an.

Als Nächstes nimmst du das USB-C Kabel und verbindest den PC und die Fernbedienung miteinander. Achte darauf, dass du das Kabel oben bei der Fernbedienung einsteckst.

Beim Einstecken sollte ein Fenster mit drei verschiedenen Auswahlmöglichkeiten erscheinen. Wähle mit dem Drehrad rechts die Option „USB-Storage“ und drücke das Drehrad. Wenn du versehentlich etwas anderes ausgewählt hast, steck das Kabel einfach wieder ein und aus und wiederhole den Vorgang

![Image](/rsc/01_img/03_RemoteSetup/RemoteUSB.png)

Klicke [hier](https://download-directory.github.io/?url=https%3A%2F%2Fgithub.com%2FRohde-Schwarz-Garage%2Fhw-it-mini-drohne%2Ftree%2Fmain%2Frsc%2F03_software%2F02_edgetx%2FMODELS) und es wird automatisch der Ordner Models heruntergeladen.  Entpacke den Ordner und kopiere diesen (STRG+C oder Rechtsklick -> Kopiersymbol).

Wähle nun links unten das USB-Laufwerk der Fernbedienung aus.

![Image](/rsc/01_img/03_RemoteSetup/RemoteDrive.png)

Dort findest du einen gleich benannten Ordner (Models). Lösche den Ordner von der Fernbedienung und füge den heruntergeladenen Ordner ein (STRG+V oder Rechtsklick -> Einfüge Symbol). Sollte ein Fenster für das Ersetzen der Dateien auftauchen, wähle „Dateien im Ziel ersetzen“.

![Image](/rsc/01_img/03_RemoteSetup/RemoteReplace.png)

Warte nun, bis der Vorgang abgeschlossen wurde. Anschließend trennst du das USB-Kabel von der Fernsteuerung und startest diese neu. Durch den Neustart werden die geänderten Konfigurationen eingelesen.

Glückwunsch, du hast die benötigte Konfiguration auf die Fernbedienung übertragen. Im weiteren Verlauf wirst du nun einige Zusatzeinstellungen vornehmen.


# Konfiguration Übertragungsmodul
![image](https://github.com/Rohde-Schwarz-Garage/.github/blob/main/ressources/graphics/2024_03_13_Trennbanner_GitHub_Grey_Transparent.png?raw=true)

Damit sich die Fernbedienung mit der Drohne verbinden kann, müssen wir das Übertragungsmodul konfigurieren.

Solltest du an irgendeinem Punkt nicht weiterkommen liegt es möglicherweise an nicht installierten Treibern. In diesem Fall gehst du wie [hier](/docs/01_Materials.md#installation-zadig-usb-treiber) beschrieben vor und installierst die Treiber per *Zadig*.

Zuerst starten wir die Fernbedienung mit einem langen Druck auf den Power Button bis das *EdgeTX*-Logo erscheint. Verbinde anschließend die Fernbedienung per USB-Kabel mit dem PC. Nimm dazu den oberen Anschluss an der Fernbedienung.

Es sollte dann folgende Anzeige auf der Fernbedienung erscheinen. Wähle mit dem Drehrad durch Drehen *USB-Serial (VCP)* (1) aus und bestätige durch Drücken des Drehrads.

![Image](/rsc/01_img/03_RemoteSetup/RemoteUSBSerial.png)

Öffne dann die Software *ExpressLRS Configurator*. Du findest sie im Ordner Drohne auf dem Desktop.
Das Fenster, das sich öffnet, sieht etwa so wie unten aus. Wähle die Werte so wie in (2,3,4) aus.

![Image](/rsc/01_img/03_RemoteSetup/RemoteExpressLRSConfigurator1.png)

Anschließend sollten die Werte unten im roten Kasten automatisch ausgewählt werden. Falls nicht, vervollständige sie bitte entsprechend. Die *Binding Phrase* (5) kannst du **frei wählen**. Du musst lediglich darauf achten, dass, falls mehrere Drohnen gleichzeitig gebaut werden, nicht mehrmals die gleiche Binding Phrase verwendet wird. Sprich dich also mit anderen Drohnenpiloten ab, sonst kann es zu Verbindungsfehlern kommen und niemand kann fliegen!

Zuletzt musst du nur noch im Dropdown-Menü (6) *COM5* auswählen. Möglicherweise ist die Zahl hinter *COM* nicht 5, sondern eine andere Zahl. Das macht nichts. Im Dropdown-Menü sollte es nur eine Auswahlmöglichkeit geben, die nimmst du einfach. Gibt es mehr als eine Auswahlmöglichkeit, ist das ein Zeichen dafür, dass noch irgendein anderes Gerät am PC angesteckt ist, das gerade nicht benötigt wird. Entferne es und öffne das Dropdown-Menü neu, dann sollte nur noch eine Möglichkeit übrigbleiben.

Anschließend kannst du die Konfiguration auf die Fernbedienung übertragen, indem du *Auf Gerät installieren* (7) drückst.

![Image](/rsc/01_img/03_RemoteSetup/RemoteExpressLRSConfigurator2.png)

Wenn die Installation fertig ist, kannst du die Fernbedienung abstecken und ausschalten sowie das Programm schließen. Kommt es zu Fehlern, liegt es wahrscheinlich an fehlenden Treibern, die du per *Zadig* nachinstallieren kannst (1.4.1 ).

![Image](/rsc/01_img/03_RemoteSetup/RemoteStartPage.png)

Nachdem du alles erfolgreich abgeschlossen hast, müssen wir noch eine kleine Änderung an der Fernbedienung machen. Dafür musst du die Fernbedienung starten und zum Startbildschirm gelangen.

Jetzt müssen wir in das System Menü gelangen. Dafür musst du den **SYS-Knopf** drücken. Danach sollte dieses Menü auf dem Bildschirm zu sehen sein: 

![Image](/rsc/01_img/03_RemoteSetup/RemoteToolsPage.png)

Nun haben wir die verschiedenen Tools aufgezählt, die es für den Controller gibt. Um das Übertragungsmodul zu konfigurieren, müssen wir in das Tool **ExpressLRS** gelangen. Mit dem Bestätigen des Drehrads gelangst du in ExpressLRS und solltest diesen Bildschirm sehen:

![Image](/rsc/01_img/03_RemoteSetup/RemoteLuaScript.png)

Nun können wir auch schon die erste Einstellung verändern. Und zwar müssen wir die erste Zeile mit dem Namen **Packet Rate** verändern (im Bild markiert). Diese musst du auf 150Hz einstellen. (Wenn die Paketrate bereits auf **150 Hz** eingestellt ist, kannst du zurück zum Startbildschirm gehen)


## [Klicke hier, um zurück zur Übersicht der Kapitel zu kommen!](/README.md#kapitel)