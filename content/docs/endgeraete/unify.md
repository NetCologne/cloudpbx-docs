---
title: "Unify"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "endgeraete"
weight: 510
toc: true
---

Die Marke Unify bietet mehrere Modelle, die mit der NetCologne Cloud PBX funktionieren. Wir zeigen Ihnen, wie Sie einzelne Geräte mit Ihrer virtuellen Telefonanlage einrichten.

Achtung: Die automatische Konfiguration ist mit den SIP-Modellen von Unify zurzeit noch nicht möglich. Deshalb zeigen wir Ihnen die manuelle Einrichtung.

## OpenScape Desk Phone CP200

<img src="/images/cp200.jpg" alt="CP200"/>
  
Grundsätzlich können nur Endgeräte mit SIP Protokoll betrieben werden. Wenn das zu konfigurierende Telefon noch mit einer HFA Firmware ausgerüstet ist, muss zunächst ein Firmware Upgrade auf eine SIP fähige Firmware durchgeführt werden. 
Um die entsprechende SIP Software zu erhalten, setzen sie sich bitte mit ihrem Anlagenbauer oder direkt mit Unify in Verbindung. 
   
Das Firmware Upgrade wird über das Web Interface der Telefone durchgeführt. Das Interface wird über die IP der Telefone erreicht. Das Hautproblem ist die IP des Telefons zu ermitteln. Im Idealfall lässt sich diese am Router auslesen.  
Der Zugriff auf das WebInterface erfolgt dann mit https://IPAdresse des Telefons. Der Admin Login für das Web Interface ist:

User:		    admin  
Passwort: 	123456  

(Falls benötigt – hier das Passwort zur Bestätigung eines Factory Resets: 124816)  

Anschließend kann dann der Firmware Upgrade durchgeführt werden (siehe Screenshot).  

![Firmware Upgrade](https://user-images.githubusercontent.com/98472426/151367590-a10cfa74-947c-4753-91e7-368ac61172a9.jpg)

Nach dem erfolgreichen Upgrade, müssen folgende Einstellungen am Endgerät durchgeführt werden:

* Port number Configuration  

![Port Number Config](https://user-images.githubusercontent.com/98472426/151367776-b2527eb0-3a7d-4cda-993e-2c35d2ce36cd.jpg)  

* Konfiguration der System Identity  

![SystemIdentity](https://user-images.githubusercontent.com/98472426/151382353-5d7c1eaa-9b76-4bcc-9dea-0224431d92c1.jpg)

* Konfiguration des SIP Interfaces  
  
![SIPInterface](https://user-images.githubusercontent.com/98472426/151382172-6e96d2b5-f897-4dc6-b143-0e1af0052c39.jpg)

* sRTP Konfiguration  

![srtpConfig](https://user-images.githubusercontent.com/98472426/151368420-1bf924f0-b3ae-46ac-91cd-5116b690b5a6.jpg)  

Damit ist das Telefon für abgehende und ankommende Telefonie nutzbar. Die Konfiguration von Kurzwahltasten ist über das WebInterfaces der Telefone möglich. 

