---
title: "Firewall Einstellungen"
date: 2022-09-28T00:11:22+00:00
menu:
  docs:
    parent: "grundlagen"
weight: 103
toc: true
---

Um die Funktion ihrer Cloud-PBX zu gewährleisten müssen folgende Voraussetzungen im lokalen Netz erfüllt sein:

### Zur Provisionierung der Telefone:

Folgende Dienste bzw. Ports müssen freigeschaltet sein:

* HTTPS (TCP Port: 443)<br>
* HTTP (TCP Port: 80)<br>
* TCP-Port 1444<br>
* TCP-Port 1445<br>

### Für die Signalisierung
* Die SIP Signalisierung erfolgt verschlüsselt über  
  **TLS/TCP** (TCP Ports: 5060 und 5061)
* Die Mobile APP verwendet zusätzlich XMPP. Zur Nutzung muss der <br>
  **TCP Port 5222** <br>
  frei gegeben werden
* freizugebende Source/Destination <br>
  ** Wildcard Domain *.cloudpbx.netcologne.de <br>
  ** alternativ Domain firmenname.cloudpbx.netcologne.de (das ist ihre individuelle Anmelde-Domain) <br>
  ** notfalls die Freigabe der IP Adresse 195.14.195.150. Achtung: Es kann u.U. in der Zukunft zur Änderung dieser Adresse kommen <br>


#### Für die Übertragung der Sprachdaten
Die Übertragung der Audio Daten erfolgt verschlüsselt per SRTP.
Dazu müssen die <br>
**UDP Ports zwischen 5062 und 51000** <br>
freigegeben werden<br>
* freizugebende Source/Destination <br>
  ** Wildcard Domain *.cloudpbx.netcologne.de <br>
  ** alternativ Domain firmenname.cloudpbx.netcologne.de (das ist ihre individuelle Anmelde-Domain) <br>
  ** notfalls die Freigabe der IP Adresse 195.14.195.150. Achtung: Es kann u.U. in der Zukunft zur Änderung dieser Adresse kommen <br>
