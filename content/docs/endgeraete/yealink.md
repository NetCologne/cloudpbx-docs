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

Username und Password lauten beide "admin".

![NC_Doku_Konto_Registrieren_03](https://user-images.githubusercontent.com/99875491/169790420-1c3212da-9da1-4103-81f8-684dacdbbf87.jpg)

![NC_Doku_Konto_Registrieren_02](https://user-images.githubusercontent.com/99875491/169790505-ac107f95-6d75-4cb3-b895-47b47a7060fe.jpg)


1. Begeben Sie sich zu dem Menüpunkt "Konto".
3. Wählen Sie nun den Punkt "Registrieren" aus.
4. Im ersten Schritt der Einrichtung wählen Sie das betreffende Konto im oberen Reiter aus.
5. Aktivieren Sie die Leitung mit Auswahl von "An".
6. Unter "Label" und "Anzeigename" können Sie einen selbst gewählte Namen für Ihr Telefon einsetzen.
7. Unter "Registrierterungsname" und "Benutzernamen" setzen Sie den SIP-Benutzernamen ein. Diesen erhalten Sie nach Anlegen des Telefons im Kundenkonto.
8. Das SIP-Passwort finden Sie ebenfalls in Ihren SIP-Benutzerdaten.
9. Bei "Server Host" tragen Sie bitte die Server-URL "firmaid.cloudpbx.netcologne.de" ein. Unter "Port" muss "5061" stehen.
10. Unter "Transport" wählen Sie "TLS" aus.
11. Bitte aktivieren Sie den "Outbound Proxy Server", indem Sie in dem Reiter den Punkt "An" auswählen.
12. Beim Punkt "Ausgehender Proxy Server 1" tragen Sie bitten Ihren Proxy Server ein: “firmaid.cloudpbx.netcologne.de“. 
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

Schließen Sie zuallererst Ihren Yealink DECT IP Multi-Cell DECT-Manager W80DM und und mindestens eine Yealink DECT IP Basisstation W80B ans Stromnetz und an Ihr Netzwerk an. 

![W80_Bild](https://user-images.githubusercontent.com/99875491/187176231-eec46598-65d6-40fa-88e6-9edf7a44754c.jpg)

Empfehlung: Sie haben die Möglichkeit, Ihren DECT IP Multi-Cell DECT-Manager W80DM automatisch über das NetCologne Cloud PBX einzurichten. Lesen Sie dazu die Hilfe Automatische Konfiguration.

Hier wird beschrieben, wie Sie das Gerät manuell einrichten können.

### Zugangsdaten 

Der Zugriff auf das WebInterface erfolgt über einen Web Browser mit http://IPAdresse, wobei die IP Adresse im lokalen Router ausgelesen werden kann:

![Zugangsdaten](https://user-images.githubusercontent.com/99875491/187174035-35fc98f6-af4a-426f-b626-84e45ccef110.jpeg)

Username und Password lauten beide "admin".

### Konfiguration

1. Begeben Sie sich zu dem Menüpunkt "Handset & Account".
2. Wählen Sie nun den Punkt "SIP-Servereinstellungen" aus.
3. Im ersten Schritt der Einrichtung klicken Sie bitte auf das Bearbeitungs-Symbol rechts in der Tabelle. 
   Es öffnet sich folgende Eingabe-Maske: 

![SIP_Server_Einstellungen_1](https://user-images.githubusercontent.com/99875491/187174069-36c4621e-5f1b-49fb-bc6c-cb0e21b92b0f.jpeg)
![SIP_Server_Einstellungen_2](https://user-images.githubusercontent.com/99875491/187174090-811d5566-3ac0-46b0-a3b9-fb36b977137f.jpeg)

4. Unter "Name der Vorlage" vergeben Sie bitte eine Bezeichnung Ihrer Wahl.
5. Bei "Server Host" tragen Sie bitte die Server-URL "firmaid.cloudpbx.netcologne.de" ein. 
6. Unter "Transport" wählen Sie "TLS" aus.
7. Unter "Ausgehender Proxy-Server 1" tragen Sie bitte "firmaid.cloudpbx.netcologne.de" ein. Unter "Port" muss "5061" stehen.
8. Falls Sie bisher noch keine Yealink DECT IP Basisstation W80B angeschlossen haben, müssen Sie dies im nächsten Schritt nachholen.
9. Die angeschlossene(n) Basis-Statione(n) sehen Sie unter Punkt "Registrieren Basis-Station"
   
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

### Konfiguration

## Yealink HD IP Conference Phone CP965

### Zugangsdaten 

### Konfiguration


