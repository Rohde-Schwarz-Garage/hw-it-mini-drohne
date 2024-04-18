# Funktionstest
Nachdem wir alles richtig eingestellt haben, kommen wir jetzt zum Funktionstest.

**Grundlegende Steuerung:**
![Image](/rsc/01_img/06_TestingAndTuning/BasicControl_OnlyRemote.png)
![Image](/rsc/01_img/06_TestingAndTuning/DroneDirections.png)

Als erstes schaltest du die Fernbedienung ein, bis du wieder den Startbildschirm siehst. Danach steckst du die Batterie der Drohne an die Drohne dran. 
Um die Drohne zu starten, müssen wir erst ein paar Bedingungen erfüllen:
1.	Die Drohne darf nicht an den PC angeschlossen sein 
2.	Die Drohne muss waagrecht auf einer Fläche stehen.  

Gut, nachdem du die Bedingungen erfüllt hast kannst du jetzt die Drohne starten. Als erstes müssen wir den linken Joystick ganz nach unten drücken und danach musst du den **Arm-Button** drücken. Nun sollten sich schon die Propeller drehen und die Drohne ist bereit zu fliegen. 
Um die Motoren wieder auszuschalten, musst du wieder den **Arm-Button** drücken.

# Tuning
Nachdem du erfolgreich alle Komponenten deiner Drohne getestet hast, folgt ein essenzieller Schritt: das Tuning der Drohne. Das erste Ziel wird es sein, dass die Drohne bei zentriertem Schubregler ihre Höhe hält. Des Weiteren soll etwaiges Driften der Drohne während des Fluges ausgeglichen werden, um somit einen stabilen und kontrollierten Flug zu gewährleisten.

>Um das Phänomen des Driftens zu verstehen, ist es notwendig, die Rolle des Beschleunigungssensors innerhalb der Drohnensteuerung zu verdeutlichen. Dieser ist ein Sensor, der dazu dient, Beschleunigungen auf allen drei Achsen (x, y, z) zu messen. Er erfasst die Geschwindigkeitsänderung der Drohne sowie die Anwesenheit der Erdanziehungskraft und ermöglicht es dadurch der Drohne, ihre Lage in Bezug auf die Erdoberfläche zu bestimmen.

>Ein falsch kalibrierter Beschleunigungssensors zeigt die Neigung der Drohne in Bezug zur Erdoberfläche nicht korrekt an. Dies führt dazu, dass die Flugsteuerung versucht, eine falsch wahrgenommene Neigung auszugleichen. Im Ergebnis führt dies zu einem Driften in die entgegengesetzte Richtung der falsch angezeigten Neigung.

>In ähnlicher Weise kann ein nicht richtig getrimmter Beschleunigungssensor dazu führen, dass die Flugsteuerung eine schräge "Ruheposition" annimmt. Dadurch wird auch ohne Steuerbefehle eine Bewegung in Richtung dieser scheinbaren Neigung eingeleitet, was ebenfalls zu einem Driften der Drohne führt.

>Um also ein stabiles und kontrolliertes Flugerlebnis zu gewährleisten, ist es von essenzieller Bedeutung, die Kalibrierung und das Trimming des Beschleunigungssensors exakt durchzuführen. Dies hilft dabei, Driften der Drohne auszugleichen und ermöglicht einen stabilen und präzisen Flug.

## Kalibrierung Beschleunigungssensor und Gyroskop
Bevor du mit dem Trimming des Beschleunigungssensors beginnst, musst du diesen und das Gyroskop kalibrieren. 

>Das Gyroskop ist ein weiterer wichtiger Sensor in deiner Drohne. Es misst die Winkelgeschwindigkeit, also wie schnell sich die Drohne um ihre eigene Achse dreht. Damit sorgt das Gyroskop für Stabilität im Flug und hilft, die Drohne bei Wind oder bei Steuerbefehlen in der gewünschten Lage zu halten. 

**Hier sind die Schritte, die du befolgen musst:**
1.	Schalte die Fernbedienung ein.
2.	Schiebe die Batterie in den Einschub an der Drohne und verbinde anschließend die Batterie mit der Drohne. Stelle die Drohne auf eine waagrechte, glatte Fläche.
3.	Prüfe, ob die Drohne vollständig eben auf ihren Standfüßen steht.

![Image](/rsc/01_img/06_TestingAndTuning/DroneOnPlane.png)

4.  Führe den Stick Befehl für die Gyroskop-Kalibrierung durch, indem du den linken Stick in der linken unteren Ecke und gleichzeitig den rechten Stick unten in der Mitte für einige Sekunden hältst. Auf dem Bild ist die Position der Sticks nochmals dargestellt

![Image](/rsc/01_img/06_TestingAndTuning/StickGyroCalibration.png)

![Image](/rsc/01_img/06_TestingAndTuning/RemoteGyroCalibration.png)

5. Warte einige Sekunden und führe dann den Stick Befehl für die Beschleunigungssensor-Kalibrierung aus, indem du den linken Stick in der linken oberen Ecke und gleichzeitig den rechten Stick unten in der Mitte für einige Sekunden hältst.

![Image](/rsc/01_img/06_TestingAndTuning/StickAccellCalibration.png)

6.  Führe einen kurzen Flugtest durch. Dafür armst du die Drohne (wie vorhergehend in den Sicherheitshinweisen beschrieben) und gibst Schub bis die Drohne abhebt und schwebt, ohne sie durch den Raum zu steuern. Ein leichtes Driften oder ungleichmäßiges Halten der Höhe stört an dieser Stelle nicht. Das werden wir im nächsten Schritt ausgleichen.

Sollte die Drohne sehr unruhig fliegen bietet es sich an die Schritte 1 bis 5 zu wiederholen.

