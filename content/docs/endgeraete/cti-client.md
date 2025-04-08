---
title: "CTI-Client"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "endgeraete"
weight: 511
toc: true
---

#### CTI - Computer Telephony Integration

CTI beschreibt eine Verbindung zwischen Computer und VoIP-Telefonanlage, die beidseitig genutzt werden kann. 
D.h. der Computer kommuniziert mit einem oder mehreren Telefonen und umgekehrt. 

Im ersten Fall ermöglicht eine CTI-Anwendung den automatischen Aufbau, die Annahme und Beendigung von Telefongesprächen, den Aufbau von Telefonkonferenzen, das Senden und Empfangen von Faxnachrichten, Telefonbuchdienste, sowie die Weitervermittlung von Gesprächen. Zudem werden Desktop-Funktionen bereitgestellt, wie z.B:

  - Dialogfenster – Anzeige mit Anrufinformationen (Nummer des Anrufers, gewählte Nummer)
  - Wählen – Automatische und computergesteuerte Einwahl.
  - Telefonsteuerung – Umfasst Anrufsteuerung (Anrufe entgegennehmen, auflegen, halten, Konferenzschaltung etc.) und Funktionen wie z.B. Anrufweiterleitung.
  - Durchstellen von Anrufen – Koordinierter Transfer von Anrufen und Daten zwischen zwei Gesprächsteilnehmern.

In der Umkehrrrichtung werden über eine automatische Anruferidentifikation die passenden Kundendaten aus einer Datenbank auf Ihren Bildschirm gebracht. Mittels Software werden Anrufberichte über geführte Gespräche angelegt. Per Datenbankaufruf kann die Nummer des Anrufers oder die gewählte Nummer ausgewertet und davon abhängig zu unterschiedlichen Zielen weitergeleitet werden.
Auch andere Systeme können über CTI mit Ihrer IP-Telefonanlage verbunden werden. Neben Applikationen, in denen die Kontaktdaten Ihrer Kunden gespeichert sind (z.B. Outlook, Lotus Notes), sind auch auch Support-Software oder spezielle Programme zur Auswertung der Telefonie möglich.

**Fazit:** Mit Hilfe von CTI können Sie mehr Effizienz in Ihren Arbeitsalltag bringen. Eine entsprechende Schnittstelle ermöglicht Ihnen den geschützten Zugriff zu Ihren digitalen Kundendaten wie z.B. Name, Position, Firma und Telefonnummer. Die wichtigsten *Funktionen* sind:

##### Click To Call
Durch einfachen Klick auf die Telefonnummer eines Kunden auf dem Bildschirm haben Sie die Möglichkeit einen Anruf über Ihre IP-Telefonanlage aufzubauen.

##### Reverse Lookup
Beim eingehenden Anruf eines Kunden, der bereits mit seiner Telefonnummer in Ihrer Datenbank gespeichert ist, wird automatisch der Kontakt geöffnet und Sie können sich die eingetragenen Informationen ansehen bevor Sie den Anruf entgegennehmen. Ihr Kundenkontakt wird noch persönlicher und kompetenter – direkt im Moment, in dem Sie das Telefon abheben.

Bei der NetCologne Cloud PBX nutzen Sie für CTI eine externe Software - einen **CTI-Client**.


#### Voraussetzungen für den PhoneSuite CTI Client

Es müssen folgende Voraussetzungen erfüllt sein, damit die Installation gemäß u.a. Anleitung erfolgen kann:

Der PC läuft mit einem Windows-Betriebssystem.

Es ist keine systemfremde Firewall (außer Windows) installiert.

Das anzubindende Telefon hat eine statische IP-Adresse. Diese wird in der CTI-Software eingetragen.
<br>
<br>
#### Installation des PhoneSuite CTI Clients

