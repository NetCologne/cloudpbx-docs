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

![cloudpbx_seat hinzufügen1](https://user-images.githubusercontent.com/98753538/158319658-b4752816-35c2-46f8-ae93-06168a1458f5.jpg)

Zur Einrichtung der Nebenstellen klicken Sie bitte im Punkt "PBX-Konfiguration" auf <br>

* Seats (1) und fügen <br>
* Namen (2, nur Kleinbuchstaben, keine Leer- oder Sonderzeichen), <br>
* Web-Password (3) sowie <br>
* SIP Password (4) hinzu. <br>
Beide können aus Sicherheitsgründen nur beim Anlegen eingesehen werden, d.h. entweder jetzt notieren oder später neu vergeben. <br>
* Ist der Kunde Eigentümer einer weitereren Nummer und hat er diese bei Auftragserteilung der NetCologne mitgeteilt, kann diese unter <br>
  "Alias-Nummer" (5) ausgewählt und zugewiesen werden. Die Nebenstelle ist dann ebenfalls unter der Alias-Nummer erreichbar. <br>
* Gruppen können hier (6) konfiguriet werden. <br>
* Sound-Set (7): Hier können Sie Ihre eigenen Töne oder Melodien im wav-Format hochladen und der Nebenstelle zuweisen. <br>

Im Beispiel wird die Nebenstelle mit der Durchwahl "0" für den User "zollstock" eingerichtet:

![cloudpbx_seat hinzufügen2](https://user-images.githubusercontent.com/98753538/157043465-299f7057-0011-4bb0-a597-5a4dcd5b25e2.jpg)

Das Web-Passwort wird benötigt, wenn der User der Nebenstelle per Web-Interface seine Nebenstelle konfigurieren können soll – also Anrufweiterschaltungen, Kurzwahlen etc. einrichten können soll.

Das SIP Passwort ist erforderlich, wenn Endgeräte – also Telefone oder Sip Clients etc. – manuell provisioniert werden sollen. Grundsätzlich kann sowohl der Administrator als auch der User die entsprechenden Passwörter ändern und genau dabei auch wieder einsehen. 

Der folgende Screenshot zeigt, wie die Passwörter geändert werden – hier wurden bereit 6 Nebenstellen konfiguriert. 

![cloudpbx_seat hinzufügen3](https://user-images.githubusercontent.com/98753538/157044723-2df6568d-81a5-48e2-bec1-7db413f34a1d.jpg)
