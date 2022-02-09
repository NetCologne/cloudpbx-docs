---
title: "Analoge Telefon Adapter"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "endgeraete"
weight: 504
toc: true
---

## Grandstream HT-814

Schließen Sie zuallererst Ihren Grandstream am Stromnetz und an Ihr Netzwerk an. Verbinden Sie dann das Gerät mit einem analogen Telefon via der Phone-Buchse.

<img src="/images/ht814.jpg" alt="HT-814"/>

#### Zugangsdaten und Firmeware

Das Grandstream HT-814 wird nicht automatisch provisioniert. Die Konfiguration ist daher selbst vorzunehmen.
Der Zugriff auf das WebInterface erfolgt über einen Web Browser mit http://IPAdresse, wobei die IP Adresse im lokalen Router ausgelesen werden kann:

![ATA_Login](https://user-images.githubusercontent.com/98472426/153013541-d360ff56-54ea-46d5-a651-2adefb915fc2.jpg)

Username und Password lauten beide "admin".

Im Menue "Grandsteam Device Configuration" überprüfen Sie bitte im Tab "Status", ob die aktuelle Firmware installiert ist.

![ATA Firmware](https://user-images.githubusercontent.com/98753538/152983105-1f5072ca-d8e5-4329-beb8-d8fb86408a5b.jpg)

https://firmware.grandstream.com/Release_Note_HT812_HT814_1.0.33.4.pdf

Weitere Informationen zum Firmwareupdate und die entsprechenden Downloads finden sich auf der Grandstream Seite: http://www.grandstream.com/support/firmware

Wechseln Sie in der Navigationsleiste auf den Reiter „Advanced Settings“ und scrollen bis zum Ende der Seite. Unter dem Punkt „Upload Firmeware“ können Sie die zuvor abgelegte Firmware auswählen und hochladen.
Mit "Export Backup Configuration" können Sie ein Backup Ihrer aktuellen Konfiguration erstellen (entfällt bei neu zu installierenden Geräten). Unter dem Punkt „Upload Configuration“ können Sie eine neue Konfiguration hochladen: Sie wählen den lokalen Pfad zu der gewünschten Konfigurations-Datei aus und klicken auf „Upload Configuration“.

#### Basic Settings

Beachten Sie die Voreinstellung von 10 Minuten beim Session Timeout.

![ATA Basic Setting](https://user-images.githubusercontent.com/98753538/152987589-de064f81-9a80-4af9-855b-2c678c5df960.jpg)

Wählen Sie die entsprechende Zeitzone und bestätigen am unteren Menueende mit "Apply". 

#### Advanced Settings

![ATA Advanced Setting 1](https://user-images.githubusercontent.com/98753538/152993085-9e822078-d8b2-4fb8-927c-45a2c5a59ae2.jpg)

![ATA Advanced Setting 2](https://user-images.githubusercontent.com/98753538/152993341-9497468f-470e-4dba-b2d0-48700a6d5cc1.jpg)

![ATA Advanced Setting 3](https://user-images.githubusercontent.com/98753538/152994356-9c31fc26-4820-4302-8472-e4911f4105d4.jpg)

###### Call Progress Tones

* Dial Tone>>>>>>>>>>>>>>>>>f1=425@-10,c=0/0;
* Ringback Tone>>>>>>>>>>>>>>f1=425@-12,c=1000/4000;
* Busy Tone>>>>>>>>>>>>>>>>>f1=425@-12,c=500/500; 
* Reorder Tone>>>>>>>>>>>>>>>f1=425@-12,c=220/220; 
* Confirmation Tone>>>>>>>>>>>f1=425@-11,f2=440@-11,c=100/100-100/100-100/100; 
* Call Waiting Tone>>>>>>>>>>>>f1=425@-10,c=220/220-220/220-0/0; 
* Prompt Tone>>>>>>>>>>>>>>>f1=425@-17,f2=440@-17, c=0/0; 
* Conference Party Hangup Tone>>>f1=425@-15,c=600/600; 

Übernehmen Sie die entsprechenden Einstellungen und bestätigen am unteren Menueende mit "Apply". 

#### Profile 1

![ATA Profile 1a](https://user-images.githubusercontent.com/98753538/152995771-2222ab95-cb9d-4a48-b043-6972b732f5a3.jpg)

![ATA Profile 1b](https://user-images.githubusercontent.com/98753538/152997833-82a5f4b8-bb80-404a-98b7-8c020d76ea02.jpg)

![ATA Profile 1c](https://user-images.githubusercontent.com/98753538/152997853-ade99b8d-a752-4e7c-867b-46c3ad457fac.jpg)

![ATA Profile 1d](https://user-images.githubusercontent.com/98753538/152998051-436127e7-19e8-4b02-989f-059c88f43d0b.jpg)

![ATA Profile 1e](https://user-images.githubusercontent.com/98753538/153001884-9cc66e53-7e67-4e8f-b5b6-5832479ad4e1.jpg)

![ATA Profile 1f](https://user-images.githubusercontent.com/98753538/153002274-b6b3e96b-891d-4887-a56f-807001b48d7f.jpg)

Übernehmen Sie die entsprechenden Einstellungen und bestätigen am unteren Menueende mit "Apply". 

#### FXS Ports

![ATA FXS Ports](https://user-images.githubusercontent.com/98753538/153131122-84c31339-ff01-4c23-97e7-615006551e4b.jpg)

Unter *SIP User ID*, *Authenticat ID*, *Name* und *Request URI Routing ID* tragen Sie den Sip Usernamen der in der Cloud PBX eingerichteten Nebenstelle ein.

Das einzutragende *Passwort* ist das zugehörige SIP Password der Nebenstelle aus der Cloud-PBX.

Mit der *Profile ID* wählen Sie das entsprechende Profil aus. *Profile 1* könnte ein Profil für ein **analoges Telefon** sein, während *Profile 2* die Einstellungen für ein **Fax** beinhaltet. 

Zu den Unterschieden in den Profilen bzgl. Fax und analogem Telefon, beachten Sie bitte die Anmerkungen in den Abbildungen unter **Profile 1**.

Übernehmen Sie die entsprechenden Einstellungen und bestätigen am unteren Menueende mit "Apply". 