## Trimmen des Schubreglers
>Damit die Drohne ruhig schweben kann muss sie eine gewisse Menge an Schub erzeugen, der ihr Eigengewicht ausgleicht. Dieser Schub soll erzeugt werden, wenn der Schubregler an der Fernsteuerung sich in der Mittelposition befindet. Um dies zu erreichen, wird durch Trimmen der an die Drohne übertragene Wert für den Schubregler verschoben, während die physische Position des Sticks gleichbleibt.

**Vorbereitung vor dem Trimmen:**

Zuerst musst du sicherstellen, dass nicht aus Versehen Trimm eingestellt wurde während den vorhergegangenen Schritten. Vergleiche dazu das Display der Fernsteuerung mit der Abbildung und korrigiere mit dem entsprechenden Trimm-Reglern, bis alle Balken symmetrisch sind.

Kontrolliere zusätzlich, dass der Akku mindestens halb voll ist.
>Ist der Akku weniger als halb voll, so ist die Leistungsabgabe etwas vermindert. Folglich ist auch etwas mehr Schub nötig, um die Drohne in der Luft zu halten. Für ein möglichst unverfälschtes Trim-Ergebnis sollte also der Akku mindestens halb voll sein.

![Image](/rsc/01_img/06_TestingAndTuning/RemoteStartTrim.png)

**Das eigentliche Trimmen:**
1.	Schalte die Fernsteuerung an und verbinde die Drohne wie bereits vorhergehend beschrieben mit dem Akku. Stelle die Drohne anschließend in die Raummitte.
2.	Arme die Drohne und führe den Schubregler in die Mitte, bis er die neutrale Position erreicht.
3.	Wenn die Drohne an Höhe verliert oder gar nicht erst abhebt, trimme den Schubregler nach oben. Wenn die Drohne stetig an Höhe gewinnt, trimme Schubregler nach unten. Dafür bewegst du den Trimm-Regler in die entsprechende Richtung und fügst somit eine Einheit Trimm hinzu. Der Vorgang lässt sich beliebig wiederholen und summiert somit den Trimm auf.  
Den Regler zum Trimmen findest du auf der Fernsteuerung, wie auf dem Bild ersichtlich. Das Trimmen des Schubreglers ist auch während dem Flug möglich, um die Auswirkungen direkt zu sehen.

![Image](/rsc/01_img/06_TestingAndTuning/RemoteThrottleTrim.png)

4.	Trimme so lange, bis die Drohne ihre Höhe selbstständig hält. Das kann etwas Geduld erfordern aber lohnt sich am Ende.

## Trimmen des Beschleunigungssensors
**Stickbefehle für das Trimmen:**

![Image](/rsc/01_img/06_TestingAndTuning/StickAccellTrim.png)

>Turbulenzen bezeichnen Luftunruhen, die durch die Nähe von Gegenständen oder Wänden erzeugt werden. Diese können die Flugfähigkeit und -stabilität deiner Drohne erheblich beeinflussen, da sie die durch die Propeller produzierten Luftströme stören. Daher kann das Schweben in der Nähe von Wänden oder Gegenständen deine Einschätzung zur Schwebestabilität verfälschen. Stelle beim Trimmen sicher, dass deine Drohne möglichst weit von Gegenständen entfernt in der Mitte des Raums schwebt.

**Hier sind die Schritte, die du befolgen musst:**
1.	Nachdem du deine Drohne sicher in die Mitte des Raums gebracht hast, lass sie schweben und beobachte, in welche Richtung sie driftet. Während des Prozesses solltest du darauf achten, den rechten Stick so wenig wie möglich zu benutzen. Sollte die Drohne nach links driften, wird dies durch ein Trimmen nach rechts ausgeglichen.
2.	Sobald du die Richtung des Driftens ermittelt hast, lande die Drohne und deaktiviere die Motoren ("Disarm").
3.	Als nächstes, führe den Stick Command, wie in der Darstellung ersichtlich, aus, um den Beschleunigungssensor in die entgegengesetzte Richtung des Driftens zu trimmen.  
**Für unser Beispiel bedeutet dies:** Wenn die Drohne nach links driftet, führe den Stick Command für ein Trimmen nach rechts aus. Dies trimmt um eine Einheit nach rechts, ein mehrmaliges Wiederholen ist möglich und summiert die Einheiten auf.
4.	Lasse die Drohne erneut schweben und überprüfe, ob noch Drift auftritt. Sollte die Drohne nun gleichmäßig schweben, hast du das Trimmen erfolgreich abgeschlossen. Falls noch Drift vorhanden ist, wiederhole die Schritte, bis die Drohne stabil schwebt.

Das korrekte Trimmen des Beschleunigungssensors ist eine wichtige Fähigkeit, die dir dabei helfen wird, die volle Kontrolle über deine Drohne zu erhalten und das bestmögliche Flugerlebnis zu erzielen. Es verlangt Geduld und Genauigkeit, aber die Belohnung einer gut abgestimmten Drohne ist es definitiv wert.

## Spaß haben
Herzlichen Glückwunsch, deine Drohne ist nun voll flugfähig!

Um deine Flugkünste zu trainieren kannst du dir noch selbst etwaige Szenarien überlegen. Beispielsweise ein Slalomkurs, durch den du fliegen musst, ohne die Pylonen zu berühren. Als Pylonen lassen sich dabei wunderbar Stühle missbrauchen, sowohl oberhalb der Sitzflächen die Stuhllehnen als auch die Stuhlbeine unterhalb. Deiner Fantasie sind keine Grenzen gesetzt. Viel Spaß!


## [Klicke hier, um zurück zur Übersicht der Kapitel zu kommen!](/README.md#kapitel)