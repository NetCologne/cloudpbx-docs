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

Zur Einrichtung einer  Nebenstellen klicken Sie bitte im Punkt "PBX-Konfiguration" auf *Nebenstellen* und anschließend auf *+ NEBENSTELLE HINZUFÜGEN* <br>

![NST hinzufügen1](https://github.com/user-attachments/assets/40772df4-7fc0-42cc-b067-94ebbfa06b7a)

Im nachfolgenden Menue werden anschließend

* Anzeigename (1), <br>
* Durchwahl (2), <br>
* Force CLI (3), <br>
* Alias-Nummern (4), <br>
* Web-Benutzernamen (5a), <br>
* Web-Passwort (5b), <br>
* SIP-Benutzername (6a) und <br>
* SIP-Password (6b) bearbeitet. <br>
* Gruppen können unter (7) konfiguriert werden. <br>
* Bei Sound-Set (8) können Sie neben dem Standard auch eigenen Töne oder Melodien im wav-Format hochladen und der Nebenstelle zuweisen. <br>

![NST hinzufügen11](https://github.com/user-attachments/assets/b69e3036-5409-442f-887d-d6a0d40f42ea)

Der auf dem Display erscheinende *Anzeigename* (1) kann unabhängig von *Web-Benutzername* (5a) und *SIP-Benutzername* (6a) vergeben werden. Er kann damit, z.B. im Falle eines Mitarbeiterwechsels, einfach aktualisiert werden, ohne dass die Nebenstelle neu eingerichtet werden muss. <br>

Setzen Sie bei *Force CLI* (3) das Häkchen, um sicher zu stellen, dass immer die in der Cloud-PBX eingetragene Rufnummer übertragen wird. Sie generiert sich zunächst aus der PBX-Stamm- oder Anschlussnummer + Durchwahl, kann aber später geändert werden. <br>

Ist der Kunde Eigentümer einer weitereren Nummer und hat er diese bei Auftragserteilung der NetCologne mitgeteilt, kann diese unter *Alias-Nummern* (4) ausgewählt und zugewiesen werden. Die Nebenstelle ist dann ebenfalls unter der Alias-Nummer erreichbar. <br>

Das *Web-Passwort* (5b) wird benötigt, wenn der User eine Nebenstelle per Web-Interface konfigurieren - also Einrichten von Anrufweiterschaltungen, Kurzwahlen etc. - können soll. <br>

Das *SIP-Passwort* (6b) ist erforderlich, wenn Endgeräte – also Telefone oder Sip Clients etc. – manuell provisioniert werden sollen. <br>

Grundsätzlich kann sowohl der Administrator als auch der User die entsprechenden Passwörter ändern und genau dabei auch wieder einsehen. <br>

Die beiden Passwörter können aus Sicherheitsgründen nur beim Anlegen eingesehen werden, d.h. entweder jetzt notieren oder später neu vergeben. <br>

![NST hinzufügen2](https://github.com/user-attachments/assets/5678029a-4a2d-4b17-8fd7-8e50c1499700)

Abschließend wird die Nebenstelle *Zollstock* mit der Durchwahl "0" für den User "Zollstock" durch Klicken auf *NEBENSTELLE HINZUFÜGEN* dann eingerichtet. <br>

Der folgende Screenshot zeigt, wie die Passwörter geändert werden: <br>

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
