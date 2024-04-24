# Vorbereitung Material und Software
![image](https://github.com/Rohde-Schwarz-Garage/.github/blob/main/ressources/graphics/2024_03_13_Trennbanner_GitHub_Grey_Transparent.png?raw=true)

In diesem Abschnitt findest du alles, was du benötigst, um dieser Anleitung folgen zu können. Die Links zu dem verwendeten Material findest du [hier](/docs/08_Links.md).


## Bauteile

![Image](/rsc/01_img/01_Materials/Parts.png)

| Bauteil                               | Anzahl | Nr.  |
|---------------------------------------|--------|------|
| Rahmen                                | 1      | 1    |
| Standfuß (zweiteilig)                 | 1      | 2    |
| Markierung rot                        | 1      | 3    |
| Markierung blau                       | 1      | 4    |
| Motoren (inkl. Schrauben)             | 4      | 5    |
| Propeller (Drehrichtung rechts)       | 2      | 6    |
| Propeller (Drehrichtung links)        | 2      | 7    |
| Flight Controller (FC) mit A30 Stecker| 1      | 8    |
| Gummi-Abstandshalter                  | 4      | 9    |
| Schrauben für Flight Controller       | 4      | 10   |
| R/S Deckplatte                        | 1      | 11   |
| Akku mit A30 Stecker                  | 2      | 12   |


## Verbrauchsmaterialien

![Image](/rsc/01_img/01_Materials/Materials.png)

| Material                       | Nr. |
|--------------------------------|-----|
| Schraubensicherung (Loctite)   | 1   |
| Uhu Kleber Extreme             | 2   |
| Doppelseitiges Klebeband       | 3   |


## Werkzeug und Zubehör

![Image](/rsc/01_img/01_Materials/Tools.png)

| Werkzeug                                                  | Nr. |
|-----------------------------------------------------------|-----|
| Werkzeugwagen (Schraubenzieher, Pinzetten, Zangen…)       | 1   |
| Ladegerät mit Netzteil                                    | 2   |
| Fernbedienung mit eingelegten 18650 Li-Ion-Batterien      | 3   |
| Kabel USB-A auf Micro-USB                                 | 4   |
| Lüfter                                                    | 5   |


# Software
![image](https://github.com/Rohde-Schwarz-Garage/.github/blob/main/ressources/graphics/2024_03_13_Trennbanner_GitHub_Grey_Transparent.png?raw=true)

| Software                                  | Link                                                             |
|-------------------------------------------|------------------------------------------------------------------|
| Betaflight Configurator (Version 10.9.0)  | [Klicke hier](https://github.com/betaflight/betaflight-configurator/releases) |
| ExpressLRS Configurator (Version 1.6.1)   | [Klicke hier](https://github.com/ExpressLRS/ExpressLRS-Configurator/releases) |
| ESC-Configurator WebUI                    | [Klicke hier](https://esc-configurator.com/)  |
| STM32 Virtual COM Port Driver             | [Klicke hier](https://www.st.com/en/development-tools/stsw-stm32102.html) |
| Zadig USB Driver Installer                | [Klicke hier](https://zadig.akeo.ie/)                |


## Installation Betaflight Konfigurator

Ab hier beginnt die Anleitung. Folge ihr Schritt für Schritt, um zum Schluss das gewünschte Ergebnis zu erzielen.  
> Generell versucht die Anleitung möglichst geradlinig zum Ziel „Du steuerst und fliegst die Drohne“ zu kommen. Wenn du aber verstehen möchtest, warum dabei gerade ein Schritt so gemacht wird, wie er gemacht wird, dann sind fast überall in der Anleitung eingerückte Kästen zu finden. Dort werden genau diese Hintergründe beleuchtet.


1.	Öffne den Link und lade die Version 10.9.0 in der passenden Version für dein Betriebssystem herunter (für 64bit Windows: betaflight-configurator_10.9.0_win64-installer.exe)

    ![Image](/rsc/01_img/01_Materials/BetaflightDownload.png)
2.	Führe die heruntergeladene Datei aus und folge den Anweisungen. Nach dem Fertigstellen kannst du den Konfigurator gleich wieder schließen, falls dieser sich geöffnet hat


## Installation ExpressLRS Konfigurator

1.	Öffne den Link und lade die Version 1.6.1 in der passenden Version für dein Betriebssystem herunter (für 64bit Windows: ExpressLRS-Configurator-Setup-1.6.1.exe)

    ![Image](/rsc/01_img/01_Materials/ExpressLRSDownload.png)
2.	Führe die heruntergeladene Datei aus und folge den Anweisungen. Nach dem Fertigstellen kannst du den Konfigurator gleich wieder schließen, falls dieser sich geöffnet hat


## Installation STM32 Virtual COM Port Treiber

1.	Öffne den Link zur Herstellerseite und klicke auf „Get Latest“

    ![Image](/rsc/01_img/01_Materials/STM32DriverDownload.png)
2.	Akzeptiere die Lizenzbestimmungen und klicke auf „Download as a guest“
3.	Nach dem Ausfüllen und Abschicken erhältst du eine E-Mail mit einem Download-Link. Mit diesem gelangst du wieder auf die Website und es wird automatisch ein komprimierter Ordner mit dem Treiber heruntergeladen
4.	Entpacke den ZIP-Ordner und führe „VCP_V1.5.0_Setup_W8_x64_64bits.exe“ aus, wenn du ein 64bit Betriebssystem mit mindestens Windows 8 hast
5.	Folge dem Wizard und denke dir einen schönen Firmennamen aus, damit du mit der Installation fortfahren kannst

    ![Image](/rsc/01_img/01_Materials/STM32Setup.png)
6.	Folge allen weiteren Anweisungen
7.	Starte deinen PC neu, damit der Treiber vollständig installiert ist


## Installation Zadig USB Treiber

1.	Öffne den Link und lade die neueste Version von Zadig herunter
2.	Wenn du an späteren Stellen in der Anleitung auf Probleme bei Installationen stößt, wirst du an diese Stelle verwiesen und kannst fehlende Treiber installieren.
3.	Öffne dafür die heruntergeladene zadig.exe und klicke auf „Install Diver“

    ![Image](/rsc/01_img/01_Materials/ZadigSetup.png)
4.	Sollte nach diesem Schritt es immer noch nicht funktionieren kannst du deinen PC neustarten.

## [Klicke hier, um zurück zur Übersicht der Kapitel zu kommen!](/README.md#kapitel)