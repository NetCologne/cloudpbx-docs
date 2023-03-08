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

[PW_Aendern_Regel](https://user-images.githubusercontent.com/99875491/223677469-1875d022-eb2d-489e-a81e-4a537eb9bb3b.jpg)

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

13. Hier keine Änderungen vornehmen; Satndardwerte übernehmen

![Provider_oder_PBX_Profil_4](https://user-images.githubusercontent.com/99875491/223679698-4f1df498-52cb-4c79-918e-b25f0572b9f6.jpg)
![Provider_oder_PBX_Profil_5](https://user-images.githubusercontent.com/99875491/223679712-42b171b8-8ab2-4886-94c0-cfbd33717f36.jpg)

14. Unter "Signalisierungsoptionen für "Halten" im Session Description Protocol (SDP) bitte "nur Senden" wählen
15. Einstellungen sichern

### Konfiguration Mobilteil 



### Mobilteil anmelden 
