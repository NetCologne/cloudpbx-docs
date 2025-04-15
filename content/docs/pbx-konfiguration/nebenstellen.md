---
title: "Nebenstellen"
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

![NST hinzufügen](https://github.com/user-attachments/assets/0ad996c1-7b00-4500-827e-698c90a71aef)


Zur Einrichtung der Nebenstellen klicken Sie bitte im Punkt "PBX-Konfiguration" auf <br>

* Nebenstellen (1) und fügen mit dem "+-Zeichen" und Angabe von <br>
* Anzeigenamen (2), <br>
* Web-Benutzernamen (3a), <br>
* Web-Passwort (3b), <br>
* SIP-Benutzername (4a) und <br>
* SIP-Password (4b) eine weitere Nebenstelle hinzu. <br>

Der auf dem Display erscheinende *Anzeigename* kann unabhängig von *Web-Benutzername* und *SIP-Benutzername* vergeben werden. Er kann damit, z.B. im Falle eines Mitarbeiterwechsels, einfach aktualisiert werden, ohne dass die Nebenstelle neu eingerichtet werden muss. <br>

Die beiden Passwörter können aus Sicherheitsgründen nur beim Anlegen eingesehen werden, d.h. entweder jetzt notieren oder später neu vergeben. <br>

* Setzen Sie bei Force CLI das Häkchen (s. Bild unten, roter Pfeil), um sicher zu stellen, dass immer die in der Cloud-PBX eingetragene Rufnummer übertragen wird.
* Ist der Kunde Eigentümer einer weitereren Nummer und hat er diese bei Auftragserteilung der NetCologne mitgeteilt, kann diese unter "Alias-Nummer" (6) ausgewählt und zugewiesen werden. Die Nebenstelle ist dann ebenfalls unter der Alias-Nummer erreichbar. <br>
* Gruppen können hier (7) konfiguriert werden. <br>
* Sound-Set (8): Hier können Sie Ihre eigenen Töne oder Melodien im wav-Format hochladen und der Nebenstelle zuweisen. <br>

![NST hinzufügen4](https://github.com/user-attachments/assets/50b57300-e02c-4f3d-a323-8725c7973d7b)

Im Beispiel wird die Nebenstelle mit der Durchwahl "0" für den User "Zollstock" eingerichtet:

![NST hinzufügen2](https://github.com/user-attachments/assets/6403d33a-fcca-4e49-9013-81c8b37c5d52)

Das Web-Passwort wird benötigt, wenn der User peine Nebenstelle per Web-Interface konfigurieren - also Einrichten von Anrufweiterschaltungen, Kurzwahlen etc. - können soll.

Das SIP-Passwort ist erforderlich, wenn Endgeräte – also Telefone oder Sip Clients etc. – manuell provisioniert werden sollen. Grundsätzlich kann sowohl der Administrator als auch der User die entsprechenden Passwörter ändern und genau dabei auch wieder einsehen. 
<br>
Der folgende Screenshot zeigt, wie die Passwörter geändert werden: 

![NST hinzufügen3](https://github.com/user-attachments/assets/d400294f-4ee4-4ada-8573-cf2d7004ab27)



### Konfiguration der angezeigten Nummer

Klickt man die Nebenstelle an, können links unter Preferences (1) weitere Einstellungen vorgenommen werden. <br>

![neu_seat Anzeige2](https://user-images.githubusercontent.com/98753538/234835421-d3c311b6-04ca-4d27-992e-0c0e50da39bf.jpg)

Bei Preferencen/Einstellungen kann unter CLI (Calling Line Identification) die abgehend signalisierte Rufnummer konfiguriert werden. Dies kann z.B. die Nummer der Vermittlung/Zentrale oder Hotline sein. <br>
**Achtung:** Diese Funktion kann nur gewährleistet werden, wenn der SIP User nicht die Durchwahl ist! Im Beispiel ist dies gegeben ("Zollstock_SIP" ≠ "0"). <br>
 <br>
Beim darüberliegenden Punkt kann eine oder mehrere Alias-Nummer ausgewählt werden, unter der diese Nebenstelle erreichbar sein soll. Dies könnte beispielweise bei einer Neuschaltung die bisherige (alte) Rufnummer sein, insofern sie "mitgenommen" wurde. Prinzipiell könnnen alle Rufnummern des Kunden der Nebenstelle als Alias zugewiesen werden. <br>
<br>
Rechts unter Call Forwards (2) kann man eine [Anrufweiterleitung](https://cloudpbx-doku.netcologne.de/docs/funktionen/anrufweiterleitung/) konfigurieren.
