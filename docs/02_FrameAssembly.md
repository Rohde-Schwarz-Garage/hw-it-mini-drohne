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