[1] Download des Clients von der Website des Herstellers: https://www.phonesuite.de/de/download.htm.<br>
<br>
[2]	Führen Sie Setup.exe aus.<br>
<br>
[3]	Folgen Sie dem Installationsprozess und wählen Sie die korrekte Lizenzversion (hier: Professional).<br>
<br>
[4]	Installieren Sie nach Bedarf "ActiveX", "Outlook" und "CTI Client TAPI Connector".<br>
<br>
![phonesuite Installation](https://user-images.githubusercontent.com/98753538/154282695-07121521-4dd6-45c2-a66a-0c0502c30c1c.jpg)<br>
<br>
[5]	Klicken Sie auf "Weiter" und führen Sie die Installation zu Ende.<br>
<br>
[6] Starten Sie "Phone Suite CTI Client" über das Windows-Startmenü.<br>
<br>
![phoneSuite_Start](https://user-images.githubusercontent.com/98753538/154282861-d6c26fca-6760-466a-80b2-62cbbe989b77.jpg)<br>
<br>
<br>
#### Einrichtung des PhoneSuite CTI Clients

[7]	Klicken Sie im Menü "Optionen" auf den Punkt "PhoneDialog (TAPI-Gerät)".<br>
<br>
![phoneSuite Einrichtung1](https://user-images.githubusercontent.com/98753538/154283706-a1b91ce8-7d6f-4d88-858a-0e2fa3136c0b.jpg)<br>
<br>
[8]	Klicken Sie im sich daraufhin öffnenden Fenster auf "TAPI-Gerät auswählen".<br>
<br>
![phoneSuite Tapi auswählen2](https://user-images.githubusercontent.com/98753538/154433643-5d54e0d4-9b00-4c75-9d9d-e423084263ca.jpg)<br>
<br>
[9]	Wählen Sie aus der Auswahl "snom Phones" oder "Yealink Phones" aus.<br>
<br>
![phoneSuite Yeahlink auswählen2](https://user-images.githubusercontent.com/98753538/154433861-b458ac1a-1895-44e4-98e2-d69002f91e7b.jpg)<br>
<br>
[10] und klicken auf "Geräte-Konfiguration".<br>
<br>
![phoneSuite Line_Konfiguration](https://user-images.githubusercontent.com/98753538/154434987-be3f84eb-97f4-46fb-acae-ec35c9faee2f.jpg)<br>
<br>
[11]	Geben Sie nun die IP-Adresse des anzubindenden Telefons ein.<br>
<br>
[12]	Tragen Sie den gewünschten Nutzernamen für die Admin-Oberfläche des Telefons ein, z.B. "admin".<br>
<br>
[13]	Das Passwort lautet im Auslieferungszustand ebenfalls "admin". Bei über die Cloud-PBX-GUI provisionierten Geräten lautet es "adminpass". Oder verwenden Sie das von Ihnen gesetzte Passwort (siehe Provisionierung Endgeräte).<br>
💡 **Hinweis:** Bei Anlagen, die von NetCologne eingerichtet wurden, werden aus Sicherheitsgründen keine Standardpasswörter verwendet. Sollten Sie das Administrator-Kennwort benötigen, wenden Sie sich bitte an den Geschäftskunden-Support.
<br>
[14]	Nach erfolgter Eingabe klicken Sie auf "Test". Sind alle Eingaben korrekt, so erscheint hier "OK".<br>
<br>
#### Konfiguration der Firewall

![phoneSuite Line_Konfiguration2a](https://user-images.githubusercontent.com/98753538/154460088-29a61e4e-4fc0-43c3-8717-06f501696c48.jpg)<br>
<br>
[15]	Klicken Sie auf den Reiter "Aktions-URL" und stellen Sie sicher, dass der Haken bei "Anruf-Ereignisse vom Telefon empfangen" gesetzt ist.<br>
<br>
[16]	Wählen Sie im Dropdown-Menü die lokale IP-Adresse Ihres Computers aus. Sollte eine IP-Adresse mit der Nummer 169.XXX.XXX.XXX angezeigt werden, so ignorieren Sie dies.<br>
<br>
[17]	Klicken Sie anschließend auf "Start". Damit ändert sich der Status von "Inaktiv" auf "Aktiv".<br>
<br>
![phoneSuite LineKonfiguration3](https://user-images.githubusercontent.com/98753538/154460446-9533fc06-1d2a-42d5-a8f7-496151eddcbe.jpg)<br>
<br>
[18]	Klicken Sie sodann auf "Windows-Firewall konfigurieren". Damit wird der TCP-Port 8080 an Ihrem PC für eingehenden Datenverkehr freigeschaltet.<br>
<br>
![phoneSuite Firewall](https://user-images.githubusercontent.com/98753538/154444715-e295431d-eef7-4f94-8ccc-9f18c3a822a4.jpg)<br>
<br>
[19]	Wählen Sie nun "Windows-Firewall jetzt automatisch konfigurieren".<br>
<br>
[20]	Klicken Sie auf "Test-URL im Browser öffnen".<br>
<br>
[21]	Ihr Webbrowser öffnet sich nun mit der Meldung <TAPI>Receive OK</TAPI>:<br>
<br>
![phoneSuite TAPI Receive](https://user-images.githubusercontent.com/98753538/154444915-bce5fcb5-9f13-4d4a-b0fd-ce756f3dc5f9.jpg)<br>
<br>
Sollte dies nicht der Fall sein, so wiederholen Sie bitte die Schritte 16 bis 21 und überprüfen Sie Ihre Firewall-Einstellungen.<br>
<br>
[22]	Klicken Sie bei der Abfrage auf "OK".<br>
<br>
![phoneSuite TAPI Receive2](https://user-images.githubusercontent.com/98753538/154444938-b8e69021-c3e2-49bc-ae31-b72b9eec8b61.jpg)<br>
<br>
[23]	Schließen Sie das Einstellungs-Fenster mit einem Klick auf "OK".<br>
<br>
#### Verknüpfung des Telefons

![phoneSuite Einrichtung1](https://user-images.githubusercontent.com/98753538/154445924-0a437dfa-8bc6-46c8-899f-f1abd6e4ab34.jpg)<br>
<br>
[24]	Wählen Sie im Menü "Optionen" nun "PhoneDialog (TAPI-Gerät)" aus.<br>
<br>
![phoneSuite PhoneDialog2](https://user-images.githubusercontent.com/98753538/154446298-f5f215c4-9435-4e3a-b39d-4e96c4390765.jpg)<br>
<br>
[25]	Klicken Sie auf "Wähleinstellungen" für das betreffende TAPI-Gerät.<br>
<br>
[26]	Wählen Sie den Reiter "Telefonanlage".<br>
<br>
[27]	Je nachdem, ob eine Amtsholung erforderlich ist, setzen Sie den Haken bei "Amtskennziffer" und geben die entsprechende Ziffer(n) ein, z.B. "0"<br>
<br>
<![phoneSuite Wähleinstellungen2](https://user-images.githubusercontent.com/98753538/154468450-8c325c65-afeb-4758-b998-c570f841ee3f.jpg)<br>
<br>
[28]	Klicken Sie abschließend auf "OK".<br>
<br>
Ihr Phone Suite CTI Client ist nun mit Ihrem Telefon verbunden. Eingehende Anrufe werden im CTI-Client signalisiert, ausgehende Anrufe werden über den CTI-Client vom IP-Telefon ausgeführt. Eventuell müssen Sie bei der Konfiguration am Telefon eine Abfrage "Remote Zugriff zulassen" bestätigen.
Rufnummern können in der Standardeinstellung aus jedem Windows-Programm systemweit (nach Aktivierung mit der Maus) mit dem Hotkey "Pause" nahe des Ziffernblocks jeder Tastatur gewählt werden. Für weitere Informationen konsultieren Sie bitte die Dokumentation des Herstellers des PhoneSuite CTI Client.
