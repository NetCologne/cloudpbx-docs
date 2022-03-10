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

[1] Das Dashboard liefert eine Überischt zu Nachrichten (Messages), Anrufen (Calls) und den registrierten Endgeräten.

[2] Beim Punkt Konversationen stehen weitere Details wie "von" und "an".

## Einrichtung von Nebenstellen 

Nebenstellen werden für jegliche Funktion der Anlage benötigt, selbst wenn dahinter kein physikalischer Anschluss steckt. Hinter Nebenstellen können folgende Funktionen konfiguriert werden:

* Physikalische Anschlüsse wie Telefone oder SIP Clients
* Anrufbeantworter
* Faxserver
* ACD/IVR

Die entsprechende Funktion wird über Weiterleitung der Nebenstelle auf die entsprechende Funktion realisiert. Weiterleitungen sind also nicht nur auf physikalische Ziele möglich, sondern auch auf die o. a. Funktionen. 

Zur Einrichtung der Nebenstellen klicken Sie bitte im Punkt "PBX-Konfiguration" auf

[3] "Seats" und fügen  

![cloudpbx_dashboard2-8](https://user-images.githubusercontent.com/98753538/152347008-0ad4c1fe-a492-4fd1-860c-2b355e903b0a.jpg)
   
[4] Namen (nur Kleinbuchstaben, keine Leer- oder Sonderzeichen) und

[5] Web- sowie SIP Password (können aus Sicherheitsgründen nur beim Anlegen eingesehen werden - entweder jetzt notieren oder später neu vergeben) hinzu.

[6] Ist der Kunde Eigentümer einer weitereren "Alias-Nummer" und hat er diese bei Auftragserteilung der NetCologne mitgeteilt, kann diese hier ausgewählt und zugewiesen werden. Die Nebenstelle ist dann ebenfalls unter der Alias-Nummer erreichbar. 

[7] Hier können Gruppen konfiguriet werden.

[8] Falls Sie Ihre eigenen Töne oder Melodien verwenden wollen, können Sie diese im wav-Format hier hochladen und der Nebenstelle zuweisen.

Beispiel: Hier wird nun die Nebenstelle 0 für den User "zollstock" eingerichtet:

![cloudpbx_seat hinzufügen](https://user-images.githubusercontent.com/98753538/157040888-c73e65a9-1cdc-4030-97d1-55d2e2eb54a3.jpg)

![cloudpbx_seat hinzufügen2](https://user-images.githubusercontent.com/98753538/157043465-299f7057-0011-4bb0-a597-5a4dcd5b25e2.jpg)

Das Web Passwort wird benötigt, wenn der User der Nebenstelle per Web Interface seine Nebenstelle konfigurieren können soll – also Anrufweiterschaltungen, Kurzwahlen etc. einrichten können soll.

Das SIP Passwort ist erforderlich, wenn Endgeräte – also Telefone oder Sip Clients etc. – manuell provisioniert werden sollen. Grundsätzlich kann sowohl der Administrator als auch der User die entsprechenden Passwörter ändern und genau dabei auch wieder einsehen. 
Der folgende Screenshot zeigt, wie die Passwörter geändert werden – hier wurden bereit 6 Nebenstellen konfiguriert. 

![cloudpbx_seat hinzufügen3](https://user-images.githubusercontent.com/98753538/157044723-2df6568d-81a5-48e2-bec1-7db413f34a1d.jpg)


## Einrichten von Geräten

Nachdem Sie die Nebenstellen eingerichtet haben, machen Sie die verwendeten Telefone in der CloudPBX bekannt. Die Einrichtung erfolgt ebenfalls unter dem Punkt PBX-Konfiguration. <br> 
Klicken Sie dafür einfach auf "+ GERÄT HINZUFÜGEN". <br>
Geben Sie Stations-Name und MAC-Adresse ein und wählen Sie das Telefonmodell aus. <br>
Abschließend bestätigen Sie mit "✓ GERÄT HINZUFÜGEN". <br>

### Snom D7-Serie
![cloudpbx_Gerät1 hinzufügen](https://user-images.githubusercontent.com/98753538/157050069-16510561-363d-4d15-842b-838dbd7b46aa.jpg)

Im nächsten Schritt konfigurieren Sie die Telefone. Sie legen also fest, welche Nebenstelle auf welchem Telefon klingeln soll und welche Nebenstellen per BusyLampField (BLF) überwacht werden sollen. Klicken Sie dafür auf das Gerät richten bei der entsprechenden Lampe/Taste den Teilnehmer ein:
![cloudpbx_Teilnehmer einrichten1](https://user-images.githubusercontent.com/98753538/157249202-096b60c3-3ec4-49b8-a22c-d85b0278d1b9.jpg)

### Yealink T5-Serie
![cloudpbx_Gerät2 hinzufügen](https://user-images.githubusercontent.com/98753538/157050085-69f52435-ca04-40c6-ae12-0e43dc7bd4b3.jpg)

Die Lampen/Tasten können auch mit anderen Teilnehmern und der Funktion "Besetzlampenfeld" belegt werden: 

![cloudpbx_Teilnehmer einrichten4](https://user-images.githubusercontent.com/98753538/157250752-3cb7113d-c166-4b48-b172-fbfe210cdc87.jpg)

So sieht z.B. die "Zentrale", welcher Kollege gerade angerufen wird oder kann einen ankommenden Anruf übernehmen:

![cloudpbx_busylampfield1](https://user-images.githubusercontent.com/98753538/157256356-a871d273-04d9-4c8c-844e-6dc818de1f0c.jpg)

### Snom M900 DECT-Basisstation
Diese Basisstation wandelt das IP-Protokoll der Cloud PBX in das DECT-Protokoll umd und bildet damit di Brücke zwischen Internet-Anschluss Ihren DECT-Telefonen. Die M900 bietet neben einem integrierten DECT-Manager auch eine DECT- und LAN-Synchronisierung. Der SIP-Transport kann neben UDP auch mittels TCP oder TLS erfolgen. Mit "Seamless Handover" ist der nahtlose Wechsel von einer Basisstation zur nächsten möglich.

![cloudpbx_Gerät3 hinzufügen](https://user-images.githubusercontent.com/98753538/157050358-01266501-cc69-4e7a-b46f-cf0dddebf921.jpg)

Kompatible Mobilteile sind M25, M65, M70, M80, M85, M90. Jedes DECT-Telefon muss einer Basisstation zugewiesen sein.

![cloudpbx_Teilnehmer einrichten2](https://user-images.githubusercontent.com/98753538/157249871-a15e2c1a-8ee4-4af3-995e-a4dde92cd579.jpg)

Bei der SNOM-Basisstation können bis zu 19 Teilnehmer eingerichtet werden. Im Beispiel sind es zwei:

![cloudpbx_Teilnehmer einrichten5](https://user-images.githubusercontent.com/98753538/157256005-95ef62fb-dcec-42a6-915e-8888618f1e67.jpg)

#### Anmeldung der Snom-Mobilteile (Handsets)

Im Fritzbox-Meü -> Heimnetz -> Netzwerk kann man unter "Netzwerkverbindungen" die IP-Adresse der DECT-Basisstation einsehen bzw. diese auswählen:

![Cloudpbx_einrichten_snom_dect_fritzbox](https://user-images.githubusercontent.com/98753538/157690228-f65b389b-9384-42ec-acd8-79b36f1ba638.jpg)

So gelangt man zum WEB-Portal der Snom M900. Im Menüpunkt "Extensions" kann man die verbundenen Mobilteile einsehen und weitere hinzufügen. Dafür das entsprechenden Gerät mit Häkchen auswählen und auf "Register Handset(s)" klicken. Daraufhin wird Ihnen im oberen Bereich der Access-Code (AC), hier "7666" angezeigt.

![Cloudpbx_einrichten_snom_dect_endgeräte3](https://user-images.githubusercontent.com/98753538/157692195-9bae9037-8950-4312-8380-033f61c84253.jpg)

Parallel dazu wählen Sie im Handset/Mobilteil den Punkt "Connectivity" aus, bestätigen "Register", tragen hier den Access-Code ein und bestätigen mit "OK".

![Handheld hinzufügen](https://user-images.githubusercontent.com/98753538/157691802-be0a428d-e6e9-49a4-b753-b00f016dbb6b.jpg)

Abschließend aktualisieren Sie im WEB-Portal die Ansicht "Extension" und Sie sehen alle registrierten Mobilteile:

![Cloudpbx_einrichten_snom_dect_endgeräte4](https://user-images.githubusercontent.com/98753538/157692597-70050298-c579-4109-b648-41ad36701c50.jpg)

Sind die angemeldeten Handsets noch nicht sichtbar ist gegebenenfalls im Menüüunkt "Home/Status" ein Reboot der DECT-Basisstation sinnvoll.

![Cloudpbx_einrichten_snom_dect_reboot](https://user-images.githubusercontent.com/98753538/157691428-c41043ce-f043-4586-ac25-4365ba70e299.jpg)



