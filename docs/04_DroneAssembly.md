# Zusammenbau Drohne

Nachdem du nun die Fernbedienung und das Übertragungsmodul eingerichtet hast, geht es jetzt an den Zusammenbau der eigentlichen Drohne.

Inzwischen sind wahrscheinlich mehr als 20min vergangen, daher kannst du die Drohne nun aus ihrer Ecke nehmen und wir beginnen den Aufbau.


## Motoren

Nimm die vier Motoren zur Hand. Wir werden diese am Rahmen anbringen. Dazu müssen wir Schraubensicherung verwenden. Der Einfachheit halber kannst du die Motoren aber schon mal **locker** mit 2 der 3 Schrauben anbringen und erst anschließend bringen wir auf jede Schraube die Schraubensicherung auf (die Schrauben also noch **nicht ganz** anziehen). Achte dabei darauf, dass die Kabel in Richtung der Mittelachse zeigen. 

![Image](/rsc/01_img/04_DroneAssembly/MotorScrewPlacement.png)

Da der Motor jetzt mit den zwei Schrauben an Ort und Stelle bleibt, trage auf die dritte Schraube einen kleinen Tropfen Schraubensicherung auf und ziehe sie vorsichtig fest. Fest bedeutet dabei wirklich nur, bis die Schraube ganz drin ist. Wende also nicht viel Kraft auf, da sie sonst eventuell abreißen könnte.

Tipp: Wenn du statt der ganzen Hand nur zwei Finger zum Drehen des Schraubenziehers verwendest, wendest du automatisch weniger Kraft an. 

![Image](/rsc/01_img/04_DroneAssembly/ThreadlockApplication.png)

>Schraubensicherung benötigen wir deswegen, weil sich durch die Vibrationen und die vielen Beschleunigungsmomente des Motors die Schraube langsam Stück für Stück wieder lösen könnte. Ähnlich wie sich eine Schleife am Schuh irgendwann lösen kann, ohne dass du tatsächlich an einem Ende gezogen hast. Die Schraubensicherung verhindert das, indem sie die Schraube ähnlich wie ein Kleber festhält, sodass mehr Kraft notwendig ist, um sie zu lösen.

Wiederhole das gleiche mit den anderen 2 Schrauben, indem du sie herausdrehst und nach dem Aufbringen der Schraubensicherung festziehst.

Den ganzen Prozess wiederholst du nochmal für die drei anderen Motoren. Achte auch dort bitte auf die richtige Orientierung der Kabel. Deine Drohne sollte jetzt folgendermaßen aussehen. 

![Image](/rsc/01_img/04_DroneAssembly/MotorsAssembled.png)


## Flight Controller

Zuerst musst du kontrollieren ob an dem Flight Controller der richtige Stecker angelötet ist. Dieser heißt A30 (1) und eignet sich am besten für kleine Drohnen. Alternativ kannst du für den Flight Controller auch BT2.0 (2) Stecker verwenden. Am Ende der Anleitung findest du Links zu den verwendeten Steckern. Diese sind als Pigtail vorgefertigt – Stecker sind bereits mit Kabeln vorbereitet – und die Verwendung spart dir viel Arbeit.

![Image](/rsc/01_img/04_DroneAssembly/DifferentPlugs.png)

Sollte der Stecker noch nicht vorhanden sein so musst du diesen erst an den Flight Controller anlöten. Wenn du noch keine Erfahrung mit Löten hast, so findest du hier ein gutes Tutorial. Alternativ kannst du gerne zu uns in die Garage kommen und dich mit professionellem Equipment in das Löten einarbeiten. 

Achte beim Löten des Steckers auf die **korrekte Polung**, da ansonsten es zu einer Beschädigung des Flight Controllers kommt, sobald du die Batterie ansteckst. Ebenfalls müssen die Kabel auf der Seite des Micro-USB Ports angelötet werden, da es ansonsten zu Problemen beim Verbau kommt.

![Image](/rsc/01_img/04_DroneAssembly/FlightControllerPolarisation.png)

Als nächstes werden wir das Herz der Drohne, den Flight Controller, montieren. Dieser braucht zunächst seine Standfüße, die du am besten mit einer Pinzette durch die Löcher ziehst. Das ist etwas tricky, lass dich nicht entmutigen, mit ein wenig Übung wirst du es schaffen. Achte darauf mit der Pinzette nicht abzurutschen und dabei die elektrischen Komponenten auf dem Board zu beschädigen. Achte außerdem auch auf die Orientierung, sodass die **lange Seite der Gummifüße auf derselben Seite wie der USB-Anschluss des Flight Controllers ist**. 

![Image](/rsc/01_img/04_DroneAssembly/FlightControllerStandoffs.png)
![Image](/rsc/01_img/04_DroneAssembly/StandoffApplikation.png)

