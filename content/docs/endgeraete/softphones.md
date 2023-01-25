---
title: "Softphones"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "endgeraete"
weight: 509
toc: true
---

## Android
### Linphone

<img src="https://user-images.githubusercontent.com/20154956/150996682-d127c94f-254a-4f78-ac10-1998d8009568.png" height="600" />
<img src="https://user-images.githubusercontent.com/20154956/150996721-180fcd0b-4120-416c-b44d-5435efb54aac.png" height="600" />

### Baresip+

<img src="https://user-images.githubusercontent.com/20154956/150996920-9714b70d-155a-45ad-bcbc-34ade9088ee9.png" height="600" />
<img src="https://user-images.githubusercontent.com/20154956/150996947-1ea0706d-8f0e-4eca-b790-327d0fde5117.png" height="600" />
<img src="https://user-images.githubusercontent.com/20154956/150997101-0a1e0205-e5a5-472d-8cb2-20cc310af44d.png" height="600" />
<img src="https://user-images.githubusercontent.com/20154956/150997140-7c5ac868-1a08-40d6-8d72-2ae8b4937e28.png" height="600" />
<img src="https://user-images.githubusercontent.com/20154956/150997165-d75bf8b7-51d5-45fa-9ff2-f03a14fc0814.png" height="600" />
<img src="https://user-images.githubusercontent.com/20154956/151002026-9be885c1-ae89-4748-9d82-eedbfcc098f7.png" height="600" />
<img src="https://user-images.githubusercontent.com/20154956/150997308-df31152a-dc9e-476e-b4e2-8bf93c03fa71.png" height="600" />


## IOS
### WaveLite
<img src="https://user-images.githubusercontent.com/20154956/151133026-6a8624de-6298-4895-91c9-198f0462fcf9.png" height="600" />
<img src="https://user-images.githubusercontent.com/20154956/151133047-6cceed1a-f045-42cf-8040-3c66e16880d4.png" height="600" />
<img src="https://user-images.githubusercontent.com/20154956/151133065-d290afc9-61b1-451e-a0e6-c0955976d5f0.png" height="600" />
<img src="https://user-images.githubusercontent.com/20154956/151133082-3f5853a1-19d0-4792-861f-e6d16cc485f5.png" height="600" />
<img src="https://user-images.githubusercontent.com/20154956/151133110-3e8ab119-612d-4a5f-bb12-604cedf54a2b.png" height="600" />
<img src="https://user-images.githubusercontent.com/20154956/151133142-b4a73e8e-7260-43a7-b9f5-b755cd398434.png" height="600" />
<img src="https://user-images.githubusercontent.com/20154956/151133171-85ef0dd0-26cd-4174-bb28-639bc6d25a05.png" height="600" />


## Windows
### PhonerLite

Installation des Softclients unter http://phonerlite.de/download_de.htm. 

#### Konfiguration

