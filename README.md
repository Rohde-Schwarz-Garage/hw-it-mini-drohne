# BAUEN EINER KLEINEN DROHNE :helicopter:
<!--- Trennbalken bei Überschriften Level 1 (#) + kann kopiert werden --->
![image](https://github.com/Rohde-Schwarz-Garage/.github/blob/main/ressources/graphics/2024_03_13_Trennbanner_GitHub_Grey_Transparent.png?raw=true)

<!--- Hier kommt ein schönes Bild + ggf. mehr im Text --->
![image](/rsc/01_img/LandingPageFlying.jpg)
<!-- ![image](/rsc/01_img/LandingPage.jpg) -->



# Verantwortlichkeiten
<!--- Trennbalken bei Überschriften Level 1 (#) + kann kopiert werden --->
![image](https://github.com/Rohde-Schwarz-Garage/.github/blob/main/ressources/graphics/2024_03_13_Trennbanner_GitHub_Grey_Transparent.png?raw=true)

Ausbildung Fachinformatik, LJ2023

# Beschreibung
<!--- Trennbalken bei Überschriften Level 1 (#) + kann kopiert werden --->
![image](https://github.com/Rohde-Schwarz-Garage/.github/blob/main/ressources/graphics/2024_03_13_Trennbanner_GitHub_Grey_Transparent.png?raw=true)

In diesem Projekt wirst du eine kleine Drohne bauen. Dazu beschäftigst du dich mit dem Zusammenbau der Komponenten sowie der verwendeten Software und dem anschließenden Tuning. Das Endziel wird es sein, dass die Drohne eigenständig fliegt und von dir einfach gesteuert werden kann.

**Dauer des Projekts:** ca. 1 Arbeitstag, wenn du das Projekt vor Ort in der Garage machst

# Grundlegende Informationen
## Sicherer Umgang mit LiPo-Akkus

>Lithium-Polymer-Akkus, allgemein bekannt als LiPo-Akkus, sind die bevorzugte Energiequelle für die meisten Drohnen aufgrund ihrer hohen Energiedichte und ihrer Fähigkeit, hohe Stromstärken bereitzustellen. Diese Aspekte ermöglichen im Vergleich zu anderen Akkutypen eine längere Flugzeit und eine bessere Performance. 

>Obwohl LiPos viele Vorteile bieten, bringen sie auch spezifische Risiken mit sich. LiPo-Akkus sind sehr empfindlich gegenüber Fehlbehandlungen und können bei falscher Lagerung, falschem Laden oder Tiefentladung Schaden nehmen. Im schlimmsten Fall können diese Akkus sogar Feuer fangen oder explodieren. Daher sind beim Umgang bestimmte Sicherheitsmaßnahmen zu beachten.

### Wichtige Aspekte, die es zu befolgen gilt:

- **Aufladen:** Benutze immer ein Ladegerät, das speziell für LiPo-Akkus ausgelegt ist und lasse die Akkus während des Ladens nicht unbeaufsichtigt. Hier verwenden wird das VIFLY WhoopStor 3 Ladegerät. Bei diesem muss vor dem Aufladen eine **Ladespannung von 4,35V** und eine **Stromstärke von 0,5A** eingestellt werden.

    ![Image](/rsc/01_img/09_Safety/ChargerCharge.png)

- **Minimale Spannung:** Achte besonders auf die Akkuspannung während des Fliegens. Sollte die Spannung eines Akkus während des Fluges unter den kritischen Wert von 3,5 Volt fallen, muss die Drohne gelandet werden. Die Fernbedienung wird dir ein Warnsignal geben, sobald die Batterie leer ist. Ebenfalls lässt sich in dem „Telemetry-Display“ der Fernbedienung der Ladestand als Balken anzeigen

    ![Image](/rsc/01_img/09_Safety/RemoteTelemetry.png)

- **Lagerzeit:** Vermeide es, die Akkus über einen längeren Zeitraum (maximal 3 Tage) vollständig geladen oder entladen zu lagern, da dies ihre Leistungsfähigkeit und Lebensdauer erheblich beeinträchtigen kann.

- **Lagerspannung:** LiPo-Akkus sollten niemals vollständig geladen oder entladen gelagert werden. Eine optimale Lagerspannung liegt bei ca. 3,8 Volt pro Zelle. Dies bedeutet, dass du die Akkus nach jedem Flug entladen oder vor dem Lagern auf diese Spannung aufladen solltest, wenn du beabsichtigst die Akkus über einen längeren Zeitraum nicht herzunehmen. Dies geschieht mit der Einstellung einer 
**Ladespannung von 3,8V** und einer **Stromstärke von 0,5A**.

    ![Image](/rsc/01_img/09_Safety/ChargerStorage.png)

- **Sichere Lagerung:** Um das Risiko im Falle eines Batteriefehlers zu minimieren, solltest du die Akkus immer in einem feuerfesten Behältnis lagern. Dies dient dazu das Restrisiko zu minimieren. Optimal hierfür wäre ein Keramiktopf abgedeckt mit einem Teller. Der Lagerort sollte ebenfalls vor direkter Sonneneinstrahlung geschützt und trocken sein.

Durch Befolgen dieser Sicherheitstipps sorgst du für einen sicheren Umgang mit den LiPo-Akkus deiner Drohne, minimierst potenzielle Gefahren und verlängerst zugleich die Lebensdauer deiner Akkus.

## Was du nach dem Projekt nach Hause nehmen darfst

- Deine fertig gebaute Drohne
- **Einen** Akku (befolge unbedingt die Sicherheitshinweise)
- **In der Garage bleiben:** Ladegerät, Fernsteuerung und Werkzeug 


# Kapitel
<!--- Trennbalken bei Überschriften Level 1 (#) + kann kopiert werden --->
![image](https://github.com/Rohde-Schwarz-Garage/.github/blob/main/ressources/graphics/2024_03_13_Trennbanner_GitHub_Grey_Transparent.png?raw=true)

Um zu einer funktionierenden Drohne zu gelangen folge einfach den Kapiteln. Am Ende jedes Kapitels kommst du wieder auf diese Seite.

<!--- Weitere Indexe sind immer möglich --->
1. [Vorbereitung Material und Software](/docs/01_Materials.md)
2. [Zusammenbau Rahmen](/docs/02_FrameAssembly.md)
3. [Navigation und Einrichtung Fernsteuerung](/docs/03_RemoteSetup.md)
4. [Zusammenbau Drohne](/docs/04_DroneAssembly.md)
5. [Einrichtung Flight-Controller](/docs/05_FlightControllerSetup.md)
7. [Testen und Tunen der Drohne](/docs/06_TestingAndTuning.md)
8. [Möglichkeiten zum Ausbau des Projekts](/docs/07_Outlook.md)
9. [Links zu den verwendeten Bauteilen](/docs/08_Links.md)
10. [Sicherheitshinweise](/docs/09_Safety.md)