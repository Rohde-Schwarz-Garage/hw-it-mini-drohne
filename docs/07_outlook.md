# Möglichkeiten zum Ausbau des Projekts
![image](https://github.com/Rohde-Schwarz-Garage/.github/blob/main/ressources/graphics/2024_03_13_Trennbanner_GitHub_Grey_Transparent.png?raw=true)

## Anpassung der Rates in Betaflight

>Die Rates legen fest, wie schnell die Drohne auf deinen Steuerbefehl reagiert und ein Kippen (Pitch), Rollen (Roll) oder eine Drehung um die eigene Achse (Yaw) vollzieht. Dabei ist die Höhe der Rates proportional zu der Geschwindigkeit, mit der die Drohne diese Bewegungen ausführt. Hohe Rates führen dazu, dass die Drohne schneller in die gewünschte Richtung kippt, rollt oder um die eigene Achse dreht, während geringere Rates entsprechend langsamere Bewegungen bewirken.

>Es ist wichtig zu beachten, dass höhere Rates zwar schnelle und akrobatische Manöver ermöglichen, sie erfordern jedoch auch ein entsprechendes Maß an Erfahrung und Kontrolle beim Fliegen. Anfänger sollten daher eher mit niedrigeren Rates starten und diese langsam steigern, je sicherer sie im Umgang mit der Drohne werden. 

Das Anpassen der Rates ist im *Betaflight Configurator* möglich. Verbinde dazu die Drohne mit deinem Rechner und wechsle in den PID Tuning Tab (1). Dort kannst du in dem Reiter „Ratenprofile anpassen“ (2) Anpassungen an den „RC-Rates“ (3) vornehmen. Vergiss anschließend nicht die Änderungen zu speichern.

![Image](/rsc/01_img/07_Outlook/BetaflightRates.png)

Es wird empfohlen, die Rates schrittweise um 0,05 zu erhöhen und anschließend ausgiebig zu testen, wie sich das Flugverhalten deiner Drohne verändert und ob dir dies gefällt.


## Erste Versuche den Acro-Modus zu bändigen

>Die Steuerung im Level Mode und Acro Mode unterscheidet sich tatsächlich erheblich und beeinflusst das Verhalten und die Reaktionsweise der Drohne auf die Eingaben des Piloten.

>Im Angle Mode versucht die Drohne, ihre Nivellierung beizubehalten. Wenn du einen Steuereingriff ausführen, etwa eine Neigung nach links oder rechts, wird die Drohne nach links oder rechts neigen, aber sobald du den Steuerknüppel freigibst, wird die Drohne automatisch in eine flache, horizontale Position zurückkehren. Dieser Modus versucht, die Drohne stets stabil und ausgeglichen zu halten, was ihn ideal für Anfänger oder für Situationen macht, in denen Stabilität und einfache Steuerung wichtig sind.

>Der Acro Mode hingegen ist viel direkter und bietet dem Piloten volle Kontrolle über die Drohne. In diesem Modus wird die Drohne nicht automatisch stabilisiert oder auf eine horizontale Position zurückgesetzt. Stattdessen bleibt die Drohne in der Position, in die du sie gebracht hast. Wenn du also den Steuerknüppel loslässt, nachdem du die Drohne in eine Neigung versetzt hast, bleibt sie in dieser Neigung und kehrt nicht automatisch in die horizontale Position zurück. Dies erfordert mehr Geschick durch den Piloten, ermöglicht aber auch mehr Kontrolle und Flexibilität bei der Durchführung von Manövern.

**Einrichten des Acro-Modus:**

1.	Schalte die Fernsteuerung an und verbinde anschließend die Drohne mit dem Betaflight-Konfigurator

2.	Wechsle in den Modi-Tab im Konfigurator. Hier wählst du zuerst „Nicht benutze Modi ausblenden“ (1) aus und du solltest dann „ANGLE“ sehen.

    ![Image](/rsc/01_img/07_Outlook/BetalfightModesStart.png)

3.	Stelle nun die Schaltfläche, die mit „AUX“ (2) beginnt, auf „AUTO“ um und raste die rechte Schultertaste der Fernsteuerung ein. Die Schaltfläche sollte nun auf einen neuen AUX-Kanal umgesprungen sein. Wenn dies nicht der Fall ist, stelle sicher, dass die Fernsteuerung mit der Drohne verbunden ist.

    ![Image](/rsc/01_img/07_Outlook/BetaflightUsedModes.png)

4.	Raste die rechte Schultertaste nun wieder aus und beobachte, wie sich die kleine gelbe Markierung unter dem Balken verschiebt. Ziehe den darüberliegenden Kasten nun so zurecht, dass er die kleine gelbe Markierung umschließt.

    ![Image](/rsc/01_img/07_Outlook/BetalfightModeRange.png)

5.	Klicke auf „Speichern“. 

Jetzt kannst du den Acro-Modus aktivieren, indem du die rechte Schultertaste einrastest! Die Beherrschung dieses Flugmodus benötigt sehr viel Geduld und Übung. Es ist zu empfehlen zuerst in einem Simulator am PC oder einer Spielekonsole zu üben. Mehr zu Simulatoren findest du unter weiterführende Quellen. 


## FPV - ein völlig neues Erlebnis

FPV steht für "First Person View", was bedeutet, dass Piloten den Flug ihrer Drohne aus der Vogelperspektive verfolgen können. Dies wird erreicht, indem ein Live-Video-Feed von der Kamera der Drohne direkt zu einem Bildschirm, einer Videobrille, oder einem anderen Display-Gerät des Piloten übertragen wird.

Traditionelle Drohnen werden oft "VLOS" (Visual Line of Sight) geflogen, was bedeutet, dass der Pilot die Drohne ständig im Auge behält und sie aus seiner eigenen Perspektive steuert. Das kann Limitationen mit sich bringen, besonders wenn die Drohne außer Sichtweite gerät oder wenn der Pilot die Ausrichtung der Drohne nicht genau bestimmen kann.

FPV-Systeme nutzen verschiedene Technologien, um das Video von der Drohne zum Piloten zu übertragen. Aktuell werden zwei Methoden unterschieden: analoge und digitale Übertragung.

Analoge FPV-Systeme sind die ältere Technologie und sind wegen ihrer niedrigen Latenz und ihrer robusten Leistung unter schwierigen Bedingungen immer noch weit verbreitet. Sie übertragen das Videosignal ohne Buffering vom Sender in der Drohne zum Empfänger in der Bodenstation des Piloten. Die Qualität des Videosignals bei analogen Systemen ist generell schlechter als bei digitalen Systemen, aber die Verzögerung des Signals (die sogenannte Latenz) ist typischerweise sehr gering und konstant. Dies ist besonders wichtig beim Fliegen mit hohen Geschwindigkeiten oder bei komplexen Manövern, da selbst eine geringfügige Verzögerung zu einem Absturz führen kann.

Digitale FPV-Systeme dagegen bieten eine höhere Videoqualität, indem sie das Videosignal digital kodieren und übertragen. Das führt zu einem schärferen Bild mit mehr Details, was insbesondere bei komplexen Flugumgebungen oder beim Fliegen auf größere Distanzen nützlich sein kann. Aber digitale Systeme haben tendenziell eine höhere Latenz als analoge, was sie weniger geeignet für Rennsport oder Fliegen unter extremen Bedingungen macht. 

![Image](/rsc/01_img/07_Outlook/DigitalAnalogComparison.png)

Jüngste Entwicklungen in der FPV-Technologie zielen darauf ab, die hohe Bildqualität der digitalen Systeme mit der geringen Latenz der analogen Systeme zu kombinieren. Diese neuen Systeme verwenden fortschrittliche Kodierungstechniken und spezielle Hardware, um digitale Videoübertragungen mit minimalem Zeitverzug zu ermöglichen. Es gilt jedoch zu beachten, dass die digitalen Systeme in der Regel deutlich teurer sind als traditionelle analoge Systeme.

Wenn du mehr über FPV erfahren willst, kannst du dich in den weiterführenden Quellen nach Belieben informieren.


## Weiterführende Quellen

Wenn du gerne noch mehr über Drohnen und insbesondere FPV-Drohnen wissen möchtest können wir dir folgende Quellen herzlichst empfehlen:

### [How To Get Started With FPV Drones](https://oscarliang.com/fpv-drone-guide/)

Ein wunderbarer Blog, der in sehr gut recherchierten und umfassenden Texten alles um das Thema Drohnen erklärt. Seien es Tipps für den Einstieg, technische Hintergründe oder empfehlenswerte Produkte. Es ist ausdrücklich erwünscht auf der Seite zu stöbern!


### [Leran to fly an FPV drone](https://www.youtube.com/watch?v=SpuXqNakP2A&list=PLwoDb7WF6c8lCKhQOTy-Vb9LfW0VAIrTP)

Mit diesem Guide kannst du deine Flugfertigkeiten verfeinern. Nutze dazu einfach deine Fernsteuerung und schließe sie an deinem PC an. Schon kannst du in einem Simulator (mehr dazu später) üben, ohne echte Drohnen abstürzen zu lassen.

Joshua Bardwell ist in der Community hoch angesehen für seine informativen Videos und Tutorials. Stöbern lohnt sich also auch hier.


### [Liftoff® Simulator](https://store.steampowered.com/app/410340/Liftoff_FPV_Drone_Racing/)

Mit diesem Simulator kannst du in vielfältigen Umgebungen die unterschiedlichsten FPV-Drohnen fliegen und im Multiplayer Rennen fliegen. Die Simulatoren sind mittlerweile so gut, dass sich die Erfahrung problemlos auf echte Drohnen übertragen lässt.

Ein Simulator ist sehr gut angelegtes Geld. Jeden Unfall, den du im Simulator baust, spart dir Geld für Ersatzteile an einer echten Drohne.


### [quadmovr - YouTube](https://www.youtube.com/@quadmovr/videos)

Man braucht kein FPV um eine Drohne akrobatisch zu fliegen. Auf diesem YouTube-Kanal findest du beeindruckende und vielleicht sogar inspirierende Beispiele dafür.


### [EU Drohnenverordnung 2024](https://www.drohnen.de/47366/eu-drohnenverordnung-2024/)

Hier findest du gesetzliche Regelungen für den Umgang mit Drohnen. Du solltest dich mit diesen auseinandersetzen, bevor du im Freien fliegst.


## [Klicke hier, um zurück zur Übersicht der Kapitel zu kommen!](/README.md#kapitel)