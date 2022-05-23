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


