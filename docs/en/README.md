# IPSymconPowerfox
[![Version](https://img.shields.io/badge/Symcon-PHPModul-red.svg)](https://www.symcon.de/service/dokumentation/entwicklerbereich/sdk-tools/sdk-php/)
[![Version](https://img.shields.io/badge/Symcon%20Version-5.0%20%3E-green.svg)](https://www.symcon.de/forum/threads/37412-IP-Symcon-5-0-%28Testing%29)

Module for IP-Symcon from version 5. Allows communication with [powerfox](https://www.powerfox.energy) devices.

## Documentation

**Table of Contents**

1. [Features](#1-features)
2. [Requirements](#2-requirements)
3. [Installation](#3-installation)
4. [Function reference](#4-functionreference)
5. [Configuration](#5-configuration)
6. [Annex](#6-annex)

## 1. Features

Read data from [powerfox](https://www.powerfox.energy) devices via powerfox API. 
	  
## 2. Requirements

 - IPS 5.2
 - powerfox account
 - [powerfox poweropti](https://www.powerfox.energy)

## 3. Installation

### a. powerfox customer account and poweropti

At [powerfox energy](https://poweropti.powerfox.energy/) or through one of the numerous powerfox partners you can
acquire the poweropti.

Pay attention to the list of supported meters: [Meter overview](https://poweropti.powerfox.energy/whiteliststromzaehler-poweropti-v16/).

If you have any problems or questions, the powerfox FAQ list will primarily help you:
[powerfox energy FAQ](https://poweropti.powerfox.energy/faq/).

Before you can activate the poweropti, you must have a powerfox account using the powerfox
Create an app, which consists of an email address and password. powerfox only gives the length of
at least 8 and a maximum of 42 characters.

You can get the apps in the respective stores:

 Android: [powerfox energy App Android](https://play.google.com/store/apps/details?id=energy.powerfox.power42&hl=de)

 iOS: [powerfox energy App iOS](https://apps.apple.com/us/app/powerfox/id1386630652)

After registering the powerfox account, you can activate your poweropti so that it is your
Can read out the counter. The data is processed in the powerfox cloud solution and is available in the long term
At your disposal. Please make sure that you are transferring the data in the powerfox app
have activated. Otherwise, unfortunately, no data can be retrieved via the API.

### b. Loading the module

Open the IP Console's web console with _http://{IP-Symcon IP}:3777/console/_.

Then click on the module store (IP-Symcon > 5.2) icon in the upper right corner.

![Store](img/store_icon.png?raw=true "open store")

In the search field type

```
Powerfox
```  
https://www.powerfox.energy/download/

![Store](img/module_store_search_en.png?raw=true "module search")

Then select the module and click _Install_

![Store](img/install_en.png?raw=true "install")


### c. Setup of the configurator module and io

Enter the powerfox user name and the powerfox password in the powerfox IO instance.

![powerfox io](img/powerfox_io.png?raw=true "powerfox io")


Now we change in the object tree to the instance _ ** powerfox ** _ (type powerfocx configurator) to be found under _Configurator Instances_.

All devices that are registered with powerfox under the account and supported by the powerfox API are listed here.

A single device can be created by marking it on the device and pressing the button _Create_. The configurator then creates a device instance.

![powerfox config](img/powerfox_config.png?raw=true "config")


### e. Device instance setup
Manual configuration of a device module is not necessary, this is done using the configurator. Individual variables can still be activated in the device module for display on the web front if required.

If you want to record the data, select _Counter_ as the type

![zaehler](img/Archiv_Zaehler.png?raw=true "counter")

## 4. Function reference

### a. Webfront View

![webfront 1nstance](img/powerfox_webfront_1.png?raw=true "instance")

![powerfox graph 2](img/powerfox_webfront_graph_1.png?raw=true "graph")

![powerfox graph 2](img/powerfox_webfront_graph_2.png?raw=true "graph 2")


## 5. Configuration:




## 6. Annnex

###  GUIDs und Data Flow:

#### powerfox IO:

GUID: `{47E17935-CBB5-02B3-BAA3-7CD681898DBC}`


#### powerfox Device:

GUID: `{70960788-E771-65EE-C6B5-1B877771B987}` 
