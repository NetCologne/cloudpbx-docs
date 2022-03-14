---
title: "Seats"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "konfiguration"
weight: 205
toc: true
---

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

Das Web-Passwort wird benötigt, wenn der User der Nebenstelle per Web-Interface seine Nebenstelle konfigurieren können soll – also Anrufweiterschaltungen, Kurzwahlen etc. einrichten können soll.

Das SIP Passwort ist erforderlich, wenn Endgeräte – also Telefone oder Sip Clients etc. – manuell provisioniert werden sollen. Grundsätzlich kann sowohl der Administrator als auch der User die entsprechenden Passwörter ändern und genau dabei auch wieder einsehen. 
Der folgende Screenshot zeigt, wie die Passwörter geändert werden – hier wurden bereit 6 Nebenstellen konfiguriert. 

![cloudpbx_seat hinzufügen3](https://user-images.githubusercontent.com/98753538/157044723-2df6568d-81a5-48e2-bec1-7db413f34a1d.jpg)
