# IPSymconPowerfox
[![Version](https://img.shields.io/badge/Symcon-PHPModul-red.svg)](https://www.symcon.de/service/dokumentation/entwicklerbereich/sdk-tools/sdk-php/)
[![Version](https://img.shields.io/badge/Symcon%20Version-5.0%20%3E-green.svg)](https://www.symcon.de/forum/threads/38222-IP-Symcon-5-0-verf%C3%BCgbar)

Modul für IP-Symcon ab Version 5. Ermöglicht die Kommunikation mit einem powerfox poweropti.

## Dokumentation

**Inhaltsverzeichnis**

1. [Funktionsumfang](#1-funktionsumfang)  
2. [Voraussetzungen](#2-voraussetzungen)  
3. [Installation](#3-installation)  
4. [Funktionsreferenz](#4-funktionsreferenz)  
5. [Anhang](#5-anhang)  

## 1. Funktionsumfang

Auslesen der Messdaten eines [powerfox](https://www.powerfox.energy) Gerätes über die Powerfox API.




## 2. Voraussetzungen

 - IPS 5.2
 - powerfox Benutzerkonto
 - [powerfox poweropti](https://www.powerfox.energy)

## 3. Installation

### a. powerfox-Kundenkonto und poweropti

Unter [powerfox energy](https://poweropti.powerfox.energy/) oder über einen der zahlreichen Partner von powerfox können Sie
den poweropti erwerben.

Achten Sie dabei auf die Liste der unterstützten Zähler: [Zählerübersicht](https://poweropti.powerfox.energy/whiteliststromzaehler-poweropti-v16/).

Falls Sie Probleme oder Fragen haben hilft Ihnen in erster Linie die FAQ-Liste von powerfox weiter:
[powerfox energy FAQ](https://poweropti.powerfox.energy/faq/).

Bevor Sie den poweropti aktivieren können, müssen Sie ein powerfox-Konto mit Hilfe der powerfox-
App anlegen, welches aus E-Mailadresse und Passwort besteht. powerfox gibt lediglich die Länge von
mindestens 8 und maximal 42 Zeichen vor.

Die Apps erhalten Sie in den jeweiligen Stores:

 Android: [powerfox energy App Android](https://play.google.com/store/apps/details?id=energy.powerfox.power42&hl=de) 

 iOS: [powerfox energy App iOS](https://apps.apple.com/us/app/powerfox/id1386630652) 

Nach Registrierung des powerfox-Konto können Sie Ihren poweropti aktivieren, sodass dieser Ihren
Zähler auslesen kann. Die Daten werden in der powerfox Cloud-Lösung verarbeitet und stehen langfristig zu
Ihrer Verfügung. Bitte vergewissern Sie sich, dass Sie das Übertragen der Daten in der powerfox-App
aktiviert haben. Andernfalls lassen sich leider keine Daten über die API abrufen.

### b. Laden des Moduls

Die Webconsole von IP-Symcon mit _http://{IP-Symcon IP}:3777/console/_ öffnen. 


Anschließend oben rechts auf das Symbol für den Modulstore (IP-Symcon > 5.2) klicken

![Store](img/store_icon.png?raw=true "open store")

Im Suchfeld nun

```
Powerfox
```  

eingeben

![Store](img/module_store_search.png?raw=true "module search")

und schließend das Modul auswählen und auf _Installieren_

![Store](img/install.png?raw=true "install")

drücken.


### c. Einrichtung des Konfigurator-Moduls und der powerfox IO Instanz

In der powerfox IO Instanz in der powerfox Benutzername und das powerfox Passwort einzutragen.

![powerfox io](img/powerfox_io.png?raw=true "install")


Jetzt wechseln wir im Objektbaum in die Instanz _**powerfox**_ (Typ powerfocx Konfigurator) zu finden unter _Konfigurator Instanzen_.

Hier werden alle Geräte, die bei powerfox unter dem Account registiert sind und von der powerfox API unterstützt werden aufgeführt.

Ein einzelnes Gerät kann man durch markieren auf das Gerät und ein Druck auf den Button _Erstellen_ erzeugen. Der Konfigurator legt dann eine Geräte Instanz an.

![powerfox config](img/powerfox_config.png?raw=true "install")


### f. Einrichtung der Geräteinstanz
Eine manuelle Einrichtung eines Gerätemoduls ist nicht erforderlich, das erfolgt über den Konfigurator. In dem Geräte-Modul können noch einzelne Variablen bei Bedarf zur Anzeige im Webfront freigeschaltet werden.


## 4. Funktionsreferenz

### a. Webfront Ansicht

![Webfront](img/powerfox_webfront.png?raw=true "Webfront")  

![Webfront Graph](img/powerfox_webfront_graph.png?raw=true "Webfront Diagramm")

## 5. Konfiguration:



## 6. Anhang

###  GUIDs und Datenaustausch:

#### powerfox IO:

GUID: `{47E17935-CBB5-02B3-BAA3-7CD681898DBC}` 


#### powerfox Device:

GUID: `{70960788-E771-65EE-C6B5-1B877771B987}` 