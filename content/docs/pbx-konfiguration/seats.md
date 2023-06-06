---
title: "Seats"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "pbx-konfiguration"
weight: 202
toc: true
---

## Einrichtung von Nebenstellen 

Nebenstellen werden für jegliche Funktion der Anlage benötigt, selbst wenn dahinter kein physikalischer Anschluss steckt. Hinter Nebenstellen können folgende Funktionen konfiguriert werden:

* Physikalische Anschlüsse wie Telefone oder SIP Clients
* Anrufbeantworter
* Faxserver
* ACD/IVR

Die entsprechende Funktion wird über Weiterleitung der Nebenstelle auf die entsprechende Funktion realisiert. Weiterleitungen sind also nicht nur auf physikalische Ziele möglich, sondern auch auf die o. a. Funktionen. 

![neu_seat hinzufügen1](https://user-images.githubusercontent.com/98753538/234775953-f92d5957-e58d-4a0e-8b7f-d82df7fcd25a.jpg)

Zur Einrichtung der Nebenstellen klicken Sie bitte im Punkt "PBX-Konfiguration" auf <br>

* Seats (1) und fügen <br>
* Display Name (2), <br>
* Web Username (3a), <br>
* Web-Password (3b), <br>
* SIP Username (4a) sowie das <br>
* SIP Password (4b) hinzu. <br>

Der Display Name kann unabhängig von Web Username und SIP Username vergeben und z.B. im Falle eines Mitarbeiterwechsels auch aktualisiert werden, ohne dass die Nebenstelle neu eingerichtet werden muss. <br>

Die beiden Passwörter können aus Sicherheitsgründen nur beim Anlegen eingesehen werden, d.h. entweder jetzt notieren oder später neu vergeben. <br>

* Ist der Kunde Eigentümer einer weitereren Nummer und hat er diese bei Auftragserteilung der NetCologne mitgeteilt, kann diese unter "Alias-Nummer" (5) ausgewählt und zugewiesen werden. Die Nebenstelle ist dann ebenfalls unter der Alias-Nummer erreichbar. <br>
* Gruppen können hier (6) konfiguriet werden. <br>
* Sound-Set (7): Hier können Sie Ihre eigenen Töne oder Melodien im wav-Format hochladen und der Nebenstelle zuweisen. <br>

Im Beispiel wird die Nebenstelle mit der Durchwahl "0" für den User "Zollstock" eingerichtet:

![neu_seat hinzufügen3](https://user-images.githubusercontent.com/98753538/234779142-f90019a9-7a45-49b5-a3ef-30b7f9576b56.jpg)

Das Web-Passwort wird benötigt, wenn der User der Nebenstelle per Web-Interface seine Nebenstelle konfigurieren können soll – also Anrufweiterschaltungen, Kurzwahlen etc. einrichten können soll.

Das SIP Passwort ist erforderlich, wenn Endgeräte – also Telefone oder Sip Clients etc. – manuell provisioniert werden sollen. Grundsätzlich kann sowohl der Administrator als auch der User die entsprechenden Passwörter ändern und genau dabei auch wieder einsehen. 
<br>
Der folgende Screenshot zeigt, wie die Passwörter geändert werden – hier wurden bereit 6 Nebenstellen konfiguriert. 

![cloudpbx_seat hinzufügen3](https://user-images.githubusercontent.com/98753538/157044723-2df6568d-81a5-48e2-bec1-7db413f34a1d.jpg)


## Konfiguration der angezeigten Nummer

Klickt man die Nebenstelle an, können links unter Preferences (1) weitere Einstellungen vorgenommen werden. <br>

![neu_seat Anzeige2](https://user-images.githubusercontent.com/98753538/234835421-d3c311b6-04ca-4d27-992e-0c0e50da39bf.jpg)

Bei Preferencen/Einstellungen kann unter CLI (Calling Line Identification) die abgehend signalisierte Rufnummer konfiguriert werden. Dies kann z.B. die Nummer der Vermittlung/Zentrale oder Hotline sein. <br>
 <br>
Beim darüberliegenden Punkt kann eine oder mehrere Alias-Nummer ausgewählt werden, unter der diese Nebenstelle erreichbar sein soll. Dies könnte beispielweise bei einer Neuschaltung die bisherige (alte) Rufnummer sein, insofern sie "mitgenommen" wurde. Prinzipiell könnnen alle Rufnummern des Kunden der Nebenstelle als Alias zugewiesen werden. <br>
<br>

Rechts unter Call Forwards (2) kann man ein Anrufweiterleitung konfigurieren, siehe hierzu https://cloudpbx-doku.netcologne.de/docs/funktionen/anrufweiterleitung/
