---
title: "CTI-Client"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "endgeraete"
weight: 511
toc: true
---

Über Computer Telephony Integration (CTI) bedienen Sie Telefone von Ihrem PC aus und können damit zum Beispiel per Mausklick Anrufe annehmen oder Rufnummern wählen. Bei der NetCologne Cloud PBX nutzen Sie dazu eine externe Software, einen CTI-Client.


#### Voraussetzungen für den PhoneSuite CTI Client

Es müssen folgende Voraussetzungen erfüllt sein, damit die Installation gemäß u.a. Anleitung erfolgen kann:

Der PC läuft mit einem Windows-Betriebssystem.

Es ist keine systemfremde Firewall (außer Windows) installiert.

Das anzubindende Telefon hat eine statische IP-Adresse, die in der CTI-Software eingetragen werden muss.

Das entsprechende Telefon hat eine statische IP-Adresse. Diese muss in der CTI-Software eingetragen werden.

#### Installation des PhoneSuite CTI Clients

[1] Laden Sie die Software auf der Website des Herstellers herunter: https://www.phonesuite.de/de/download.htm.<br>
[2]	Führen Sie die Setup.exe aus.<br>
[3]	Folgen Sie dem Installationsprozess und wählen Sie dabei die korrekte Lizenzversion (hier: Professional).<br>
[4]	Installieren Sie nach Bedarf "ActiveX", "Outlook" und "CTI Client TAPI Connector" mit.<br>
![phonesuite Installation](https://user-images.githubusercontent.com/98753538/154282695-07121521-4dd6-45c2-a66a-0c0502c30c1c.jpg)
[5]	Klicken Sie auf "Weiter" und führen Sie die Installation zu Ende.<br>
[6] 6.	Starten Sie "Phone Suite CTI Client" über das Windows-Startmenü.<br>
![phoneSuite_Start](https://user-images.githubusercontent.com/98753538/154282861-d6c26fca-6760-466a-80b2-62cbbe989b77.jpg)

#### Einrichtung des PhoneSuite CTI Clients

![phoneSuite Einrichtung1](https://user-images.githubusercontent.com/98753538/154283706-a1b91ce8-7d6f-4d88-858a-0e2fa3136c0b.jpg)
[7]	Klicken Sie im Menü "Optionen" auf den Punkt "PhoneDialog (TAPI-Gerät)".<br>
![phoneSuite Tapi auswählen](https://user-images.githubusercontent.com/98753538/154283893-db566f8e-96e4-4d01-8ab4-e1a0fb40c49c.jpg)
[8]	Klicken Sie im sich daraufhin öffnenden Fenster auf "TAPI-Gerät auswählen".<br>
![phoneSuite Yeahlink auswählen](https://user-images.githubusercontent.com/98753538/154284087-ee1e3d86-1f91-4a69-a9d4-2dc52d5dadfd.jpg)
[9]	Wählen Sie aus der Auswahl "snom Phones" oder "Yealink Phones" aus.<br>
