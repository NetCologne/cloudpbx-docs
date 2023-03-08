---
title: "Gigaset"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "endgeraete"
weight: 513
toc: true
---

In diesem Kapitel erhalten Sie eine Anleitung für die manuelle Konfiguration der IP-DECT Basis-Station Gigaset N670.

### Zugangsdaten 

Der Zugriff auf das WebInterface erfolgt über einen Web Browser mit http://IPAdresse, wobei die IP Adresse im lokalen Router ausgelesen werden kann:

![PW_Aendern_Regel](https://user-images.githubusercontent.com/99875491/223677469-1875d022-eb2d-489e-a81e-4a537eb9bb3b.jpg)

Username und Password lauten im Auslieferungs-Zustand beide "admin". Bitte beachten Sie, dass beim erstmaligem Zugriff das Passwort geändert werden 
muss entsprechend der dargestellten Passwort-Regeln.

### Konfiguration Basis-Sataion

1. Navigieren sie zu „Einstellungen“
2. Wählen sie „Provider- oder PBX-Profile aus
3. Klicken sie auf IP1 um die Leitung zu bearbeiten

![Provider_oder_PBX_Profil_1](https://user-images.githubusercontent.com/99875491/223679646-3b803763-4cc8-451a-99a5-dc147e948057.jpg)

4. Eintragen des Profilnamens
5. Eintragen der Domain
6. Eintragen der Proxy Serveradresse (identisch mit Domain) – Serverport auf 5061 ändern
7. Transportprotokoll auf TLS setzen, SRTP auswählen

![Provider_oder_PBX_Profil_2](https://user-images.githubusercontent.com/99875491/223679667-181d03d3-9104-407a-b96f-43eda7628e7f.jpg)

8. Für DNS Abfrage SRV + A auswählen
9. Outbound Proxymode auf „Immer“ setzen
10. Eintragen der Serveradresse (identisch mit Domain)
11. Outbound Proxyport auf 5061
12. SIP Subsribe für MWI auf Ja

![Provider_oder_PBX_Profil_3](https://user-images.githubusercontent.com/99875491/223679681-449dc688-bad4-4c2f-98ed-769db94c6ad6.jpg)

13. Hier keine Änderungen vornehmen; Standardwerte übernehmen

![Provider_oder_PBX_Profil_4](https://user-images.githubusercontent.com/99875491/223679698-4f1df498-52cb-4c79-918e-b25f0572b9f6.jpg)
![Provider_oder_PBX_Profil_5](https://user-images.githubusercontent.com/99875491/223679712-42b171b8-8ab2-4886-94c0-cfbd33717f36.jpg)

14. Unter "Signalisierungsoptionen für "Halten" im Session Description Protocol (SDP) bitte "nur Senden" wählen
15. Einstellungen sichern

### Konfiguration Mobilteil 

16. Klicken sie nun auf Mobilteile und Navigieren sie zum Punkt Verwaltung
17. Um ein Mobilteil hinzuzufügen, klicken sie auf „Hinzufügen“

![Mobilteile_Verwaltung_1](https://user-images.githubusercontent.com/99875491/223686097-0b4a3c69-ecfc-4979-a881-a8be7b29dc6c.jpg)

18. Tragen Sie bitte unter "IPUI" die IPUI ihres Mobilteiles ein. Um die IPUI anzeigen zu lassen, drücken sie auf dem Handset auf Menü. 
Während das Menü angezeigt wird '*#06#' eingeben, dann erscheint zuoberst die IPEI (IPUI).
19. Tragen Sie dann unter "Persönliche Providerdaten" die Daten Ihres SIP-Accounts ein, welche Sie von NetCologne erhalten haben
20. Tragen Sie unter „Anmeldename“ den SIP Usernamen ein
21. Tragen Sie unter Anmeldepasswort das SIP Passwort ein
22. Wiederholen Sie die Eingabe des Benutzernamens unter „Benutzername“
23. Geben Sie den angezeigten Namen ein. Der Name kann frei gewählt werden
24. Wählen Sie bei Voip-Provider das eben eigerichtete Profil aus (unter 4. festgelegt)

![Mobilteile_Verwaltung_2](https://user-images.githubusercontent.com/99875491/223686138-e2a49c2b-002e-4c71-9f77-5266530f9da6.jpg)
 
 Hier bitte Standard-Werte übernehmen.

![Mobilteile_Verwaltung_3](https://user-images.githubusercontent.com/99875491/223688339-b0aea619-ffff-4ee2-ac84-609a145342e3.jpg)

Hier bitte ebenfalls Standard-Werte übernehmen.

![Mobilteile_Verwaltung_4](https://user-images.githubusercontent.com/99875491/223686206-f76ce24e-54dd-4b62-adf2-8978ab0d8e4f.jpg)

25. Klicken Sie auf "Sichern", um die Anmelde-Daten zu speichern.

![Mobilteile_Verwaltung_5](https://user-images.githubusercontent.com/99875491/223686238-c029c9c0-5628-44bf-bb57-99575678b725.jpg)

Nun sehen Sie den Status Ihres eingerichteten Mobilteils ( Nicht angemeldet )

![Mobilteile_Verwaltung_6](https://user-images.githubusercontent.com/99875491/223686269-7c8bde46-fa6c-49e0-b8c2-045215ecb9a1.jpg)

### Mobilteil anmelden 

26. Wählen Sie im nächsten Schritt das soeben eingerichtet Mobilteil aus ( Bearbeiten )
27. Wählen Sie unter RegStatus "Zur Anmeldung" aus.
28. Klicken Sie dann auf "Anmeldung starten"

![Mobilteile_Verwaltung_7](https://user-images.githubusercontent.com/99875491/223686336-a27701d2-cafb-4e7c-8771-c4dfab46adf9.jpg)
![Mobilteile_Verwaltung_8](https://user-images.githubusercontent.com/99875491/223686396-c40456ab-4113-4fc7-95dc-abf374935a09.jpg)

29. Wählen Sie im Menü ihres Mobilteils den Punkt "Mobilteil anmelden" anmelden aus. Es wird nun die PIN abgefragt. Falls Sie diese im Einrichtungsprozess nicht geändert haben, ist sie i.d.R. "0000".

![Mobilteile_Verwaltung_9](https://user-images.githubusercontent.com/99875491/223686435-4130d94c-82be-414f-ae78-b44e7b5c7538.jpg)

Die erfolgreiche Anmeldung können Sie überprüfen, indem Sie unter "Mobilteile -> Verwaltung" den Status des/der Mobilteile anzeigen lassen.
Bei erfolgreicher Anmeldung ist der Status "Angemeldet". Damit ist gleichzeitig der jeweilige SIP-Account erfolgreich an der Cloud-PBX registriert.


