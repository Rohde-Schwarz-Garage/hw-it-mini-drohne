# Einrichten Flight-Controller

Damit die Drohne fliegen kann muss nicht nur die Hardware korrekt zusammengebaut sein, sondern auch die Software richtig konfiguriert sein. Einen Großteil, die Flugsteuerung im Flight Controller, werden wir in diesem Kapitel erledigen.

Wir starten damit die Firmware auf den Controller zu flashen.

> Firmware kannst du dir im Grunde vorstellen wie das Betriebssystem auf deinem PC/Laptop zu Hause. Erst dadurch kannst du mit der Hardware interagieren und sie das machen lassen, was du möchtest. Erst dadurch kannst du Einstellungen vornehmen, Programme ausführen, Internetseiten öffnen usw. Auf dem Flight Control-ler läuft nur eben kein Windows, Android oder iOS, sondern ein ganz spezielles für diesen Zweck entwickeltes Betriebssystem namens _Betaflight_. Dieses Betriebssystem müssen wir nun zu anfangs installieren, was man allgemein auch „flashen“ nennt.

**Wichtig:** Immer wenn du den Flight Controller länger als ein paar Sekunden mit dem PC verbindest, richte einen Lüfter auf ihn. Gerade während des Flashens kann er sehr heiß werden. Ohne ein wenig Kühlung riskiert man im besten Fall ein Abstürzen des Controllers, was insbesondere wenn man Einstellungen noch nicht gesi-chert hat, sehr ärgerlich sein kann. Im schlimmsten Fall kann es bei manchen Flight Controllern sogar zu De-fekten führen.

Um Betaflight installieren zu können, müssen wir den Controller zuerst in einen speziellen Modus versetzen, der diese Art von Zugriff ermöglicht. Nimm einen kleinen Flachkopfschraubenzieher zur Hand und halte ihn wie auf dem Bild auf die markierten Kontakte (1) auf dem Flight Controller. Während du immer noch die zwei Kon-takte mit dem Schraubenzieher verbunden hältst, verbinde den Controller mit dem USB-Kabel an den PC.  Möglicherweise ist es einfacher das mit einer zweiten Person gemeinsam zu machen, sodass eine nur die Kontakte mit dem Schraubenzieher verbindet und die andere nur das Kabel ansteckt. Hast du alles richtig ge-macht, dann blinkt nur die rote LED (2) auf der gegenüberliegenden Seite des USB-Anschlusses. Falls etwas schiefgelaufen ist, dann blinken sowohl die etwas kleinere grüne LED als auch die hellere rote LED abwech-selnd. In diesem Fall wiederholst du den Prozess einfach (Kabel nochmal abstecken und dann wieder anste-cken). Achte vor allem darauf, dass der Schraubenzieher tatsächlich die zwei Kontaktstellen verbindet.

![Image](/rsc/01_img/05_FlightControllerSetup/FlightControllerBootPins.png)

![Image](/rsc/01_img/05_FlightControllerSetup/BootPinsShorted.png)

![Image](/rsc/01_img/05_FlightControllerSetup/BootSuccessful.png)

