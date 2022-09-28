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

## Provisionierung der Telefone:

Folgende Dienste bzw. Ports müssen freigeschaltet sein:

HTTPS<br>
HTTP<br>
TCP-Port 1444<br>
TCP-Port 1445<br>

## Signalisierung
Die SIP Signalisierung erfolgt verschlüsselt über TLs auf UDP-Port 5061
Die Mobile APP verwendet zusätzlich XMPP. Zu Nutzung mus der TCP Port 5222 frei gegeben werden

### Audio
Die Übertragung der Audio Daten erfolgt verschlüsselt per SRTP.
Dazu müssen die UDP Ports zwischen 10000 und 50000 freigegeben werden
