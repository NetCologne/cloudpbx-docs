---
title: "FritzBox"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "endgeraete"
weight: 506
toc: true
---

Mit der Fritzbox können Sie mehrere Rufnummern einrichten und mit analogen (DECT)-Telefonen telefonieren. Am Modell 7490 zeigen wir schrittweise, wie Sie Ihre Fritzbox mit der NetCologne Cloud PBX verbinden und analoge Telefone mit der virtuellen Telefonanlage einsetzen können. 

## Einrichtung 7490 (stellvertretend für FritzBox)

Schließen Sie zuallererst Ihre FritzBox am Stromnetz und an Ihren DSL-Anschluß an. Verbinden Sie dann das Gerät mit einem analogen Telefon via der Phone-Buchse. Zum Konfigurieren der Rufnummer(n) auf der FritzBox verbinden Sie dann Ihren PC/Notebook mit der FritzBox (z.B. Buchse "LAN1").
Starten Sie einen Browswer Ihrer Wahl und geben als URL "fritz.box" ein. Sie gelangen auf die GUI der FritzBox. 
Vergewissern Sie sich bitte zunächst über die aktuelle Firmware-Version der FritBox. Sie ist in der Übersicht hier zu finden:

![990](https://user-images.githubusercontent.com/99875491/178981706-bc0b0d42-3db4-447f-9331-78639f1ccf97.png)

Die Firmware-Version muss 7.20 oder größer sein, damit die veschlüsselte Übertragung unterstützt wird. Ohne verschlüsselte Übertragung wird der Anschluss nicht funktionieren. 

### Eigene Rufnummer einrichten

Wählen Sie im Menue Telefonie den Unterpunkt Eigene Rufnummern aus:
![1000](https://user-images.githubusercontent.com/99875491/178975443-51f51fa3-9a63-4517-8e7e-aa5d19abc41f.png)
Wählen Sie unter Punkt "Neue Rufnummer" die folgende Option aus:
![1005](https://user-images.githubusercontent.com/99875491/178976078-84ff1609-27be-4159-9e8d-d57f14e43ae7.png)
Tragen Sie im Anschluss Ihre Rufnummern wie folgt ein ( Rufnummer für die Anmeldung: komplette Nummer / Interne Nummer in der FritzBox: die Nebenstelle )
![1010_1](https://user-images.githubusercontent.com/99875491/178977016-6899a8bc-4782-45c8-9a16-00f7c75e9203.png)
Unter Zugangsdaten werden Benutzername / Kennwort eingetragen und die Domänen für Registrar und Proxy, wie sie Ihnen von NetCologne mitgeteilt wurden.
![1010_2](https://user-images.githubusercontent.com/99875491/178977473-990e91bf-118a-4f64-a5a9-940bcac49fbf.png)
Im Weiteren werden die Standard-Vorgaben aus der Gui verwendet, mit Ausnahme von Transportprotokoll. Hier wählen Sie bitte "UDP"
![1010_3_1](https://user-images.githubusercontent.com/99875491/178978075-33376f83-b9bb-4c07-aa89-c0fb8167f1c6.png)
Ein wichtiger Punkt für die generelle Funktion das Anschlusses ist die Eistellung für die Verschlüsselung Ihrer Telefonate. Ihre Telefonate werden bei NetCologne verschlüsselt übertragen. Hierzu aktivieren Sie bitte die Check-Box "Der Anbieter unterstützt verschlüsselte Telefonie..." und wählen unter "Media Protocol" RTP/SAVP aus :
![1010_3_2](https://user-images.githubusercontent.com/99875491/178978575-cfbd4553-8f5d-4c3b-be32-d6513e27d44b.png)
Im Anschluss erhalten Sie eune Übersicht Ihrer Telefonie-Konfigurationsdaten und wählen "weiter"
![1010_4](https://user-images.githubusercontent.com/99875491/178978819-51ed6ada-8f4f-447a-b747-09ddbf0eeff2.png)
Im nächsten Schritt konfigurieren Sie ein oder 2 analoge Telefone, welche Sie bereits aun die FritzBox angeschlossen haben:
![1020](https://user-images.githubusercontent.com/99875491/178979105-845c1129-5f71-43a7-9c3e-bf82a0585a59.png)
Hier ist beispielhaft die Einrichtung einer Nebenstelle auf einem der Analogen Ports der FritzBox dargestellt:
![1020_1](https://user-images.githubusercontent.com/99875491/178979352-f70e296d-3276-4f4c-99e5-1901b4213e98.png)
Zum Abschluss der Konfiguration sollten Sie noch prüfen, ob sich Ihre Cloud-PBX-Nebenstelle ordnungsgemäß am NetCologne-Netz registriert hat.
Dazu rufen Sie die folgende Übersicht auf:
![1030](https://user-images.githubusercontent.com/99875491/178979653-0e92acac-c143-4b31-8c45-9598e7a87fec.png)
Wenn dort unter Telefonie die von Ihnen eingerichteten Rufnummern als "aktiv" dargestellt werden, war die Einrichtung / Registrierung erfolgreich.
Falls nicht, überprüfen Sie bitte die eingegeben Daten und ändern/korrigieren sie ggf.



