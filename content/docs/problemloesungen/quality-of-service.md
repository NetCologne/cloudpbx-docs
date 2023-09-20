---
title: "Quality-of-Service"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "problemloesungen"
weight: 513
toc: true
---

Abhängig vom Netzwerk ist es erforderlich, Datenpakete für die Telefonie priorisiert durch das Netz zu routen. Die entsprechenden Pakete können mit Hilfe der Differentiated Services klassifiziert werden, sodass sie im Netz bevorzugt behandelt werden. Unter Windows 10 kann zu diesem Zweck eine NetQosPolicy eingerichtet werden. Dafür sind Administratorrechte erforderlich. Im Zweifelsfalls nehmen Sie Kontakt mit Ihrem Netzwerkadministrator auf.

Auf der Netzseite sind die notwendigen Klassifizierung in Richtung Kunde in der Cloud PBX eingerichtet. Auf der Seite des Kunden ist dieser bzw. der Businesspartner für die entsprechenden Regeln zuständig.

Für das Einrichten und Bearbeiten von Policies stellt Microsoft die "Windows PowerShell ISE" zur Verfügung. Diese muss mit Administratorrechten gestartet werden.

In der Regel ist die priorisierte Behandlung der UDP Pakete wichtig, da sie für eine verlustlose Übertragung der Sprache bzw. Nutzdaten erforderlich ist. Mit folgendem Kommando wird eine Policy für UDP zum Server der Cloud PBX eingerichtet:

New-NetQosPolicy -Name voice_udp -DSCPAction 56 -IPDstPrefixMatchCondition 195.14.195.150 -IPProtocolMatchCondition UDP

voice_udp: frei wählbarer Name der Policy<br>
DSCPAction 56: Differentiated Service Codepoint: 56 entspricht dem Class Selector 7 (CS7), der in der Regel für VoIP verwendet wird<br>
IPDstPrefixMatchCondition 195.14.195.150: Ziel-IP-Adresse, für die die entsprechenden Pakete klassifiziert werden sollen<br>
IPProtocolMatchCondition UDP: es sollen nur die UDP Pakete klassifiziert werden<br>

Sollen auch die SIP-Nachrichten klassifiziert werden, so muss zusätzlich eine Regel für die TCP Pakete eingerichtet werden:

New-NetQosPolicy -Name voice_sip -DSCPAction 56 -IPDstPrefixMatchCondition 195.14.195.150 -IPProtocolMatchCondition TCP

Bis auf den letzten Parameter ist das Kommando mit dem für UDP identisch.

Die aktiven Regeln kann man mit folgendem Kommando anzeigen lassen:

Get-NetQosPolicy

Da es ohne weitere Parameter aufgerufen wurde, werden alle aktiven Regeln angezeigt. In diesem Beispiel:

Name : voice_udp<br>
Owner : Group Policy (Machine)<br>
NetworkProfile : All<br>
Precedence : 127<br>
JobObject : <br>
IPProtocol : UDP<br>
IPDstPrefix : 195.14.195.150<br>
DSCPValue : 56<br>
  
Name : voice_sip<br>
Owner : Group Policy (Machine)<br>
NetworkProfile : All<br>
Precedence : 127<br>
JobObject :<br>
IPProtocol : TCP<br>
IPDstPrefix : 195.14.195.150<br>
DSCPValue : 56
