---
title: "Nebenstellen"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "pbx-konfiguration"
weight: 202
toc: true
---

Nebenstellen werden für jegliche Funktion der Anlage benötigt, selbst wenn dahinter kein physikalischer Anschluss steckt. Hinter Nebenstellen können folgende Funktionen konfiguriert werden:

* Physikalische Anschlüsse wie Telefone oder SIP Clients
* Anrufbeantworter
* Faxserver
* ACD (**A**utomatic **C**all **D**istribution = Automatische Anrufverteilung) vergleichbar mit
* IVR (**I**nteractive **V**oice **R**esponse = Interaktiver Anrufbeantworter). <br>
Beide Male erhalten Anrufer die Möglichkeit, ihre Präferenzen auszuwählen, bevor sie mit einem Callcenter-Agenten verbunden werden.

Die entsprechende Funktion wird über Weiterleitung der Nebenstelle auf die entsprechende Funktion realisiert. Weiterleitungen sind also nicht nur auf physikalische Ziele möglich, sondern auch auf die o. a. Funktionen. 

## Einrichtung von Nebenstellen 

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

⚠️ **Wichtig:** Die beiden Passwörter können aus Sicherheitsgründen nur beim Anlegen eingesehen werden, d.h. entweder jetzt notieren oder später neu vergeben. <br>

![NST hinzufügen2](https://github.com/user-attachments/assets/5678029a-4a2d-4b17-8fd7-8e50c1499700)

Abschließend wird die Nebenstelle *Zollstock* mit der Durchwahl "0" für den User "Zollstock" durch Klicken auf *NEBENSTELLE HINZUFÜGEN* dann eingerichtet. <br>

Der folgende Screenshot zeigt, wie die Passwörter geändert werden: <br>

![NST hinzufügen3](https://github.com/user-attachments/assets/d400294f-4ee4-4ada-8573-cf2d7004ab27)

Klickt man die Nebenstelle an, kann man zwischen den Reitern

* EINSTELLUNGEN, 
* RUFUMLEITUNGEN, 
* ANRUFBEANTWORTER, 
* "FAX TO MAIL" UND "SENDFAX" und 
* MAIL TO FAX auswählen. <br>  

### 1. EINSTELLUNGEN

![NST Einstellungen](https://github.com/user-attachments/assets/2fed0b1f-87d2-4ab9-9f9f-bf1cd7749d79)

Beim Punkt *Alias-Nummer* (1) kann die Nummer ausgewählt werden, unter der diese Nebenstelle erreichbar sein soll. Dies könnte beispielweise bei einer Neuschaltung die bisherige (alte) Rufnummer sein, insofern sie "mitgenommen" wurde. Prinzipiell könnnen alle Rufnummern des Kunden der Nebenstelle als Alias zugewiesen werden. <br>

Beim darunter liegenden Punkt *CLI* (2) kann die "Calling Line Identification" also die abgehend signalisierte Rufnummer konfiguriert werden. Dies kann z.B. die Nummer der Vermittlung/Zentrale oder Hotline sein. <br>

⚠️ **Wichtig:** Diese Funktion kann nur gewährleistet werden, wenn der SIP User nicht die Durchwahl ist! Im Beispiel ist dies gegeben (SIP USER: "Zollstock_SIP" ≠ Durchwahl "0"). <br>

Ansage vor Melden (3) <br>

Ansage nach Melden (4) <br>

Anrufweiterleitung bei Anrufen von Mitgliedern einer Gruppe ignorieren (5) <br>
<br>

### 2. RUFUMLEITUNGEN

![NST Rufumleitungen](https://github.com/user-attachments/assets/3ecc72ba-0629-4be3-ae54-529eb83a4d1d)

Wie sie diese Funktionen konfigurieren, ist ausführlich unter [RUFUMLEITUNGEN](https://cloudpbx-doku.netcologne.de/docs/funktionen/anrufweiterleitung/) beschrieben. <br>

### 3. ANRUFBEANTWORTER

![NST ABW](https://github.com/user-attachments/assets/0b36dc4d-1b88-4a3d-9108-c698641e08cc)

Die Beschreibung dieser Funktion finden sien unter [ANRUFBEANTWORTER](https://cloudpbx-doku.netcologne.de/docs/funktionen/anrufbeantworter/) <br>

### 4. "FAX TO MAIL" UND "SENDFAX"

<br>

### 5. MAIL TO FAX

<br>
