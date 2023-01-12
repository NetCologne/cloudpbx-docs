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

* HTTPS<br>
* HTTP<br>
* TCP-Port 1444<br>
* TCP-Port 1445<br>

### Für die Signalisierung
* Die SIP Signalisierung erfolgt verschlüsselt über  
  **TLS/TCP**
* Die Mobile APP verwendet zusätzlich XMPP. Zur Nutzung muss der <br>
  **TCP Port 5222** <br>
  frei gegeben werden

#### Für die Übertragung der Sprachdaten
Die Übertragung der Audio Daten erfolgt verschlüsselt per SRTP.
Dazu müssen die <br>
**UDP Ports zwischen 5062 und 50000** <br>
freigegeben werden<br>
