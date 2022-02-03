---
title: "Erste Schritte"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "konfiguration"
weight: 201
toc: true
---

Nun machen Sie sich mit Ihrer NetCologne Cloud PBX vertraut. In diesem Abschnitt erfahren Sie, wie Sie am besten bei der Konfiguration Ihrer Anlage vorgehen.

## Anmeldevorgang

Sie haben von uns ihre Login-Daten zur Konfiguration ihrer CloudPBX in folgender Form erhalten:

 Webseite: [https://myportal.cloudpbx.netcologne.de/v2](https://myportal.cloudpbx.netcologne.de/v2/ "Cloud-PBX Konfiguration")  
 Benutzer: `+49ONKZRufNr@firma.cloudpbx.netcologne.de`  
 Passwort: `xxxxxxxxxxxxxx`  

Auf der angebenen Seite können Sie sich mit diesen Daten anmelden

![CloudPBX-Login_cr](https://user-images.githubusercontent.com/98472426/151378584-db4a2417-cd21-4552-9dc7-313f3234a700.jpg)

Sie befinden sich nun in der Administrator-Maske der CloudPBX - hier können sie ihre Anlage konfigurieren:

![Schritt1-NST-einrichten](https://user-images.githubusercontent.com/98472426/151360917-a172d4b3-f9fa-4e63-9fc1-ee0aa02177ec.jpg)

## Einrichtung von Nebenstellen 

Nebenstellen werden für jegliche Funktion der Anlage benötigt, selbst wenn dahinter kein physikalischer Anschluss steckt. Hinter Nebenstellen können folgende Funktionen konfiguriert werden:

* Physikalische Anschlüsse wie Telefone oder SIP Clients
* Anrufbeantworter
* Faxserver
* ACD/IVR

Die entsprechende Funktion wird über Weiterleitung der Nebenstelle auf die entsprechende Funktion realisiert. Weiterleitungen sind also nicht nur auf physikalische Ziele möglich, sondern auch auf die o. a. Funktionen. 
Hier wird nun die Nebenstelle 10 für den User max eingerichtet:

![Schritt2-NST-einrichten](https://user-images.githubusercontent.com/98472426/151360059-00894ef1-789f-40ca-8a79-50c51eb1657f.jpg)

![Schritt3-NST-einrichten](https://user-images.githubusercontent.com/98472426/151360126-9c9fc7ef-8c7d-4a0c-9041-799d06bc641c.jpg)

Das Web Passwort wird benötigt, wenn der User der Nebenstelle per Web Interface seine Nebenstelle konfigurieren können soll – also Anrufweiterschaltungen, Kurzwahlen etc. einrichten können soll. 
Das SIP Passwort ist erforderlich, wenn Endgeräte – also Telefone oder Sip Clients etc. – manuell provisioniert werden sollen. Grundsätzlich kann, sowohl der Administrator als auch der User die entsprechenden Passwörter ändern und dabei dann auch wieder einsehen. 
Der folgende Screenshot zeigt, wie die Passwörter geändert werden – hier wurden bereit 3 Nebenstellen konfiguriert. 

![Ändern NST](https://user-images.githubusercontent.com/98472426/151360446-3d90ea15-3cfa-4651-b644-baec80a2c62d.jpg)



