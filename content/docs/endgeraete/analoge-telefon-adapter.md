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

# Zugangsdaten und Firmeware

Das Grandstream HT-814 wird nicht automatisch provisioniert. Die Konfiguration ist daher selbst vorzunehmen.
Über die IP-Adresse (hier 87.78.68.220), die man z.B. in der Fritzbox auslesen kann, und den Portzusatz ":49080" gelangt man auf die GUI:

![ATA Login](https://user-images.githubusercontent.com/98753538/152982361-ef730222-a9e8-49ac-bb52-665fc1d45da0.jpg)

Username und Password lauten beide "admin".

Im Menue "Grandsteam Device Configuration" überprüfen Sie bitte im Tab "Status", ob die aktuelle Firmware installiert ist.

![ATA Firmware](https://user-images.githubusercontent.com/98753538/152983105-1f5072ca-d8e5-4329-beb8-d8fb86408a5b.jpg)

https://firmware.grandstream.com/Release_Note_HT812_HT814_1.0.33.4.pdf

Weitere Informationen zum Firmwareupdate finden sich auf der Grandstream Seite: http://www.grandstream.com/support/firmware

Um eine Konfigurationsdatei hochzuladen, wechseln Sie in der Navigationsleiste auf den Reiter „Advanced Settings“. Scrollen Sie bis zum Ende der Seite und erstellen ein Backup Ihrer aktuellen Konfiguration. (Bei frisch installierten Geräten kann dieser Schritt auch übersprungen werden). Unter dem Punkt „Upload Configuration“ können Sie die neue Konfiguration hochladen. Hier wählen Sie lediglich den lokalen Pfad zu der gewünschten Konfigurations-Datei aus und klicken auf „Upload Configuration“.


