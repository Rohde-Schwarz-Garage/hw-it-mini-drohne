# Zusammenbau Rahmen


## Grundlegende Komponenten einer Drohne

Im Kern ist eine Drohne ziemlich simpel: Es gibt eine Energiequelle, den Akku. Aus diesem wird die Energie entnommen und über die ESCs (Electronic Speed Controller), die auf der Platine des Flight Controllers sitzen, an die vier Motoren geschickt. Die Motoren treiben die Propeller an, die wiederum für Auftrieb sorgen, sodass die Drohne abheben und fliegen kann. Aerodynamisch funktioniert sie im Grunde wie ein Helikopter, nur statt einem großen Rotor hat sie eben vier kleinere Propeller.

Die Steuerung des ganzen übernimmt der Flight Controller. Er ist das Gehirn der Drohne. Seine Befehle erhält er von der Fernbedienung, die du in der Hand hältst.  
In der Fernbedienung integriert ist ein Übertragungs- bzw. Sendemodul. Auf dem Flight Controller sitzt das Gegenstück dazu, das Empfangsmodul. Über diese Module hinweg erfolgt die Kommunikation zwischen Fernbedienung und dem Flight Controller auf der Drohne.

**Legende:** 
<code style="color : Cyan">Kommunikation/Steuerung</code>
<code style="color : Orangered">Energiefluss</code>


![Image](/rsc/01_img/02_FrameAssembly/BasicConcept.png)


## Akku laden

Als allererstes werden wir die Akkus laden, damit sie mit Sicherheit voll sind, sobald es an den ersten Flug der Drohne geht.

