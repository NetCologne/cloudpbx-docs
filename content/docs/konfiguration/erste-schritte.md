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

![cloudpbx_login](https://user-images.githubusercontent.com/98753538/152331121-be008d22-e8da-4997-88f2-47daf5f423f7.jpg)

Sie befinden sich nun in der Administrator-Maske der CloudPBX

![cloudpbx_dashboard1](https://user-images.githubusercontent.com/98753538/152346499-6842be07-6604-4428-be19-691e8e123992.jpg)

1. Das Dashboard liefert eine Überischt zu Nachrichten (Messages), Anrufen (Calls) und den registrierten Endgeräten.

2. Beim Punkt Konversationen stehen weitere Details wie "von" und "an".  
   Einrichtung der Nebenstellen klicken Sie bitte im Punkt "PBX-Konfiguration" auf  
3. "Seats" und fügen  
   ![cloudpbx_dashboard2-8](https://user-images.githubusercontent.com/98753538/152347008-0ad4c1fe-a492-4fd1-860c-2b355e903b0a.jpg)
4. Namen (nur Kleinbuchstaben, keine Leer- oder Sonderzeichen)

(5) Web- und SIP Password (können aus Sicherheitsgründen nur beim Anlegen eingesehen werden - entweder jetzt notieren oder später neu vergeben)

(6) Unter Alias-Nummern können Sie eine oder mehrere Rufnummern eintragen, unter denen diese Nebenstelle ebenfalls erreicht werden soll. Die Zuordnung der gewählten Rufnummer auf die der Nebenstelle ist hiermit gespeichert.

(7) Hier können Gruppen konfiguriet werden.

[8] Falls Sie Ihre eigenen Töne oder Melodien verwenden wollen, können Sie diese im wav-Format hier hochladen und der Nebenstelle zuweisen.


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