Der gesamte Flight Controller mit den Gummifüßen soll nun auf den Rahmen gesetzt werden. Die Orientierung soll so wie auf dem Bild sein, sodass der USB-Anschluss nach unten zeigt und auf der hinteren Seite der Drohne ist (rote Markierung). Da die Anschlüsse der Motoren nach der Montage des Flight Controllers nicht mehr zugänglich sind, müssen diese **vor** der Montage eingesteckt werden. Die Stecker haben auf einer Seite eine Nase, die nur in einer Richtung passt. Sieh sie dir genau an und dann steck sie ein. Die Kabel müssen in etwa so geführt sein wie auf dem Bild, damit später keine Gefahr besteht, dass sie sich in den Propellern verfangen. Jetzt kannst du den Flight Controller auf die Montagepunkte im Rahmen senken. Es sollte aktuell so aussehen (Überprüfe insbesondere auch die Kabelverläufe):

![Image](/rsc/01_img/04_DroneAssembly/CableRouting.png)

Obendrauf kommt dann nur noch die schwarze Abdeckplatte mit R/S-Logo, achte auch bei ihr darauf, dass die Schrift in Flugrichtung „vorne“ zeigt (also in Richtung blaue Markierung). Befestigt wird alles mit den 4 noch verbleibenden Schrauben. Wie bei den Motor-Schrauben soll wieder nur so fest angezogen werden, dass die Schraube am Anschlag ist, damit sie nicht abreißt. 

![Image](/rsc/01_img/04_DroneAssembly/DeckplateScrews.png)


## Hinweis

Die wichtigsten Bauteile sind jetzt schon zusammengebaut, es fehlt also nicht mehr viel und die Drohne ist technisch gesehen flugbereit. Als erstes fallen dir bestimmt die noch fehlenden Propeller auf und natürlich braucht deine Drohne auch noch einen Akku. Die Anleitung zu deren Montage folgt hier auch gleich. Bitte lies aber unbedingt **zuerst** die [Sicherheitshinweise](/docs/09_Safety.md).

## Propeller

Es gibt für jeden Propeller eine Drehrichtung und auf der Drohne gibt es für jeden Motor eine Drehrichtung. Diese Richtungen müssen übereinstimmen.

>Die Drehrichtungen sind deswegen so wichtig, weil sich die Drohne später während des Fluges mit Hilfe verschiedener Drehzahlen zwischen den einzelnen Motoren dreht. Wenn alle Motoren in die gleiche Richtung drehen würden, dann würde sich die Drohne ständig drehen, ähnlich wie ein Helikopter, bei dem der hintere Rotor ausgefallen ist. Wenn nun zwei Motoren in die eine und zwei Motoren in die andere Richtung drehen, dann heben sich diese sogenannten Drehmomente gegenseitig auf und die Drohne steht still in der Luft. Gleichzeitig erhält man so eine einfache Möglichkeit die Drohne zu steuern. Indem man die Drehzahl der Motoren nur ein wenig anpasst dreht sie sich schon, weil insgesamt mehr Moment nach links, als nach rechts besteht oder eben umgekehrt.

Am einfachsten ist, du orientierst dich am untenstehenden Bild. Es ist sehr wichtig, dass die Richtungen stimmen, nimm dir also Zeit und prüfe genau. Die Drehrichtung der Propeller kannst du an der sogenannten leading edge, also an der führenden Kante des Propellers (in <code style="color : Orangered">Rot</code> eingezeichnet) erkennen.

![Image](/rsc/01_img/04_DroneAssembly/PropDirectionBetaflight.png)

![Image](/rsc/01_img/04_DroneAssembly/PropDirectionDrone.png)

Wenn du dir sicher bist, welcher Propeller wohin kommt, dann bleibt nur noch ihn aufzustecken. Dazu musst du nichts weiter machen, als ihn vorsichtig aufzustecken. Halte gleichzeitig von hinten dagegen, damit sich dabei nicht der Rahmen verbiegt. Es kann etwas Kraft benötigen bis der Propeller ganz auf der Achse steckt. Es gilt der Grundsatz: so wenig Kraft wie möglich, aber so viel wie nötig.

![Image](/rsc/01_img/04_DroneAssembly/PropMounting.png)

## Standfuß montieren

Nun befestigst du den zusammengeklebten Standfuß an dem Rahmen der Drohne. Hierfür clipst du diesen, wie auf dem Bild ersichtlich um den Rahmen. Es ist möglich, dass du dafür den Rahmen etwas zusammendrücken musst. Übe dabei allerdings nicht zu viel Kraft aus.

![Image](/rsc/01_img/04_DroneAssembly/StandMounting.png)

## Akku einbauen

Zu guter Letzt musst du vor Benutzung der Drohne nur noch den Akku in seine Halterung einführen. Stecke den Akku aber noch nicht an bzw. vom Ladegerät ab, bis du bei [Konfiguration Motorsteuerung](/docs/05_FlightControllerSetup.md#konfiguration-motorsteuerung) angekommen bist.

![Image](/rsc/01_img/04_DroneAssembly/BatteryMounting.png)
  
## [Klicke hier, um zurück zur Übersicht der Kapitel zu kommen!](/README.md#kapitel)