**Wichtig:** Lies bitte unbedingt zuerst die Sicherheitshinweise zu Akkus bevor du fortfährst. Klicke dazu [hier](/docs/09_Safety.md#sicherer-umgang-mit-lipo-akkus).

Die Stromstärke stellst du mit mehrmaligem kurzem Drücken des *Current Set* - Buttons (1) ein. Die Spannung stellst du mit mehrmaligem kurzem Drücken des *Voltage Set* – Buttons (2) ein. 

Wenn du die richtigen Werte für Stromstärke (4) und Spannung (6) eingestellt hast, kannst du das Laden durch **langes** Drücken des *Start/Stop*–Buttons (1) starten. Dadurch werden Stromstärke (4) und Spannung (6) rot hinterlegt und lassen sich jetzt auch erst wieder ändern, wenn du das Laden durch langes Drücken des *Start/Stop*–Buttons (1) unterbrichst.

Den/die Akkus kannst du jetzt einfach anstecken. Im Feld (7) sollte dann auch dessen aktuelle Spannung angezeigt werden. Ein roter blinkender Punkt auf der linken Seite signalisiert, dass er geladen wird.

Grundsätzlich ist das Ladegerät auch hotplugging-fähig, sprich du kannst jederzeit einen Akku an- oder abstecken. Es ist dennoch ratsam einen Akku nur dann an- oder abzustecken, wenn du dir auch sicher bist, dass du das möchtest.

Die Spannung (5) ist lediglich die Eingangs-Spannung des Netzteils. Diese kann auch einen anderen Wert haben als auf dem Bild, lass dich davon nicht verwirren.

![Image](/rsc/01_img/02_FrameAssembly/Charger.png)
![Image](/rsc/01_img/02_FrameAssembly/ChargerScreen.png)

Wenn der Akku fertig geladen ist, sprich die Spannung des Akkus (7) gleich der Zielspannung (6) ist, dann stoppt das Ladegerät für diesen Akku automatisch und zeigt *OK!* (8) an.


## Zusammenbau Rahmen

### 3D-Druck

Einige Teile der Drohne werden aus Plastik gedruckt. Dies sind die farbigen Markierungen des Rahmens, der Standfuß und die Deckplatte. Wenn du vor Ort in der Garage das Projekt machst sind die Teile bereits vorgedruckt und du musst dich mit der Thematik nicht weiter beschäftigen.

Wenn du die Teile bei dir zuhause mit einem einfarbigen Drucker druckst, findest du hier die STEP, STL, 3mf und G-Code Dateien. Wenn dein Drucker mehrere Materialien gleichzeitig drucken kann (z.B: Bambulab mit AMS) findest du hier STEP und STL-Dateien. 

Mit den STEP-Dateien kannst du in einem CAD-Programm deiner Wahl Änderungen an den Teilen vornehmen. Die STL-Dateien kannst du in einen Slicer deiner Wahl laden und für deinen eigenen Drucker G-Codes erstellen. Als Besonderheit findest du auch 3mf Projekt-Dateien für den PrusaSlicer. Diese sind nach dem Muster *ZuDruckendeTeile_Material_Drucker.3mf* benannt. Nach dem gleichen Muster sind auch fertig geslicte Dateien für den für den Prusa MK3s mit der Endung .gcode verfügbar. Achte stets darauf nur Dateien zu Drucken, die für den 3D-Drucker und das geladene Material gedacht sind, ansonsten kann es zu Schäden an dem Drucker kommen.

Geeignete Materialien für Standfuß und Deckplatte sind **PETG oder ABS**. Für die Markierungen solltest du **TPU** verwenden, falls dein Drucker dies drucken kann. Ansonsten verwende ebenfalls PETG oder ABS. Die Farben für die zwei Markierungen sollten farblich gut unterscheidbar sein, da sie die als Orientierung für die Ausrichtung der Drohne dienen.


### Kleben der Markierungen und des Standfußes

Als allererstes werden wir der Drohne ein *Vorne* und ein *Hinten* geben.

>Wie du auf dem Deckblatt mit der fertigen Drohne vielleicht schon erkannt hast, ist es ohne die farblichen Markierungen schwierig, vorne von hinten oder links von rechts zu unterscheiden. Ohne diese Referenzpunkte zur Orientierung, hättest du es später sehr schwer, die Drohne zu steuern.

Da der Kleber für den Standfuß etwa 20min braucht, um einigermaßen fest zu werden, starten wir mit den Klebeteilen. Bis der Kleber angetrocknet ist, werden wir uns dann mit der Fernbedienung beschäftigen.

Allgemein solltest du alle Klebeflächen einmal abwischen, **bevor** du Kleber oder Klebeband anbringst, um Fettrückstände und Verunreinigungen zu entfernen.#

Zuerst bringen wir die **blaue** Markierung auf einer beliebigen Seite, die senkrecht zur im Bild eingezeichneten Mittelachse (1) liegt, an. Um die Achse zu finden, kannst du dich auch an der pfeilartigen Stelle im Rahmen (2) orientieren. Du nimmst also das doppelseitige Klebeband und klebst es so wie unten zu sehen, auf den Außenseiten des Rahmens an. Du kannst das Band an einem Stück anbringen oder in Einzelteilen, wie es dir lieber ist. Entferne die Schutzfolie des Klebebandes erst, wenn es an Ort und Stelle ist und du die Markierung ankleben willst. Das vereinfacht das initiale Ankleben deutlich.

![Image](/rsc/01_img/02_FrameAssembly/FrameTaped.png)
![Image](/rsc/01_img/02_FrameAssembly/FrameCenterLine.png)

Drücke dann die Markierung wie auf dem Foto an den Rahmen an. Anschließend machst du das gleiche mit der **roten** Markierung auf der gegenüberliegenden Seite der Drohne. 

![Image](/rsc/01_img/02_FrameAssembly/FrameMarked.png)

Nun fehlt nur noch der Standfuß. Dieser besteht anfangs noch aus zwei Teilen.

Uhu Extreme ist ziemlich gutmütig, was die Verarbeitungszeit angeht, das heißt er wird nicht sofort fest und ist daher nicht so gefährlich im Umgang. **Achte dennoch** darauf, dass deine Finger sauber bleiben und kein Kleber auf den Boden o.ä. tropft. Lege dir **vor** der Verarbeitung ein Papiertuch bereit, um eventuelle Tropfen sofort wegwischen zu können und wasche dir **sofort** die Hände, sollten sie doch schmutzig werden.

Trage also etwas Uhu Extrem Kleber auf beide Klebeflächen auf und presse das Unterteil des Standfußes an das Oberteil. Am besten du drückst die zwei Teile dabei zwischen Daumen und Zeigefinger (s. Foto).

![Image](/rsc/01_img/02_FrameAssembly/StandGlueApplied.png)
![Image](/rsc/01_img/02_FrameAssembly/StandGluePressed.png)

Ab jetzt legst du Drohne und den Standfuß in eine Ecke, wo die Gefahr möglichst gering ist, dass die angeklebten Teile in den nächsten 20 Minuten verrutschen.


## [Klicke hier, um zurück zur Übersicht der Kapitel zu kommen!](/README.md#kapitel)