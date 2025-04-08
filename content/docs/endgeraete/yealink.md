---
title: "Yealink"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "endgeraete"
weight: 502
toc: true
---

Hier geben wir Ihnen eine Einführung zu Ihrem Yealink VoIP Telefon. Im ersten Schritt machen Sie sich mit der Tastenbelegung Ihres Telefons vertraut und bekommen dann eine Schritt-für-Schritt-Anleitung zur Einrichtung Ihres Telefons.

>💡**Hinweis**  
>Aktuell liefert Yealink neue Tischtelefone (mindestens der T5-Serie) mit der Firmware-Version **96.86.0.75** aus. Zu dieser Version liegen keine Releasenotes vor. Auch ist sie nicht auf der Homepage von Yealink zu finden. Bei dieser Version werden die Einstellungen für TLS, Outbound-Proxy und Port nicht automatisch provisioniert. Entweder installieren Sie die vorherige Version **96.86.0.70** (Download siehe https://firmware.cloudpbx.netcologne.de/files/) oder ergänzen die Parameter manuell über die GUI unter Konto->Registrieren des Telefons:<br><br>
> SIP-Server 1 -> Transport: TLS<br>
> Ausgehenden Proxy-Server aktivieren: An<br>
> Ausgehender Proxy-Server 1: **kunde**.cloudpbx.netcologne.de Port: **5061**<br><br>
> ![Konto_TLS_outbound-prxy_manuell](https://github.com/NetCologne/cloudpbx-docs/assets/99875470/9646f2bd-5579-48c5-9027-05c9479a3a90)<br>
> Bei einem Neustart des Telefons bleibt die Einstellung erhalten. Nach dem Zurücksetzen auf Werkseinstellungen muss die Einstellung allerdings wieder manuell nachgetragen werden.<br>

Empfehlung: Sie haben die Möglichkeit, Ihr Yealink VoIP Telefon automatisch über das NetCologne Cloud PBX einzurichten. Lesen Sie dazu die Hilfe Automatische Konfiguration.

Gehen Sie zu Manuelle Konfiguration wenn Sie das Gerät lieber manuell einrichten wollen.

## Tastenbelegung

Nun machen Sie sich mit der Tastenbelegung des Yealink vertraut.

Unterschiedliche Modelle bieten eine unterschiedliche Anzahl von Funktionstasten. Fehlt an Ihrem Modell eine Funktionstaste, kann die Funktion über die jeweilige Display-Taste aufgerufen werden. Lesen Sie mehr dazu unter Funktionen.

## Yealink DECT IP Basisstation W70B

Schließen Sie zuallererst Ihre Yealink DECT IP Basisstation W70B am Stromnetz und an Ihr Netzwerk an. 

![NC_Doku_W70B-front](https://user-images.githubusercontent.com/99875491/169034722-72b71c3d-5147-4359-b750-3fe9fe09b159.jpg)

Empfehlung: Sie haben die Möglichkeit, Ihre Yealink DECT IP Basisstation automatisch über das NetCologne Cloud PBX einzurichten. Lesen Sie dazu die Hilfe Automatische Konfiguration.

Hier wird beschrieben, wie Sie das Gerät manuell einrichten können.

### Zugangsdaten 

Der Zugriff auf das WebInterface erfolgt über einen Web Browser mit http://IPAdresse, wobei die IP Adresse im lokalen Router ausgelesen werden kann:

![NC_Doku_Login](https://user-images.githubusercontent.com/99875491/169037825-ceb507ee-9886-4f5e-8ef7-3409a2bc55e8.jpg)

Username und Password lauten beide "admin". <br>
<br> 💡 **Hinweis:** Bei Anlagen, die von NetCologne eingerichtet wurden, werden aus Sicherheitsgründen keine Standardpasswörter verwendet. Sollten Sie das Administrator-Kennwort benötigen, wenden Sie sich bitte an den Geschäftskunden-Support.

![NC_Doku_Konto_Registrieren_03](https://github.com/NetCologne/cloudpbx-docs/assets/99875491/e3959192-c1ff-443b-826f-f26569121b64)


![NC_Doku_Konto_Registrieren_02](https://github.com/NetCologne/cloudpbx-docs/assets/99875491/30e1ccb2-72ae-4dd7-afaa-e41214398aee)



1. Begeben Sie sich zu dem Menüpunkt "Konto".
3. Wählen Sie nun den Punkt "Registrieren" aus.
4. Im ersten Schritt der Einrichtung wählen Sie das betreffende Konto im oberen Reiter aus.
5. Aktivieren Sie die Leitung mit Auswahl von "An".
6. Unter "Label" und "Anzeigename" können Sie einen selbst gewählte Namen für Ihr Telefon einsetzen.
7. Unter "Registrierungsname" und "Benutzernamen" setzen Sie den SIP-Benutzernamen ein. Diesen erhalten Sie nach Anlegen des Telefons im Kundenkonto.
8. Das SIP-Passwort finden Sie ebenfalls in Ihren SIP-Benutzerdaten.
9. Bei "Server Host" tragen Sie bitte die Server-URL, welche Ihnen von NetCologne mitgeteilt wurde, ein. Unter "Port" muss "5061" stehen.
10. Unter "Transport" wählen Sie "TLS" aus.
11. Bitte aktivieren Sie den "Outbound Proxy Server", indem Sie in dem Reiter den Punkt "An" auswählen.
12. Beim Punkt "Ausgehender Proxy Server 1" tragen Sie bitten Ihren Proxy Server ein welcher Ihnen von NetCologne mitgeteilt wurde. 
Unter "Port" muss "5061" stehen.
12. Stellen Sie sicher, dass "NAT" auf "Deaktiviert" gestellt wird.
15. Mit Klick auf "Bestätigen" ist die Konfiguration abgeschlossen. 

### Verschlüsselung
Ihre Gesprächsdaten/Inhalte werden verschlüsselt übertragen. Bitte stellen Sie hierzu sicher, dass folgende Einstellung aktiv ist ( SRTP )

![NC_Doku_SRTP_Obligatorisch](https://user-images.githubusercontent.com/99875491/169795970-996dd398-d9f6-4c9e-b820-9f6106d18373.jpg)

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

## Yealink DECT IP Multi-Cell DECT-Manager W80DM

Schließen Sie zuallererst Ihren Yealink DECT IP Multi-Cell DECT-Manager W80DM und mindestens eine Yealink DECT IP Basisstation W80B ans Stromnetz und an Ihr Netzwerk an. 

![W80_Bild](https://user-images.githubusercontent.com/99875491/187176231-eec46598-65d6-40fa-88e6-9edf7a44754c.jpg)

Empfehlung: Sie haben die Möglichkeit, Ihren DECT IP Multi-Cell DECT-Manager W80DM automatisch über das NetCologne Cloud PBX einzurichten. Lesen Sie dazu die Hilfe Automatische Konfiguration.

Hier wird beschrieben, wie Sie das Gerät manuell einrichten können.

### Zugangsdaten 

Der Zugriff auf das WebInterface erfolgt über einen Web Browser mit http://IPAdresse, wobei die IP Adresse im lokalen Router ausgelesen werden kann:

![Zugangsdaten](https://user-images.githubusercontent.com/99875491/187174035-35fc98f6-af4a-426f-b626-84e45ccef110.jpeg)

Username und Password lauten beide "admin". <br>
<br> 💡 **Hinweis:** Bei Anlagen, die von NetCologne eingerichtet wurden, werden aus Sicherheitsgründen keine Standardpasswörter verwendet. Sollten Sie das Administrator-Kennwort benötigen, wenden Sie sich bitte an den Geschäftskunden-Support.

### Konfiguration

1. Begeben Sie sich zu dem Menüpunkt "Handset & Account".
2. Wählen Sie nun den Punkt "SIP-Servereinstellungen" aus.
3. Im ersten Schritt der Einrichtung klicken Sie bitte auf das Bearbeitungs-Symbol rechts in der Tabelle. 
   Es öffnet sich folgende Eingabe-Maske:
   
![SIP_Server_Einstellungen_1](https://github.com/NetCologne/cloudpbx-docs/assets/99875491/0a2cc63e-5710-4422-a290-19f35ec917f0)
![SIP_Server_Einstellungen_2](https://github.com/NetCologne/cloudpbx-docs/assets/99875491/d0858bbe-ebf0-4d60-b8a5-ae3fc05505d1)

5. Unter "Name der Vorlage" vergeben Sie bitte eine Bezeichnung Ihrer Wahl.
6. Bei "Server Host" tragen Sie bitte die Server-URL, welche Ihnen von NetCologne mitgeteilt wurde, ein. 
7. Unter "Transport" wählen Sie "TLS" aus.
8. Unter "Ausgehender Proxy-Server 1" tragen Sie bitte den Proxy-Server, welcher Ihnen von NetCologne mitgeteilt wurde, ein. Unter "Port" muss "5061" stehen.
9. Falls Sie bisher noch keine Yealink DECT IP Basisstation W80B angeschlossen haben, müssen Sie dies im nächsten Schritt nachholen.
10. Die angeschlossene(n) Basis-Station(en) sehen Sie unter Punkt "Registrieren Basis-Station"
   
![Registrieren_Basis_Station](https://user-images.githubusercontent.com/99875491/187176771-82f43a3a-ec23-418e-bb66-d864330141e4.jpeg)

10. Klicken Sie hier auf das Verbindungs-Symbol, um die Basis-Station zu registrieren. 
    Es öffnet sich folgende Maske, in der Sie nichts zu ändern brauchen. Quittieren Sie bitte mit "OK".

![Registrieren_Basis_Station_1](https://user-images.githubusercontent.com/99875491/187175571-86be43ba-2cac-4351-b5f2-b9a248545ae8.jpeg)

11. Unter Menüpunkt "Einstellungen Basisstation" können Sie sehen, ob die Registrieung der Basisstation(en) erfolgreich war:

![Einstellungen_Basis_Station](https://user-images.githubusercontent.com/99875491/187174127-c83879bf-7108-44fe-bd64-d62e5236432f.jpeg)

( Falls Sie weitere Basis-Stationen anschliessen möchten, wiederholen Sie die Aktion, wie unter Punkt 10. beschrieben. Es sind ausser dem Anschliessen ans Netzwerk keine weiteren Konfigurationsmaßnahmen notwendig. )

12. Nun können Mobilteile angemeldet werden. Gehen Sie hierzu unter Punkt "Registrierung Mobilteil"

![Registrierung_Mobilteil](https://user-images.githubusercontent.com/99875491/187174164-e54650d4-f636-4646-8671-4ffd56cfdbba.jpeg)

13. Unter "Label" und "Anzeigename" können Sie einen selbst gewählte Namen für Ihr Telefon einsetzen.
14. Unter "Registrierterungsname" und "Benutzernamen" setzen Sie den SIP-Benutzernamen ein. Diesen erhalten Sie nach Anlegen des Telefons im Kundenkonto.
15. Das SIP-Passwort finden Sie ebenfalls in Ihren SIP-Benutzerdaten.
16. Klicken Sie dann auf "Erweiterte Einstellungen anzeigen"

![Registrierung_Mobilteil_1](https://user-images.githubusercontent.com/99875491/187174225-3fb22c35-71d0-4f35-b7b5-0aaa4c0c7d48.jpeg)

17. Scrollen Sie bis zum Punkt "RTP-Verschlüsselugn (SRTP)" und wählen dort "obligatorisch" aus.
    Damit wird sichergestellt, dass ihre Gesprächsdaten/Inhalte verschlüsselt übertragen werden.

18. Das Mobilteil sollte nun in der Übersicht vorhanden sein. 
    
![Registrierung_Mobilteil_2](https://user-images.githubusercontent.com/99875491/187174245-8b336160-c308-48df-a170-3a97d932b634.jpeg)

19. Klicken Sie auf das "Bearbeiten-Symbol"
    
![Registrierung_Mobilteil_3](https://user-images.githubusercontent.com/99875491/187174266-07776bac-8118-4b96-ad43-23d2529cb98c.jpeg)

20. Tragen Sie unter "IPUI"(International Portable User Identity) die IPUI des Mobilteils ein und klicken Sie auf "Mobilteil registrieren starten"
    ( Die IPUI Ihres Mobilteils können Sie folgendermaßen ermitteln: Beispiel W53H -> Menü (OK) / Status / Mobilteil)

21. Starten Sie zeitnah die Mobilteil-Anmeldung ( siehe weiter unten)
22. Wenn das Mobilteil erfolgreich an der Basisstation angemeldet wurde, erscheint es in der Übersicht:

![Registrierung_Mobilteil_4](https://user-images.githubusercontent.com/99875491/187174295-ff6f4d6d-177d-4867-be4b-664aa2d2b025.jpeg)

### Mobilteil anmelden ( Im Falle eines W53H )

1. OK-Taste
2. Menue-Punkt "Einstellungen"
3. Punkt "6.Registrieren"
4. "Mobilteil registrieren"
5. Basisstation ersetzen
6. Nun werden Sie von Ihrem Mobilteil aufgefordert, die PIN einzugeben. Im Auslieferungszustand lautet die PIN "0000"
7. Nun ist das Mobilteil an der DECT IP Basisstation angemeldet 

## Yealink HD IP Conference Phone CP920

### Zugangsdaten 

Der Zugriff auf das WebInterface erfolgt über einen Web Browser mit http://IPAdresse, wobei die IP Adresse im lokalen Router ausgelesen werden kann:

![Zugangsdaten_920](https://user-images.githubusercontent.com/99875491/196953811-471560b6-56d5-493a-a66c-d03ed8da342a.jpeg)

Username und Password lauten beide "admin". <br>
<br> 💡 **Hinweis:** Bei Anlagen, die von NetCologne eingerichtet wurden, werden aus Sicherheitsgründen keine Standardpasswörter verwendet. Sollten Sie das Administrator-Kennwort benötigen, wenden Sie sich bitte an den Geschäftskunden-Support.

### Konfiguration

1. Begeben Sie sich zu dem Menüpunkt "Konto / Registrieren"; Setzen Sie bitte den Leitungsstatus auf "aktiviert", damit sich nach Abschluss der Konfiguration Ihr Konferenztelefon automatisch am NetCologne-Cloud-PBX-Server registriert.

![Registrieren_01](https://github.com/NetCologne/cloudpbx-docs/assets/99875491/c9e454bf-badc-436e-9349-5fde2f32467f)

2. Unter "Label" und "Anzeigename" können Sie einen selbst gewählte Namen für Ihr Konferenz-Telefon einsetzen.
3. Unter "Registrierterungsname" und "Benutzernamen" setzen Sie den SIP-Benutzernamen ein. Diesen erhalten Sie nach Anlegen des Telefons im Kundenkonto.
4. Das SIP-Passwort finden Sie ebenfalls in Ihren SIP-Benutzerdaten.
5. Bei "Server Host" tragen Sie bitte die Server-URL, welche Ihnen von NetCologne mitgeteilt wurde, ein. 
6. Unter "Transport" wählen Sie "TLS" aus.

![Registrieren_02](https://github.com/NetCologne/cloudpbx-docs/assets/99875491/63bd7bd8-5bc2-4fd6-893a-aa772a34fb48)

7. Unter "Ausgehender Proxy-Server 1" tragen Sie bitte den Proxy-Server, welcher Ihnen von NetCologne mitgeteilt wurde, ein. Unter "Port" muss "5061" stehen.
8. Klicken Sie dann auf "Erweitert"

![Erweitert_01](https://user-images.githubusercontent.com/99875491/196955107-dc81d8bd-f25a-4c39-a8c7-72883ba67dcc.jpeg)

9. Wählen Sie hier bei "Quelle Anrufer-ID" "PAI-VON"
10. Wählen Sie hier unter RTP-Verschlüsselung (SRTP) "Obligatorisch" aus.


## Yealink HD IP Conference Phone CP965

### Zugangsdaten 
Der Zugriff auf das WebInterface erfolgt über einen Web Browser mit http://IPAdresse, wobei die IP Adresse im lokalen Router ausgelesen werden kann:

![Zugangsdaten_965](https://user-images.githubusercontent.com/99875491/196953845-cfb21eae-19cb-4c3a-b119-d3b6ad7b372b.jpeg)

Username und Password lauten beide "admin". <br>
<br> 💡 **Hinweis:** Bei Anlagen, die von NetCologne eingerichtet wurden, werden aus Sicherheitsgründen keine Standardpasswörter verwendet. Sollten Sie das Administrator-Kennwort benötigen, wenden Sie sich bitte an den Geschäftskunden-Support.

### Konfiguration

1. Begeben Sie sich zu dem Menüpunkt "Konto / Registrieren". Setzen Sie bitte den Leitungsstatus auf "An", damit sich nach Abschluss der Konfiguration Ihr Konferenztelefon automatisch am NetCologne-Cloud-PBX-Server registriert.

![Registrieren_01](https://github.com/NetCologne/cloudpbx-docs/assets/99875491/2e43373c-da60-47eb-975c-b3b7b99dbb71)

2. Unter "Label" und "Anzeigename" können Sie einen selbst gewählte Namen für Ihr Konferenz-Telefon einsetzen.
3. Unter "Registrierterungsname" und "Benutzernamen" setzen Sie den SIP-Benutzernamen ein. Diesen erhalten Sie nach Anlegen des Telefons im Kundenkonto.
4. Das SIP-Passwort finden Sie ebenfalls in Ihren SIP-Benutzerdaten.
5. Bei "Server Host" tragen Sie bitte die Server-URL, welche Ihnen von NetCologne mitgeteilt wurde, ein. 
6. Unter "Transport" wählen Sie "TLS" aus.

![Registrieren_02](https://github.com/NetCologne/cloudpbx-docs/assets/99875491/efeacb0a-0e87-457d-9358-a77719e9aec0)

7. Unter "Ausgehender Proxy-Server 1" tragen Sie bitte den Proxy-Server, welcher Ihnen von NetCologne mitgeteilt wurde, ein. Unter "Port" muss "5061" stehen.
8. Klicken Sie dann auf "Erweitert"

![Erweitert_01](https://user-images.githubusercontent.com/99875491/196958328-97784b09-1f31-4133-8597-a43d2176a731.jpeg)

9. Wählen Sie hier bei "Quelle Anrufer-ID" "PAI-VON"
10. Wählen Sie hier unter RTP-Verschlüsselung (SRTP) "Obligatorisch" aus.

## Yealink EXP50 Erweiterungs-Modul

Das Yealink EXP50 Erweiterungs-Modul verfügt über ein 10,9cm Farb-Display und ist mit den Yealink SIP-T5-Reihe Business Media Telefonen kompatibel.
20 zweifarbige LED-Tasten über 3 Seiten bieten 60 programmierbare Tasten. Wenn mehr Tasten benötigt werden, können für insgesamt 180  programmierbare Tasten, 
bis zu 3 EXP50 Erweiterungs-Module durch Daisy Chaining miteinander verkabelt werden.

Tasten können für verschiedene Funktionen wie unter anderem Kurzwahl, BLF / BLA, Rufumleitung und Rufweiterleitung 
programmiert werden. Das Yealink EXP50 Erweiterungs-Modul wurde entwickelt um ein hohes Volumen von gleichzeitigen 
Anrufen verwalten zu können, einen mühelosen Überblick über Anrufe zu haben und um Ihre Produktivität extrem zu steigern.

Kompatible Geräte

Yealink SIP-T56A / SIP-T58V / SIP-T58A / SIP-T53 / SIP-T53W / SIP-T54W / SIP-T57W

Ansicht des Gerätes:

![EPX50](https://github.com/NetCologne/cloudpbx-docs/assets/99875491/e6493966-cb7b-4dfa-8e8b-25893c61ceca)

Ansicht des montierten Gerätes ( Yealink T57W + EXP50 )

![T57_EXP50](https://github.com/NetCologne/cloudpbx-docs/assets/99875491/c608ba8a-e26c-4ad0-a6eb-23bb97ed2bd3)

Montieren Sie zunächst das Erweiterungsmodul an das bereits bestehende und konfigurierte Basisgerät entsprechend
dem mitgelieferten Quick Start Guide. Im Anschluss wird beschrieben, wie Sie das EXP50 konfigurieren können.

### Zugangsdaten

Der Zugriff auf das WebInterface erfolgt über einen Web Browser mit http://IPAdresse, wobei die IP Adresse 
im lokalen Router ausgelesen werden kann:

![Yealink_T57_Login](https://github.com/NetCologne/cloudpbx-docs/assets/99875491/ff740e0c-de91-405d-bc77-351453897363)

Username lautet “admin”, Password lautet “adminpass”. <br>
<br> 💡 **Hinweis:** Bei Anlagen, die von NetCologne eingerichtet wurden, werden aus Sicherheitsgründen keine Standardpasswörter verwendet. Sollten Sie das Administrator-Kennwort benötigen, wenden Sie sich bitte an den Geschäftskunden-Support.

### Konfiguration

![EXP50_T57_DSS_Key_Konfig](https://github.com/NetCologne/cloudpbx-docs/assets/99875491/886c25c4-6856-43a1-8039-156199596aea)

1. Wählen Sie im linken Frame unter "Dsskey" den Punkt "Ext-Taste" aus.
2. Auf der nun dargestellten Seite können Sie die Tasten des EXP50 den von Ihnen gewünschten Funktionen zuordnen:
zB. BLF / Kurzwahl / Rufweiterleitung / Pick-Up / Übergeben/Transfer etc.
Übernommen werden die Daten mit Klick auf "Bestätitigen". Damit ist die Konfiguration abgeschlossen. 
Sie kann jedoch jederzeit angepasst oder verändert werden.


## Anleitung zum Entfernen eines Brandings

Gelegentlich kann es vorkommen, dass Endgeräte aus einer vorherigen Verwendung übernommen werden sollen. Wenn diese Geräte
auf einen bestimmten Hersteller "gebranded", d.h. mit einer speziellen Firmware ausgestattet sind, muss zuerst das Branding
durch Aufspielen einer Lizenzdatei entfernt werden. Anschließend kann die Standardfirmware in der aktuellen Version installiert werden.

Um die notwendige Lizenz zu bekommen, wenden Sie sich bitte an Ihren Ansprechpartner bei NetCologne. Dazu halten Sie bitte die MAC-Adressen der
betroffenen Endgeräte bereit.

Wenn Sie die erforderlichen Lizenzdateien bekommen haben sind folgende Schritte durchzuführen (hier am Beispiel eines SIP-T46S dargestellt):

Melden Sie sich über einen Browser auf der Bedieneroberfläche des entsprechenden Telefons an.

Im Menü "Sicherheit" wählen Sie den Eintrag "Lizenz".

![licence_importieren](https://github.com/NetCologne/cloudpbx-docs/assets/99875470/03aa96a4-160b-4586-b094-08086e88f149)

Laden Sie die zur Verfügung gestellte Lizenzdatei hoch.

Anschließend können Sie im Menü "Einstellungen" unter "Upgrade" die aktuelle neutrale Firmware installieren. Auf der Homepage https://www.yealink.com/ erhalten Sie die Firmware.

![fw-update](https://github.com/NetCologne/cloudpbx-docs/assets/99875470/db9f60ac-3dec-49c4-86d1-bc5ac3b08471)