Sobald also ausschließlich die rote LED blinkt, öffne auf dem PC das Programm _Betaflight Configurator_. Du solltest es wie in [Installation Software und Treiber](/docs/01_Materials.md#installation-betaflight-konfigurator) beschrieben bereits installiert haben. Falls nicht, solltest du das jetzt nachholen. Die Startseite sollte in etwa wie auf dem Bild aussehen. Achte darauf, dass weder der _ExpressLRS Configurator_ noch der _ESC Configurator_ (aus einem späteren Kapitel) geöffnet sind, während du im _Betaflight Configurator_ arbeitest.

![Image](/rsc/01_img/05_FlightControllerSetup/BetaflightStartScreen.png)

>_Betaflight Configurator_ ist eine Software, mit der die Firmware auf den Flight Controller geflashed werden kann und anschließend dann alle Einstellungen vorgenommen werden können, damit der Flight Controller genau das macht, was du möchtest. Der Zugriff erfolgt über die USB-Verbindung. Um also Einstellungen zu tätigen, muss der Flight Controller später wieder per USB-Kabel verbunden werden.

Wähle nun links den Reiter _Firmware Flasher_ (1). Im Einstellungsfeld (2) wählst du BetaflightF4, **in der Version 4.4.3** und aktivierst **Chip vollständig löschen**. Dann sollte das Fenster so aussehen wie auf dem Bild. Wichtig ist, dass oben rechts DFU – STM32 Bootloader angezeigt wird. Das bestätigt, dass der Flight Controller im richtigen Modus ist und damit auch, dass du davor beim Verbinden der Kontakte alles richtig gemacht hast. Eine mögliche Fehlerquelle können auch wieder fehlende Treiber sein. In diesem Fall insbesondere der STM32-Treiber. Halte dich an die Anleitung in [Installation Software und Treiber](/docs/01_Materials.md#installation-betaflight-konfigurator), um das zu beheben. Achte außerdem darauf, dass alle anderen Programme geschlossen sind.

![Image](/rsc/01_img/05_FlightControllerSetup/BetaflightFlash.png)

Jetzt kannst du die Firmware online laden (3). Sobald der Vorgang abgeschlossen ist, wird der Button _Firmware Flashen_ (4) auch gelb werden und du kannst auch ihn drücken. Dann beginnt das eigentliche Flashen. Es dau-ert ein paar Sekunden und wird quittiert mit einem grünen Balken und der Meldung Programmierung erfolgreich (5).

![Image](/rsc/01_img/05_FlightControllerSetup/BetaflightFlashSuccessful.png)

Jetzt sollte oben rechts statt _DFU – STM32 Bootloader_ dann _COM3 – Betaflight STM32F405_ stehen (statt _COM3_ kann es an deinem PC möglicherweise auch eine andere Zahl als 3 sein). Drücke auf _Verbinden_ (7). Wahrscheinlich ploppt ein Fenster auf, in dem es um Standardeinstellungen geht. Dort musst du den Button _Benutzerdefinierte Standardeinstellungen_ anwenden drücken.

![Image](/rsc/01_img/05_FlightControllerSetup/BetafligthComPort.png)

Du solltest jetzt in der Benutzeroberfläche sein, in der du so ziemlich alles einstellen kannst, was es gibt. Wenn du deine Drohne ein wenig in der Luft drehst und schwenkst, solltest du genau diese Bewegungen auch in der Anzeige (7) sehen können.

![Image](/rsc/01_img/05_FlightControllerSetup/BetaflightStartConnected.png)

>Während wir bei normalen PCs und Laptops meistens über Bildschirme interagieren, an die direkt vom Rechner ein Videosignal gesendet wird, ist das beim Flight Controller etwas anders. Er ist nur per USB an den PC ange-bunden und wir können aber die speziell dafür entwickelte Software _Betaflight Configurator_ daran Einstellungen in einer grafischen Benutzeroberfläche vornehmen. Im Grunde fungiert der PC nur als Übermittler.

Im aktuellen Zustand lässt sich mit der Drohne aber noch nicht viel anfangen. Sie hat weder eine Verbindung zur Fernbedienung, noch weiß sie, wie sie auf verschiedene Befehle der Fernbedienung reagieren soll. Auch weiß die Drohne noch nicht, was sie überhaupt für Komponenten besitzt und wie sie diese intern ansteuern muss.

Für die allermeisten dieser Einstellung gibt es schon ein gutes Preset (bereits davor abgespeicherte Konfigura-tion), das die meiste Arbeit für dich erledigt. Du findest es im Reiter _Presets_ (8). Die Kachel _ExpressLRS 150Hz_ (9) sollte ganz oben links zu sehen sein. Falls sie nicht zu sehen ist, kannst du einfach im Suchfeld (10) danach suchen, indem du dort _ExpressLRS_ eingibst.

![Image](/rsc/01_img/05_FlightControllerSetup/BetaflightPresets.png)

Mit Klick auf die Kachel öffnet sich dann ein Fenster in dem du nur noch im Drop-Down-Menü folgende Haken (11) setzen musst:
-	Ultra Cinematic
-	Serial, separate RX
-	Whole Pack values

![Image](/rsc/01_img/05_FlightControllerSetup/BetaflightExpressLRS.png)

Wenn du die Haken gesetzt hast, dann kannst du auf _Auswählen_ (12) drücken. Anschließend laden wir noch ein paar Einstellungen, die schon extra für dich vorbereitet wurden, indem du auf _Backup laden_ (13) drückst. Du wirst dann aufgefordert eine passende Datei auszuwählen. Du findest sie [hier](/rsc/03_software/01_betaflight) mit dem Namen _Backup_Drohne.txt_. Wenn du diese Backup-Datei geöffnet hast, dann kannst du auf Speichern und _Neustarten_ (14) drücken. Der Flight Controller startet nun neu und wird sich gleich darauf wieder automatisch verbinden.

Damit sind wir fürs erste mit dem Flight Controller selbst fertig. Bitte lies nun unbedingt **zuerst** die [Sicherheitshinweise](/docs/09_Safety.md) und fahre **erst dann** mit der weiteren Einrichtung fort.

# Konfiguration Motorsteuerung

Als nächstes konfigurieren wir die ESCs, also die Motorsteuerung.

>Wie in der grundlegenden Beschreibung der Drohne (2.1) erwähnt sind die ESCs (Electronic Speed Controller) dafür verantwortlich die Energie so an die Motoren zu leiten, wie es der Flight Controller vorgibt. Um das korrekt ausführen zu können, müssen die ESCs aber einige Parameter übergeben bekommen. Genau das machen wir in diesem Kapitel.

Entferne den Akku vom Ladegerät und verbinde ihn mit der Drohne. Lass dich nicht verunsichern, ein eventuel-les Piepsen der Drohne beim Anstecken des Akkus ist ganz normal. Verbinde dann die Drohne per USB-Kabel an den PC. Vergiss dabei nicht, wieder den Lüfter auf die Drohne zu richten. Öffne im Browser [esc-configurator.com](https://esc-configurator.com). Achte darauf, dass sowohl der _Betaflight Configurator_ als auch der _ExpressLRS Configurator_ geschlossen sind, während du im _ESC Configurator_ arbeitest. Außerdem muss die Fernbedienung ausgeschaltet sein. Das Browser-Fenster sollte wie unten aussehen.

Port und Baud-Rate rechts oben (1) sollten schon automatisch vorausgewählt sein. Falls sie nicht vorausgewählt sind, dann gehe auf _Seriellen Port wählen_ und wähle _Betaflight STM32_ aus. Anschließend kannst du auf _Verbinden_ (2) drücken.

![Image](/rsc/01_img/05_FlightControllerSetup/ESCConfiguratorStartPage.png)

Drücke dann _Einstellungen lesen_ (3), um die aktuellen Parameter der Motoren auszulesen. Wenn hier ein Fehler auftritt oder die Einstellungen einfach nicht ausgelesen werden, dann empfiehlt sich mittels _Zadig_ etwaige fehlende Treiber nochmals zu installieren (siehe [Installation Software und Treiber](/docs/01_Materials.md#installation-betaflight-konfigurator)).

![Image](/rsc/01_img/05_FlightControllerSetup/ESCConfiguratorReadSettings.png)

Im nächsten Fenster werden wir nun die eigentlichen Einstellungen vornehmen. Wundere dich nicht, wenn bei dir die angezeigten Werte/Parameter noch nicht mit dem Fenster aus dem Screenshot übereinstimmen, wir werden diese erst noch einstellen. Zuerst musst du aber noch die richtige Firmware auf die ESCs flashen. Drücke auf _Alle flashen_ (4), um also alle vier ESCs zu flashen.

![Image](/rsc/01_img/05_FlightControllerSetup/ESCConfiguratorFlashAll.png)

Im Fenster, das sich dann öffnet, wählst du in den Dropdown-Menüs (5) für _Firmware_, _ESC_, _Version_ und _PWM Frequency_ die Einträge aus dem Bild unten aus und drückst dann auf _Flashen_ (6).

![Image](/rsc/01_img/05_FlightControllerSetup/ESCConfiguratorFlashSettings.png)

Das Fenster wird dann wieder auf das vorherige zurückspringen und du kannst beobachten wie die ESCs nacheinander geflashed werden. (7)

![Image](/rsc/01_img/05_FlightControllerSetup/ESCConfiguratorFlashProgress.png)

Sobald die Buttons unten rechts nicht mehr ausgegraut sind, ist das Flashen beendet. Überprüfe, ob die Firmware der ESCs bei dir genauso lautet wie in (8), dann kannst du fortfahren. Jetzt musst du jeden einzelnen Parameter auf der linken Seite (9) auf die Werte im Screenshot anpassen. Bist du fertig, dann drücke _Einstellungen schreiben_ (10), um die Parameter auf den ESCs zu speichern.

![Image](/rsc/01_img/05_FlightControllerSetup/ESCConfiguratorSettings.png)

Schließe den Browser und öffne den _Betaflight Configurator_. Verbinde dich mit dem Flight Controller und klicke auf den Reiter _Motoren_ (11). Was wir jetzt noch anpassen müssen, ist die Standard-Drehrichtung der Motoren. Du kannst dich dabei an der Grafik (12) orientieren.Um herauszufinden, wie die Motoren aktuell drehen, wirst du nacheinander die Motoren ganz leicht drehen lassen. Du wirst einen kleines Stück Papier vorsichtig in die Propeller halten. Anhand dessen, in welche Richtung das Papier dabei vom Propeller gedrückt wird, kannst du erkennen in welche Richtung der Propeller dreht. Versuch nicht, es nur mit bloßem Auge ohne den Trick mit dem Stück Papier zu erkennen. Man vertut sich leider sehr schnell, was dann aber einen stabilen Flug der Drohne unmöglich macht.

**Wichtig:** Achte darauf keine Haare/Schals/Finger/o.ä. in die Propeller zu halten, während sie sich drehen oder generell während der Akku der Drohne angesteckt ist.

Um die Motoren einzeln drehen zu lassen musst du den Schalter (13) aktivieren. Achtung: Ab jetzt sind die Motoren aktiviert! Entgegen dem Hinweis in dem Kasten darüber entfernen wir nicht die Propeller. Sie sind erstens sehr klein, daher ist das Verletzungsrisiko generell nicht ganz so groß, wie bei größeren Drohnen. Zwei-tens sind auch die Achsen der Motoren, auf denen die Propeller aufgesteckt sind, sehr klein, weshalb sie nicht so geeignet sind, um die Propeller oft auf- und abzustecken.

Bewege nun einzeln die Regler (14) **vorsichtig** nach oben, bis sich der jeweilige Motor **langsam (nicht mehr!)** dreht und befolge die Schritte mit dem Papierstück von oben. Markiere in der Grafik (12) z.B. mit einem Kreuz, welche(n) der Motoren du umkehren musst, damit sie in die richtige Richtung drehen.

![Image](/rsc/01_img/05_FlightControllerSetup/BetaflightMotors.png)

![Image](/rsc/01_img/05_FlightControllerSetup/SpinDirectionTest.png)

Wenn du herausgefunden hast, welche Motoren du umkehren musst, dann drücke Motoren stoppen (15) und schließe den Betaflight Configurator. Öffne wieder Microsoft Edge, verbinde dich im ESC Configurator mit der Drohne und lies die Einstellungen aus. Jetzt solltest du wieder auf der Seite von zuvor sein. Es bleibt nun nur noch die Motoren, die du eben ermittelt hast, zu reversen (16).

**Wichtig:** Hier musst du **deine** Konfiguration übernehmen. Es könnten bei dir also beispielsweise auch die Motoren 1&2 oder 2&4 _reversed_ sein.

Zum Schluss musst du nur noch die _Einstellungen schreiben_ (17). Um sicherzugehen, kannst du die Steps im _Betaflight Configurator_ wiederholen und überprüfen, ob sich die Motoren jetzt in die richtige Richtung drehen.

![Image](/rsc/01_img/05_FlightControllerSetup/ESCConfiguratorReverse.png)

# Konfiguration Empfangsmodul

Bevor wir zum Jungfernflug deiner Drohne kommen können, ist der letzte Schritt noch das Empfangsmodul zu konfigurieren. Den Akku kannst du wieder von der Drohne trennen. Er ist nur nötig, um die Motoren drehen zu lassen. Für alles andere genügt die Spannungsversorgung per USB. Analog zur [Konfiguration Übertragungsmodul](/docs/03_RemoteSetup.md#konfiguration-übertragungsmodul) verwenden wir wieder den _ExpressLRS Configurator_. Achte darauf, dass sowohl _Betaflight Configurator_ und _ESC Configurator_ geschlossen, sowie außerdem die Fernbedienung ausgeschaltet ist.

Schließe die Drohne per USB-Kabel am PC an. Öffne den _ExpressLRS Configurator_. Triff dort die Einstellungen (1,2,3) so wie im untenstehenden Screenshot. Sobald du das getan hast, sollten die meisten der Einstellungen im roten Kasten (4) automatisch richtig erscheinen. Falls sie das nicht tun, korrigiere sie bitte entsprechend. Lediglich bei der _Binding Phrase_ (5) musst du aufpassen. Hier gilt es dieselbe Binding Phrase einzutragen, die du im Übertragungsmodul der Fernbedienung (siehe [Konfiguration Übertragungsmodul](/docs/03_RemoteSetup.md#konfiguration-übertragungsmodul)) vergeben hast!

![Image](/rsc/01_img/05_FlightControllerSetup/ExpressLRSFlightController1.png)

![Image](/rsc/01_img/05_FlightControllerSetup/ExpressLRSFligthController2.png)

Sobald du alle Einstellungen getroffen hast, musst du nur noch auf _Auf Gerät Installieren_ (6) drücken. Dann startet die Installation und wird am Ende mit Operation erfolgreich abgeschlossen quittiert. Kommt es zu Fehlern, liegt es wahrscheinlich an fehlenden Treibern, die du per _Zadig_ nachinstallieren kannst (siehe [Installation Software und Treiber](/docs/01_Materials.md#installation-betaflight-konfigurator)). Kontrolliere außerdem, ob alle anderen Programme geschlossen sind und der richtige COM-Port ausgewählt ist.

Du kannst den _ExpressLRS Configurator_ jetzt schließen.

Stecke die Drohne vom PC ab und dann wieder an. So triggerst du ein erneutes Suchen nach Fernbedienungssignalen. Schalte auch die Fernbedienung wieder an. Sie sollte sich nun automatisch mit dem Empfangsmodul auf dem Flight Controller verbinden.

Als Check, ob alles geklappt hat, solltest du jetzt nochmal den _Betaflight Configurator_ öffnen. Verbinde die Drohne genauso, wie du es mittlerweile schon kennst. Im Reiter _Empfänger_ (7) solltest du in den Balken (8) jetzt die Änderungen der Werte live verfolgen können, wenn du die Sticks auf der Fernbedienung bewegst.

![Image](/rsc/01_img/05_FlightControllerSetup/FlightControllerRemoteTest.png)


## [Klicke hier, um zurück zur Übersicht der Kapitel zu kommen!](/README.md#kapitel)