Zur Konfiguration wird im Reiter "Server" in den Feldern Proxy/Registrar und Domain/Realm der Servername eingetragen. Für die Registrieung ist ein Häkchen zu setzen - 3.600 Sekunden sind ein plausibler Wert. Das Häkchen beim message-waiting indicator (MWI) ist optional:
![PhoneLite Konfiguration Server](https://user-images.githubusercontent.com/98753538/153848572-20e621de-3bd6-49a9-8b27-91cfaa74f07c.jpg)
<br>
<br>  
Im Reiter "Benutzer" werden Benutzername, Angezeigter Name, Authentifizierungsname und zur Bestätigung das SIP-Kennwort eingetragen:
![PhoneLite Konfiguration Benutzer](https://user-images.githubusercontent.com/98753538/153848487-ffd54614-be89-4a5e-a1bb-7d88b315be46.jpg)
<br>
<br>  
Um die Inhalte zu schützen bzw. sicher zu verschlüsseln, wird im Reiter "Netzwerk" TLS als bevorzugte Verbindungsart ausgewählt. Der Lokale Port lautet 5061:
![PhoneLite Konfiguration Netzwerk](https://user-images.githubusercontent.com/98753538/153848648-7e632f41-637a-4e9e-9981-62e29ab2c0cd.jpg)
<br>
<br>  
Im Reiter muss der Codec "G.711 A-Law" ausgewählt werden. Weitere Codecs sind optional. Wichtig auch die Häkchen bei SRTP und SAVP:
![PhoneLite Konfiguration Codecs](https://user-images.githubusercontent.com/98753538/153848681-538cc078-55c7-4d99-a235-6ea1dedfa2ad.jpg)
<br>
<br>  
Abschließend speichert man das Profil mit Angabe eines Namens
![PhoneLite Konfiguration Speichern](https://user-images.githubusercontent.com/98753538/153848898-3573ac86-51c3-46d6-8db3-87855a3fd115.jpg)
<br>
<br>  
und erhält in der unteren Statusleiste eine Bestätigung der Registrierung:
![PhoneLite Konfiguration Registrierung](https://user-images.githubusercontent.com/98753538/153848918-f7d61a80-3fb9-4fdf-a09f-fc252ebfb171.jpg)
<br>
<br>  
#### Telefonbuch

PhonerLite bietet die Möglichkeit ein Telefonbuch anzulegen:
![PhoneLite Konfiguration Telefonbuch](https://user-images.githubusercontent.com/98753538/153849003-47444112-b522-4fb7-8d51-908cb3d2ed61.jpg)
<br>
<br>  
Im Menue "Optionen" können die Kurzwahltasten angewählt werden:
![PhoneLite Konfiguration Kurzwahl](https://user-images.githubusercontent.com/98753538/153849019-0e5857be-3c33-44a8-92c6-b6fffb33f279.jpg)
<br>
<br>  
Zur Belegung zieht man den gewünschten Telefonbuch-Eintrag einfach auf das Kurzwahl-Feld:
![PhoneLite Konfiguration Kurz Kollege](https://user-images.githubusercontent.com/98753538/153849040-d45cd9ec-cdd1-4644-aba0-667edcf25be6.jpg)


### Zoiper

Für die Verwendung mit der Cloud PBX ist die kostenpflichtige Version erforderlich, da nur diese die notwendige Verschlüsselung mit TLS und SRTP unterstützt.

Die aktuelle Version laden Sie am besten direkt vom Hersteller herunter: https://www.zoiper.com/en/voip-softphone/download/current
Zur Installation des Clients folgen Sie der Anleitung des Herstellers.

#### Konfiguration

Die folgende Beschreibung führt Sie durch die grundlegende Konfiguration für die Cloud PBX. Nach dem Start des Clients erscheint zunächst ein Fenster mit leeren Feldern für die Anmeldedaten. Dort werden die Anmeldedaten für den Subscriber eingetragen. Exemplarisch wird hier der Subscriber "mulheim" in der Domäne firmaid.cloudpbx.netcologne.de verwendet.

<img width="622" alt="02_Cloud-PBX_Start" src="https://user-images.githubusercontent.com/99875470/214311476-0834c659-fe79-4994-a26c-159af36de675.png">

Username/Login: mulheim
Passwort: Hier wird das Passwort des SIP-Benutzers eingetragen.

Im folgenden Fenster wird als Hostname die URL der Cloud PBX eingetragen: firmaid.cloudpbx.netcologne.de

<img width="683" alt="03_Cloud-PBX_Hostname" src="https://user-images.githubusercontent.com/99875470/214313961-c9fffa2d-0878-43f3-bf0e-d8b40ee59409.png">

Auf der nächsten Seite muss das Häkchen für optionale Angaben gesetzt werden und Angaben zur Authentifizierung und zum outbound proxy eingetragen werden.

Authentication username: mulheim@firmaid.cloudpbx.netcologne.de
Outbound proxy: firmaid.cloudpbx.netcologne.de

<img width="680" alt="05_Cloud-PBX_Authentication_Out-Proxy" src="https://user-images.githubusercontent.com/99875470/214316599-2a7ab341-70a5-44a2-ac68-05088a6129af.png">

Im nächsten Schritt erkennt der SIP Client automatisch die Verschlüsselung über TLS.

<img width="659" alt="06_Cloud-PBX_SIP-TLS" src="https://user-images.githubusercontent.com/99875470/214319317-e9cf571f-9ce4-4377-b64d-852fb9049076.png">

Diese Seite muss mit klicken auf "Next" bestätigt werden.

Die Grundeinstellungen wurden nun vorgenommen. Allerdings müssen noch ein paar Details angepasst werden.

Durch Auswahl des neu angelegten Accounts erreichen Sie die Seite für die Einstellungen.

<img width="628" alt="08_Cloud-PBX_Feinheiten_nachjustieren" src="https://user-images.githubusercontent.com/99875470/214320947-ddb794b4-c8b3-4284-9b5e-75e33550e442.png">

Oben rechts schalten Sie mit "advanced" die erweiterten Einstellungen frei.

<img width="627" alt="09_Cloud-PBX_Advanced" src="https://user-images.githubusercontent.com/99875470/214321755-e34b55a0-3664-4b6d-89d3-4e6b92b7d36f.png">

Im Abschnitt "Features" werden die gewünschten Leitungsmerkmale angehakt.

<img width="550" alt="10_Cloud-PBX_Features" src="https://user-images.githubusercontent.com/99875470/214569579-c4e7f8f4-1db0-4610-9b38-fa8987aed09e.png">

"Register on startup" sorgt dafür, dass sich der Client sofort beim Starten an der Cloud PBX registriert. Erst mit der Registrierung sind Gespräche möglich.

"Subscribe presence" muss aktiviert werden, wenn Sie den Status anderer Teilnehmer der Cloud PBX in Ihrem Client angezeigt bekommen wollen. Voraussetzung dafür ist, dass die anderen Teilnehmer ihren Status veröffentlichen (publish presence). Der Status der anderen Teilnehmer wird im Telefonbuch angezeigt (siehe Abschnitt "Telefonbuch").

"Publish presence" muss aktiviert werden, wenn Sie Ihren Status in der Cloud PBX bekannt geben wollen.

"Use BLF" muss aktiviert sein, damit der Status eines Teilnehmers in der Cloud in Ihrem Telefonbuch angezeigt wird (siehe auch Abschnitt "Telefonbuch").

Unter "Number Rewriting" sorgt der Haken bei "Strip dial chars" dafür, dass die aufgeführten Sonderzeichen vor dem Wählen der Rufnummer entfernt werden. Das ist u.a. wichtig, wenn Sie im Telefonbuch diese Sonderzeichen im Rufnummernfeld verwenden.

<img width="438" alt="11_Cloud-PBX_number_rewriting" src="https://user-images.githubusercontent.com/99875470/214571826-35e7cba6-9fbb-4039-83cc-1f9309b76589.png">

In den Einstellungen für "Pre-configured Extensions" wird im Feld "Check voicemail" 2000 eingetragen. Damit wird das Brief-Symbol in der Benutzeroberfläche so eingestellt, dass mit einem Klick darauf der interne Anrufbeantworter abgefragt werden kann.

Bei den "Compatibility modes" werden vornehmlich die Einstellungen für DTMF vorgenommen.

"DTMF mode": Use DTMF RFC-2833

"Send KPML (Cisco Unified Communications Manager)" muss aktiviert sein, damit bei der Abfrage des interenen Anrufbeantworters die Ziffern (DTMF) richtig übertragen werden. Andernfalls ist eine Navigation im Anrufbeantworter nicht möglich.

<img width="431" alt="12_Cloud-PBX_pre-conf-ext_compat-modes" src="https://user-images.githubusercontent.com/99875470/214579241-84d6f555-0399-4017-a4b9-c76e428a0fb9.png">

