---
title: "Unify"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "endgeraete"
weight: 504
toc: true
---

Die Marke Unify bietet mehrere Modelle, die mit dem NetCologne Cloud PBX funktionieren. Wir zeigen Ihnen, wie Sie einzelne Geräte mit Ihrer virtuellen Telefonanlage einrichten.

Achtung: Die automatische Konfiguration ist mit den SIP-Modellen von Unify zurzeit noch nicht möglich. Deshalb zeigen wir Ihnen die manuelle Einrichtung.

## OpenScape Desk Phone CP200

<img src="/images/cp200.jpg" alt="CP200"/>
  
Grundsätzlich können nur Endgeräte mit SIP Protokoll betrieben werden. Wenn das zu konfigurierende Telefon noch mit einer HFA Firmware ausgerüstet ist, muss zunächst ein Firmware Upgrade auf eine SIP fähige Firmware durchgeführt werden.  
Ein entsprechendes Image kann [hier](https://hipath.tonidoid.com/ui/core/index.html#expl-tabl.G:%5CTonido%5CShared%5COpenScape%20Desk%20Phone%20CP%5CSIP%5CDesk%20Phone%20CP20x%20SIP%20V1/ "Login als guest, User und PW hipath4000") heruntergeladen werden.

![DownloadImage](https://user-images.githubusercontent.com/98472426/151367270-09e12db5-0af5-4072-b640-36c99ddb7419.jpg)

Das File „CP20X_SIP_V1_R9_2_0.img“ bitte herunterladen und auf einem PC speichern, der im gleichen Netz hängt, wie die upzudatenden Endgeräte.   
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

![SystemIdentity](https://user-images.githubusercontent.com/98472426/151368099-9476679e-af1f-40f7-87cd-0c205a550a6a.jpg)  

* Konfiguration des SIP Interfaces  

![SIPInterface](https://user-images.githubusercontent.com/98472426/151368295-d115b93d-9778-410d-bdd8-5dec94804a67.jpg)  

* sRTP Konfiguration  

![srtpConfig](https://user-images.githubusercontent.com/98472426/151368420-1bf924f0-b3ae-46ac-91cd-5116b690b5a6.jpg)  

Damit ist das Telefon für abgehende und ankommende Telefonie nutzbar. Die Konfiguration von Kurzwahltasten ist über das WebInterfaces der Telefone möglich. 

