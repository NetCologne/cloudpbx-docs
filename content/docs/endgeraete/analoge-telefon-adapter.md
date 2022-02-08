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
Über die IP-Adresse (hier 87.78.68.220), die man z.B. in der Fritzbox auslesen kann, und den Portzusatz ":49080" gelangt man auf die GUI:

![ATA Login](https://user-images.githubusercontent.com/98753538/152982361-ef730222-a9e8-49ac-bb52-665fc1d45da0.jpg)

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

Übernehmen Sie die entsprechenden Einstellungen und bestätigen am unteren Menueende mit "Apply". 

#### Profile 1

![ATA Profile 1a](https://user-images.githubusercontent.com/98753538/152995771-2222ab95-cb9d-4a48-b043-6972b732f5a3.jpg)




