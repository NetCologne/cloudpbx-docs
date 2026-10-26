---
title: "Firewall Einstellungen"
date: 2022-09-28T00:11:22+00:00
menu:
  docs:
    parent: "grundlagen"
weight: 103
toc: true
---

### Freizugebene Domain und Ports
Telefone, Softphones und Mobile Apps müssen folgende Ziele auf folgenden Ports erreichen können: <br>

#### Ziel / Quelladresse

* freizugebende Source/Destination Adresse<br>
  * Wildcard Domain:     *.cloudpbx.netcologne.de <br>
  * alternativ Domains:     firmenname.cloudpbx.netcologne.de (dies ist ihre individuelle Anmelde-Domain) und die Domäne phones.cloudpbx.netcologne.de <br>
  * Notfalls:       Freigabe der IP Adresse 195.14.195.150. (Achtung: Es kann u.U. in der Zukunft zur Änderung dieser Adresse kommen) <br>

#### Signalisierung

 Die SIP Signalisierung erfolgt verschlüsselt über  
 
* TLS/TCP (TCP Ports: 5060 und 5061) <br>

 Die Mobile APP verwendet zusätzlich XMPP. Zur Nutzung wird folgender Port benötigt: <br>
 
* TCP Port 5222 <br>

####  Übertragung der Sprachdaten

Die Übertragung der Audio Daten erfolgt verschlüsselt per SRTP. <br>
Hierzu müssen folgende Ports freigegeben werden <br>

* UDP Ports zwischen 5062 und 51000  <br>

#### Zur Provisionierung der Telefone:

Folgende Dienste bzw. Ports müssen für die Telefone erreichbar sein:

* HTTPS (TCP Port: 443)<br>
* HTTP (TCP Port: 80)<br>
* TCP-Port 1444<br>
* TCP-Port 1445<br>
* Folgende NTP-Server müssen für die Telefone auf **port 123** erreichbar sein: <br>
  * Cn.pool.ntp.org <br>
  * pool.ntp.org <br>

### SIP-Helper
Auf einigen Firewalls sind standardmäßig SIP-Helper- bzw. SIP-ALG-Funktionen aktiviert (z. B. Sophos oder FortiGate). <br>
Bitte prüfen Sie die Dokumentation Ihres Firewall-Herstellers und deaktivieren Sie diese Funktionen auf der jeweiligen Appliance. <br>
Für einen störungsfreien Betrieb der Cloud-PBX müssen SIP-Helper/SIP-ALG-Funktionen vollständig deaktiviert sein, da diese die SIP-Kommunikation beeinflussen und zu Fehlfunktionen bei der Telefonie mit unserer Anlage führen können.
