---
title: "Geräte"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "pbx-konfiguration"
weight: 204
toc: true
---

## Einrichten von Geräten

Nachdem Sie die Nebenstellen eingerichtet haben, machen Sie die verwendeten Telefone in der CloudPBX bekannt. Die Einrichtung erfolgt ebenfalls unter dem Punkt PBX-Konfiguration. <br> 
Klicken Sie dafür einfach auf "+ GERÄT HINZUFÜGEN". <br>
Geben Sie Stations-Name und MAC-Adresse ein und wählen Sie das Telefonmodell aus. <br>
Abschließend bestätigen Sie mit "✓ GERÄT HINZUFÜGEN". <br>

### Snom D7-Serie
![cloudpbx_Gerät1 hinzufügen](https://user-images.githubusercontent.com/98753538/157050069-16510561-363d-4d15-842b-838dbd7b46aa.jpg)

Im nächsten Schritt konfigurieren Sie die Telefone. Sie legen also fest, welche Nebenstelle auf welchem Telefon klingeln soll und welche Nebenstellen per BusyLampField (BLF) überwacht werden sollen. Klicken Sie dafür auf das Gerät und richten bei der entsprechenden Lampe/Taste den Teilnehmer ein:
![cloudpbx_Teilnehmer einrichten1](https://user-images.githubusercontent.com/98753538/157249202-096b60c3-3ec4-49b8-a22c-d85b0278d1b9.jpg)

Weitere Funktionen für die Tastenbelegung sind Kurzwahl, Forward oder Transfer.

![Neue Tasten2](https://user-images.githubusercontent.com/98753538/234840253-484f59f6-3a4e-4e79-9f4a-df0a22b3ec41.jpg)


### Yealink T5-Serie
![cloudpbx_Gerät2 hinzufügen](https://user-images.githubusercontent.com/98753538/157050085-69f52435-ca04-40c6-ae12-0e43dc7bd4b3.jpg)

Die Lampen/Tasten können auch mit anderen Teilnehmern und der Funktion "Besetzlampenfeld" (BLF) belegt werden: 

![cloudpbx_Teilnehmer einrichten4](https://user-images.githubusercontent.com/98753538/157250752-3cb7113d-c166-4b48-b172-fbfe210cdc87.jpg)

So sieht z.B. die "Zentrale", welcher Kollege gerade angerufen wird oder kann einen ankommenden Anruf übernehmen:

![cloudpbx_busylampfield1](https://user-images.githubusercontent.com/98753538/157256356-a871d273-04d9-4c8c-844e-6dc818de1f0c.jpg)

Weitere Funktionen für die Tastenbelegung sind *Kurzwahl, Forward oder Transfer*.

![Neue_Tasten](https://user-images.githubusercontent.com/98753538/234839231-0bb97cbc-eb29-4d51-be63-e7ee1c95fc9f.jpg)


### Yealink W60B
Diese Basisstation wandelt das IP-Protokoll der Cloud PBX in das DECT-Protokoll umd und bildet damit die Brücke zwischen Internet-Anschluss Ihren DECT-Telefonen.

![cloudpbx yealinkW60B](https://user-images.githubusercontent.com/98753538/159929245-d66ec338-1a73-42dc-9967-5330f1423112.jpg)

Durch Klicken auf die entsprechende Nummer (grüner Pfeil), weisen Sie dem Gerät die entsprechende Nebenstelle zu:

![cloudpbx yealinkW60B_NSt](https://user-images.githubusercontent.com/98753538/159929867-bbe9c09b-d4bb-4556-bf4f-3de8ee100c74.jpg)

Dem zugehörigen Handset, z.B. Yealink 56H, wird dann die Nebenstelle automatisch zugewiesen.<br>
<br>
<br>
<br>

### Yealink W70B
Diese Basisstation wandelt das IP-Protokoll der Cloud PBX in das DECT-Protokoll umd und bildet damit die Brücke zwischen Internet-Anschluss Ihren DECT-Telefonen.

Durch Klicken auf die entsprechende Nummer , weisen Sie dem Gerät die entsprechende Nebenstelle zu:

![W70B](https://user-images.githubusercontent.com/99875491/195816281-00e94e06-4e14-4267-93a8-391e5f6d132f.png)

Nach erfolgreicher Nummernzuweisung muss auf der W70B noch ein Factory-Reset durchgeführt werden, damit die zugewiesenen Nummern automatisch übernommen werden. Die Zuweisung und Registrierung der DECT-Mobilteile efolgt dann ebenfalls über die GUI der Basis-Station:

### Mobilteil anmelden W56H 

Um ein Mobilteil an der Yealink DECT IP Basisstation W70B anzumelden, gehen Sie bitte wie folgt vor:

![NC_Doku_Mobilteil_Anmelden_1](https://user-images.githubusercontent.com/99875491/169036830-5e5ea5de-a2a6-4c47-a654-16cc1c3d8ffb.jpg)

1. Begeben Sie sich zu dem Menüpunkt "Status".
2. Wählen Sie nun den Punkt "Handset & Voip" aus.
3. Mit Klick auf "Mobilteil registrieren starten" wird das Mobilteil an der DECT IP Basisstation angemeldet.
4. Sie werden nun von der WEB-Site aufgerufen, das Mobilteil zu registrieren.
" Bitte registrieren Sie Ihr Mobilteil..."
5. Dazu wählen Sie den Entsprechenden Punkt aus dem Menü Ihres Mobilteils aus.

Im Falle eines W56H zB:

1. OK-Taste
2. Menue-Punkt "Einstellungen"
3. Punkt "6.Registrieren"
4. "Mobilteil registrieren"
5. Basisstation ersetzen
6. Nun werden Sie von Ihrem Mobilteil aufgefordert, die PIN einzugeben. Im Auslieferungszustand lautet die PIN "0000"
7. Nun ist das Mobilteil an der DECT IP Basisstation angemeldet 

### Hinweis für Konfigurations-Änderungen nach Erst-Konfiguration :

Falls im Laufe des Betriebs Änderungen an der Konfiguration der Nebenstellen ( DECT-Mobilteile ) vorgenommen werden sollen ( zB. Löschen und Hinzufügen von Nebenstellen  ( DECT-Mobilteile ) so gehen Sie bitte wie folgt vor:

Um ungewollte Vertauschungen von SIP Usern und Dect Endgeräten zu vermeiden, muss folgendermaßen vorgegangen werden:

1.Schritt: Lückenlose Provisionierung der Nebenstellen im WebInterface der CloudPBX:

![grafik](https://user-images.githubusercontent.com/99875491/196387496-83f9ceaa-3d2c-494d-bb91-a88e9248f777.png)

Das heißt die Ports müssen der Reihe nach belegt werden (hier also 1 – 3)

2.Schritt: Factory Reset des W70B – damit ist sicher gestellt, dass es zu keinen Vertauschungen kommt und in der GUI des W70B sieht das so aus:

![W70_Doku](https://user-images.githubusercontent.com/99875491/196388088-f344b0a3-4892-4f76-b1c3-a02c071a332c.png)

![grafik](https://user-images.githubusercontent.com/99875491/196387806-39d9b8ba-9e75-423d-b8a9-dfed6d76e315.png)

3.Schritt: Registrierung der DECT Telefone über die GUI des W70B

Sollen Nebenstellen ergänzt werden, sollte ein Factory Reset nicht notwendig sein, solange die lückenlose Provisionierung gewährleistet ist.

Wenn in der Web Ansicht des W70B die Diagonale (wie oben zu sehen) unter Eingehende bzw. Ausgehende Leitungen nicht mehr durchgängig ist, ist mindestens ein Factory Reset erforderlich. Die Provisionierung ist vorher auf etwaige Lücken zu prüfen.

### Yealink W80DM (W80DM-10)
Diese Basisstation wandelt das IP-Protokoll der Cloud PBX in das DECT-Protokoll umd und bildet damit die Brücke zwischen Internet-Anschluss Ihren DECT-Telefonen.

Durch Klicken auf die entsprechende Nummer , weisen Sie dem Gerät die entsprechende Nebenstelle zu:

![W80DM-10](https://user-images.githubusercontent.com/99875491/195816308-371b8e1b-b56f-436e-b906-fa8d417f5410.png)

Nach erfolgreicher Nummernzuweisung muss auf der W80DM noch ein Factory-Reset durchgeführt werden, damit die zugewiesenen Nummern automatisch übernommen werden. Die Zuweisung und Registrierung der DECT-Mobilteile efolgt dann ebenfalls über die GUI der Basis-Station:

1. Die Nebenstelle (Mobilteil) sollte nun in der Übersicht vorhanden sein. 
    
![Registrierung_Mobilteil_2](https://user-images.githubusercontent.com/99875491/187174245-8b336160-c308-48df-a170-3a97d932b634.jpeg)

2. Klicken Sie auf das "Bearbeiten-Symbol"
    
![Registrierung_Mobilteil_3](https://user-images.githubusercontent.com/99875491/187174266-07776bac-8118-4b96-ad43-23d2529cb98c.jpeg)

3. Tragen Sie unter "IPUI"(International Portable User Identity) die IPUI des Mobilteils ein und klicken Sie auf "Mobilteil registrieren starten"
    ( Die IPUI Ihres Mobilteils können Sie folgendermaßen ermitteln: Beispiel W53H -> Menü (OK) / Status / Mobilteil)

4. Starten Sie zeitnah die Mobilteil-Anmeldung ( siehe weiter unten)
5. Wenn das Mobilteil erfolgreich an der Basisstation angemeldet wurde, erscheint es in der Übersicht:

![Registrierung_Mobilteil_4](https://user-images.githubusercontent.com/99875491/187174295-ff6f4d6d-177d-4867-be4b-664aa2d2b025.jpeg)

### Mobilteil anmelden ( Im Falle eines W53H )

1. OK-Taste
2. Menue-Punkt "Einstellungen"
3. Punkt "6.Registrieren"
4. "Mobilteil registrieren"
5. Basisstation ersetzen
6. Nun werden Sie von Ihrem Mobilteil aufgefordert, die PIN einzugeben. Im Auslieferungszustand lautet die PIN "0000"
7. Nun ist das Mobilteil an der DECT IP Basisstation angemeldet 

### Yealink W80DM (W80DM-30)
Diese Basisstation wandelt das IP-Protokoll der Cloud PBX in das DECT-Protokoll umd und bildet damit die Brücke zwischen Internet-Anschluss Ihren DECT-Telefonen.

Durch Klicken auf die entsprechende Nummer , weisen Sie dem Gerät die entsprechende Nebenstelle zu:

![W80DM-30](https://user-images.githubusercontent.com/99875491/195816325-aee911dd-1490-4dc5-826b-80c3ef8b2c2b.png)

Nach erfolgreicher Nummernzuweisung muss auf der W80DM noch ein Factory-Reset durchgeführt werden, damit die zugewiesenen Nummern automatisch übernommen werden. Die Zuweisung und Registrierung der DECT-Mobilteile efolgt dann ebenfalls über die GUI der Basis-Station:

1. Die Nebenstelle (Mobilteil) sollte nun in der Übersicht vorhanden sein. 
    
![Registrierung_Mobilteil_2](https://user-images.githubusercontent.com/99875491/187174245-8b336160-c308-48df-a170-3a97d932b634.jpeg)

2. Klicken Sie auf das "Bearbeiten-Symbol"
    
![Registrierung_Mobilteil_3](https://user-images.githubusercontent.com/99875491/187174266-07776bac-8118-4b96-ad43-23d2529cb98c.jpeg)

3. Tragen Sie unter "IPUI"(International Portable User Identity) die IPUI des Mobilteils ein und klicken Sie auf "Mobilteil registrieren starten"
    ( Die IPUI Ihres Mobilteils können Sie folgendermaßen ermitteln: Beispiel W53H -> Menü (OK) / Status / Mobilteil)

4. Starten Sie zeitnah die Mobilteil-Anmeldung ( siehe weiter unten)
5. Wenn das Mobilteil erfolgreich an der Basisstation angemeldet wurde, erscheint es in der Übersicht:

![Registrierung_Mobilteil_4](https://user-images.githubusercontent.com/99875491/187174295-ff6f4d6d-177d-4867-be4b-664aa2d2b025.jpeg)

### Mobilteil anmelden ( Im Falle eines W53H )

1. OK-Taste
2. Menue-Punkt "Einstellungen"
3. Punkt "6.Registrieren"
4. "Mobilteil registrieren"
5. Basisstation ersetzen
6. Nun werden Sie von Ihrem Mobilteil aufgefordert, die PIN einzugeben. Im Auslieferungszustand lautet die PIN "0000"
7. Nun ist das Mobilteil an der DECT IP Basisstation angemeldet 


*IN VORBEREITUNG: ### Snom M900 DECT-Basisstation*
*Diese Basisstation wandelt das IP-Protokoll der Cloud PBX in das DECT-Protokoll umd und bildet damit die Brücke zwischen Internet-Anschluss Ihren DECT-Telefonen. Die M900 bietet neben einem integrierten DECT-Manager auch eine DECT- und LAN-Synchronisierung. Der SIP-Transport kann neben UDP auch mittels TCP oder TLS erfolgen. Mit "Seamless Handover" ist der nahtlose Wechsel von einer Basisstation zur nächsten möglich.*

![cloudpbx_Gerät3 hinzufügen](https://user-images.githubusercontent.com/98753538/157050358-01266501-cc69-4e7a-b46f-cf0dddebf921.jpg)

*Kompatible Mobilteile sind M25, M65, M70, M80, M85, M90. Jedes DECT-Telefon muss der Basisstation zugewiesen werden.*

![cloudpbx_Teilnehmer einrichten2](https://user-images.githubusercontent.com/98753538/157249871-a15e2c1a-8ee4-4af3-995e-a4dde92cd579.jpg)

*Bei der SNOM-Basisstation können bis zu 19 Teilnehmer eingerichtet werden. Im Beispiel sind es zwei:*

![cloudpbx_Teilnehmer einrichten5](https://user-images.githubusercontent.com/98753538/157256005-95ef62fb-dcec-42a6-915e-8888618f1e67.jpg)

*IN VORBEREITUNG: #### Anmeldung der Snom-Mobilteile (Handsets)*

*Im Fritzbox-Meü -> Heimnetz -> Netzwerk kann man unter "Netzwerkverbindungen" die IP-Adresse der DECT-Basisstation einsehen bzw. diese auswählen:*

![Cloudpbx_einrichten_snom_dect_fritzbox](https://user-images.githubusercontent.com/98753538/157690228-f65b389b-9384-42ec-acd8-79b36f1ba638.jpg)

*So gelangen Sie zum Web-Interface Ihrer Snom M900. Im Menüpunkt "Extensions" können Sie die verbundenen Mobilteile einsehen und weitere hinzufügen. Dafür wählen Sie das entsprechenden Gerät mit einem Häkchen aus und klicken auf "Register Handset(s)". Daraufhin wird Ihnen im oberen Bereich der Access-Code (AC), hier "7666" angezeigt.*

![Cloudpbx_einrichten_snom_dect_endgeräte3](https://user-images.githubusercontent.com/98753538/157692195-9bae9037-8950-4312-8380-033f61c84253.jpg)

*Parallel dazu wählen Sie im Handset/Mobilteil den Punkt "Connectivity", dann "Register", tragen hier den Access-Code ein und bestätigen diesen mit "OK".*

![Handheld hinzufügen](https://user-images.githubusercontent.com/98753538/157691802-be0a428d-e6e9-49a4-b753-b00f016dbb6b.jpg)

*Abschließend aktualisieren Sie im Web-Interface die Ansicht "Extension" und sehen alle registrierten Mobilteile:*

![Cloudpbx_einrichten_snom_dect_endgeräte4](https://user-images.githubusercontent.com/98753538/157692597-70050298-c579-4109-b648-41ad36701c50.jpg)

*Sind die angemeldeten Handsets noch nicht sichtbar, ist gegebenenfalls im Menüpunkt "Home/Status" ein Reboot der DECT-Basisstation sinnvoll.*

![Cloudpbx_einrichten_snom_dect_reboot](https://user-images.githubusercontent.com/98753538/157691428-c41043ce-f043-4586-ac25-4365ba70e299.jpg)
