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

![PW_Aendern_Regel](https://user-images.githubusercontent.com/99875491/223705005-0f615291-8dac-4abc-ad11-d1071340c51e.jpg)

Username und Passwort lauten im Auslieferungs-Zustand beide "admin". Bitte beachten Sie, dass beim erstmaligem Zugriff das Passwort geändert werden 
muss entsprechend der dargestellten Passwort-Regeln.

### Konfiguration Basis-Sataion

1. Navigieren sie zu „Einstellungen“
2. Wählen sie „Provider- oder PBX-Profile aus
3. Klicken sie auf IP1 um die Leitung zu bearbeiten

![Provider_oder_PBX_Profil_1](https://user-images.githubusercontent.com/99875491/223705089-178acdc5-2912-41d6-b81e-109ce3e1cea7.jpg)

4. Eintragen des Profilnamens ( frei wählbar )
5. Eintragen der Domain
6. Eintragen der Proxy Serveradresse (identisch mit Domain) – Serverport auf 5061 ändern
7. Transportprotokoll auf TLS setzen, SRTP auswählen

![Provider_oder_PBX_Profil_2](https://user-images.githubusercontent.com/99875491/223706265-46051314-323d-4c43-86ff-908115c4c373.jpg)

8. Für DNS Abfrage SRV + A auswählen
9. Outbound Proxymode auf „Immer“ setzen
10. Eintragen der Serveradresse (identisch mit Domain)
11. Outbound Proxyport auf 5061
12. SIP Subsribe für MWI auf Ja

![Provider_oder_PBX_Profil_3](https://user-images.githubusercontent.com/99875491/223705235-35c21a35-0db7-4b2a-a319-566df24399ce.jpg)

13. Hier keine Änderungen vornehmen; Standardwerte übernehmen

![Provider_oder_PBX_Profil_4](https://user-images.githubusercontent.com/99875491/223705288-aaea1e2f-0a65-4caf-82f5-bc52969f3a9a.jpg)
![Provider_oder_PBX_Profil_5](https://user-images.githubusercontent.com/99875491/223705309-bff6c850-06a4-4d28-ace0-99f8e3dde70d.jpg)

14. Unter "Signalisierungsoptionen für "Halten" im Session Description Protocol (SDP) bitte "nur Senden" wählen
15. Einstellungen sichern

### Konfiguration Mobilteil 

16. Klicken sie nun auf Mobilteile und Navigieren sie zum Punkt Verwaltung
17. Um ein Mobilteil hinzuzufügen, klicken sie auf „Hinzufügen“

![Mobilteile_Verwaltung_1](https://user-images.githubusercontent.com/99875491/223705372-722acd8d-3a2f-46ca-818c-d89e8e654f12.jpg)

18. Tragen Sie bitte unter "IPUI" die IPUI ihres Mobilteiles ein. Um die IPUI anzeigen zu lassen, drücken sie auf dem Handset auf Menü. 
Während das Menü angezeigt wird '*#06#' eingeben, dann erscheint zuoberst die IPEI (IPUI).
19. Tragen Sie dann unter "Persönliche Providerdaten" die Daten Ihres SIP-Accounts ein, welche Sie von NetCologne erhalten haben
20. Tragen Sie unter „Anmeldename“ den SIP Usernamen ein
21. Tragen Sie unter "Anmeldepasswort" das SIP Passwort ein
22. Wiederholen Sie die Eingabe des Benutzernamens unter „Benutzername“
23. Geben Sie den angezeigten Namen ein. Der Name kann frei gewählt werden
24. Wählen Sie bei Voip-Provider das eben eigerichtete Profil aus (unter 4. festgelegt)

![Mobilteile_Verwaltung_2](https://user-images.githubusercontent.com/99875491/223705414-b9863011-dc05-4472-b1b0-f99f84a67101.jpg)
 
 Hier bitte Standard-Werte übernehmen.

![Mobilteile_Verwaltung_3](https://user-images.githubusercontent.com/99875491/223705462-53ca6bd4-254c-4451-bf71-c7f561a4110c.jpg)

Hier bitte ebenfalls Standard-Werte übernehmen.

![Mobilteile_Verwaltung_4](https://user-images.githubusercontent.com/99875491/223705516-d0381d04-00f3-4522-915e-7dbdc91da12f.jpg)
![Mobilteile_Verwaltung_5](https://user-images.githubusercontent.com/99875491/223705536-6dbe72c8-677f-4f0e-bbab-92ae8cc90f04.jpg)

Klicken Sie auf "Sichern", um die Anmelde-Daten zu speichern.
Nun sehen Sie den Status Ihres eingerichteten Mobilteils ( Nicht angemeldet )

![Mobilteile_Verwaltung_6](https://user-images.githubusercontent.com/99875491/223705619-14272aaa-ff25-4ac4-a1fa-9d72e17dd7cd.jpg)

### Mobilteil anmelden 

26. Wählen Sie im nächsten Schritt das soeben eingerichtet Mobilteil aus ( Bearbeiten )
27. Wählen Sie unter RegStatus "Zur Anmeldung" aus.
28. Klicken Sie dann auf "Anmeldung starten"

![Mobilteile_Verwaltung_7](https://user-images.githubusercontent.com/99875491/223705721-b0c97193-2a74-4310-a642-4bfbd07a65ee.jpg)
![Mobilteile_Verwaltung_8](https://user-images.githubusercontent.com/99875491/223717235-286450b7-8d9b-4915-b1a0-8ae222defd1f.jpg)

29. Wählen Sie im Menü ihres Mobilteils den Punkt "Mobilteil anmelden" aus. Es wird nun die PIN abgefragt. Falls Sie 
diese im Einrichtungsprozess nicht geändert haben, ist sie i.d.R. "0000".

![Mobilteile_Verwaltung_9](https://user-images.githubusercontent.com/99875491/223705788-c3387b53-a2b7-4cd4-ad0a-37d62cba5132.jpg)

Die erfolgreiche Anmeldung können Sie überprüfen, indem Sie unter "Mobilteile -> Verwaltung" den Status des/der Mobilteile anzeigen lassen.
Bei erfolgreicher Anmeldung ist der Status "Angemeldet". Damit ist gleichzeitig der jeweilige SIP-Account erfolgreich an der Cloud-PBX registriert.


