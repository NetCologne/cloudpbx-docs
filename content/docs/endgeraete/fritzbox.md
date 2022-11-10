---
title: "FritzBox"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "endgeraete"
weight: 506
toc: true
---

An der Fritzbox können Sie mehrere Rufnummern und analoge (DECT)-Telefone einrichten. Am Modell der 7490 zeigen wir schrittweise, wie Sie Ihre Fritzbox mit der NetCologne Cloud PBX verbinden und so analoge Telefone bei Ihrer virtuellen Telefonanlage nutzen können. 

## Einrichtung 7490 (stellvertretend für FritzBox)

Schließen Sie zuallererst Ihre FritzBox ans Stromnetz und an Ihren DSL-Anschluß an. <br>
Verbinden Sie dann das Gerät über die Phone-Buchse mit einem analogen Telefon. <br>
Zum Konfigurieren der Rufnummer(n) auf der FritzBox verbinden Sie dann Ihren PC/Notebook mit der FritzBox (z.B. Buchse "LAN1").
Starten Sie einen Browswer Ihrer Wahl und geben als URL "fritz.box" ein. Sie gelangen auf die GUI der FritzBox. <br>
Vergewissern Sie sich bitte zunächst über die aktuelle Firmware-Version der FritzBox. Sie ist in der Übersicht hier zu finden: <br>

![990](https://user-images.githubusercontent.com/99875491/178981706-bc0b0d42-3db4-447f-9331-78639f1ccf97.png)

Die Firmware-Version muss 7.20 oder größer sein, damit die veschlüsselte Übertragung unterstützt wird. Ohne verschlüsselte Übertragung wird der Anschluss **nicht funktionieren.** <br>

### Eigene Rufnummern

Wählen Sie im Menue "Telefonie" den Unterpunkt "Eigene Rufnummern" aus: <br>

![Neue_Rufnummer_00](https://user-images.githubusercontent.com/99875491/201092217-89587ea6-82ed-4635-be3f-c40a24497ee6.jpeg)

Wählen Sie den Punkt "Neue Rufnummer" aus: <br>

![Neue_Rufnummer_01](https://user-images.githubusercontent.com/99875491/201092297-b9667ad6-c995-4a15-b7d1-8fd56674cf60.jpeg)

Tragen Sie im Anschluss unter dem Punkt "Rufnummer für die Anmeldung*" die komplette Nummer und bei "Interne Rufnummer in der FritzBox**" die Nebenstelle ein. <br>

![Neue_Rufnummer_02](https://user-images.githubusercontent.com/99875491/201096556-01796cb0-f850-4885-aca1-dc948f4463f6.jpeg)

Unter Zugangsdaten werden *Benutzername* und *Kennwort* eingetragen, wie sie Ihnen von NetCologne mitgeteilt wurden. Gleiches gilt für die Domäne bei *Registrar* und *Proxy-Server*. <br>

![Neue_Rufnummer_03](https://user-images.githubusercontent.com/99875491/201092427-f4b21471-b3bb-4552-a5b5-a27df4bb702a.jpeg)
<br>

Im Weiteren werden die Standard-Vorgaben aus der GUI verwendet, mit Ausnahme beim Punkt  *Ortsvorwahl für ausgehende Gespräche einfügen* ( bitte deaktivieren ) und *Rufnummer für die Anmeldung verwenden* ( bitte aktivieren ) und * Anmeldung immer über eine Internetverbindung* ( bitte aktivieren ). 
Bei *Transportprotokoll* wählen Sie bitte "TLS" <br>
Grundsätzlich werden Ihre Telefonate bei NetCologne nur verschlüsselt übertragen. Damit dies funktioniert, setzen Sie bitte das Häkchen bei "Der Anbieter unterstützt verschlüsselte Telefonie..." und wählen unter *Media Protocol* "RTP/SAVP" aus : <br>
Im Anschluss erhalten Sie eine Übersicht Ihrer Telefonie-Konfigurationsdaten und wählen "weiter". <br>

![Neue_Rufnummer_04](https://user-images.githubusercontent.com/99875491/201093147-2b0b91fd-a875-452c-a4bc-f02927fe450a.jpeg)

Im Anschluss daran werden Ihre Einrichtung-Daten geprüft und der Anschluss an der NetColgne-Cloud-PBX registriert. Falls die Registrierung fehlschlagen sollte ( "Die Prüfung der Telefonie war nicht erfolgreich ), überprüfen Sie bitte Ihre Eingaben.

![Neue_Rufnummer_05](https://user-images.githubusercontent.com/99875491/201092479-96a95773-a04a-441c-b140-c8df68e1ea66.jpeg)

### Telefoniegeräte

Wählen Sie im FritzBox-Menue den Punkt "Telefoniegeräte". Nun konfigurieren Sie ein oder zwei analoge Telefone, welche Sie bereits an die FritzBox angeschlossen haben: <br>

![Telefoniegeräte](https://user-images.githubusercontent.com/98753538/179159967-b3a54cef-8b88-44ae-9fed-0824e97f7455.jpg)

Hier ist beispielhaft die Einrichtung einer Nebenstelle auf einem der analogen Ports der FritzBox dargestellt: <br>

![1020_1](https://user-images.githubusercontent.com/99875491/178979352-f70e296d-3276-4f4c-99e5-1901b4213e98.png)

Zum Abschluss der Konfiguration sollten Sie noch prüfen, ob sich Ihre Cloud-PBX-Nebenstelle ordnungsgemäß am NetCologne-Netz registriert hat.
Dazu rufen Sie die folgende Übersicht auf: <br>

![Übersicht](https://user-images.githubusercontent.com/98753538/179160026-eb870bf3-d938-4bb2-b0cd-98f7ed04185c.jpg)

Wenn dort unter Telefonie die von Ihnen eingerichteten Rufnummern als "aktiv" dargestellt werden, war die Einrichtung/Registrierung erfolgreich. <br>
Falls nicht, überprüfen Sie bitte die eingegeben Daten und ändern/korrigieren sie ggf.. <br>
