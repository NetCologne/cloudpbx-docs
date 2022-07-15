---
title: "FritzBox"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "endgeraete"
weight: 506
toc: true
---

An der Fritzbox können Sie mehrere Rufnummern und analoge (DECT)-Telefone einrichten. Am Modell der 7490 zeigen wir schrittweise, wie Sie Ihre Fritzbox mit der NetCologne Cloud PBX verbinden und so analoge Telefone bei der virtuellen Telefonanlage nutzen können. 

## Einrichtung 7490 (stellvertretend für FritzBox)

Schließen Sie zuallererst Ihre FritzBox ans Stromnetz und an Ihren DSL-Anschluß an. <br>
Verbinden Sie dann das Gerät über die Phone-Buchse mit einem analogen Telefon. <br>
Zum Konfigurieren der Rufnummer(n) auf der FritzBox verbinden Sie dann Ihren PC/Notebook mit der FritzBox (z.B. Buchse "LAN1").
Starten Sie einen Browswer Ihrer Wahl und geben als URL "fritz.box" ein. Sie gelangen auf die GUI der FritzBox. <br>
Vergewissern Sie sich bitte zunächst über die aktuelle Firmware-Version der FritBox. Sie ist in der Übersicht hier zu finden: <br>

![990](https://user-images.githubusercontent.com/99875491/178981706-bc0b0d42-3db4-447f-9331-78639f1ccf97.png)

Die Firmware-Version muss 7.20 oder größer sein, damit die veschlüsselte Übertragung unterstützt wird. Ohne verschlüsselte Übertragung wird der Anschluss **nicht funktionieren.** <br>

### Eigene Rufnummern

Wählen Sie im Menue "Telefonie" den Unterpunkt "Eigene Rufnummern" aus: <br>

![1000](https://user-images.githubusercontent.com/99875491/178975443-51f51fa3-9a63-4517-8e7e-aa5d19abc41f.png)

Wählen Sie unter Punkt "Neue Rufnummer" die folgende Option aus: <br>

![Eigene Rufnummer](https://user-images.githubusercontent.com/98753538/179160233-07979018-da04-4197-8291-40006fe6101d.jpg)

Tragen Sie im Anschluss unter dem Punkt "Rufnummer für die Anmeldung*" die komplette Nummer und bei "Interne Rufnummer in der FritzBox**" die Nebenstelle ein. <br>

![1010_1](https://user-images.githubusercontent.com/99875491/178977016-6899a8bc-4782-45c8-9a16-00f7c75e9203.png)

Unter Zugangsdaten werden *Benutzername* und *Kennwort* eingetragen, wie sie Ihnen von NetCologne mitgeteilt wurden. Gleiches gilt für die Domäne bei *Registrar* und *Proxy-Server*. <br>

![Zugangsdaten](https://user-images.githubusercontent.com/98753538/179159885-5013b8ab-69a6-4352-a670-d2d94972e3d5.jpg)

Im Weiteren werden die Standard-Vorgaben aus der GUI verwendet, mit Ausnahme beim Punkt *Transportprotokoll*. Hier wählen Sie bitte "UDP" <br>

![1010_3_1](https://user-images.githubusercontent.com/99875491/178978075-33376f83-b9bb-4c07-aa89-c0fb8167f1c6.png)

<br>
Grundsätzlich werden Ihre Telefonate bei NetCologne nur verschlüsselt übertragen. Damit dies funktioniert, setzen Sie bitte das Häkchen bei "Der Anbieter unterstützt verschlüsselte Telefonie..." und wählen unter *Media Protocol* "RTP/SAVP" aus : <br>

![1010_3_2](https://user-images.githubusercontent.com/99875491/178978575-cfbd4553-8f5d-4c3b-be32-d6513e27d44b.png)
Im Anschluss erhalten Sie eine Übersicht Ihrer Telefonie-Konfigurationsdaten und wählen "weiter". <br>

![Internetrufnummern](https://user-images.githubusercontent.com/98753538/179161233-736582f4-9a29-41f1-8432-34aff97e4602.jpg)

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
