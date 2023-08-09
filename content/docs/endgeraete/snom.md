---
title: "Snom"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "endgeraete"
weight: 501
toc: true
---

Um Ihnen Bedienung und Einrichtung zu erleichtern zeigen wir Ihnen nun die Tastenbelegung und erklären wichtige Funktionen. Die Schritt-für-Schritt-Anleitung zur Konfiguration erhalten Sie außerdem. Unsere Empfehlung: Befindet sich Ihr snom-Modell im NetCologne Shop, haben Sie die Möglichkeit, Ihr Gerät automatisch zu konfigurieren. (außer bei DECT-Geräten)


## Tastenbelegung

Für die leichtere Bedienung ist es gut zu wissen, wie die Tastenbelegung eingestellt ist.

Manche snom Geräte haben andere oder mehr Funktionstasten als andere. Fehlt an Ihrem Gerät eine Funktionstaste, zum Beispiel die Halten-Taste, können Sie die kontextsensitiven Display-Tasten nutzen. Lesen Sie mehr dazu unter Funktionen.

## Snom D865 - IP-Tischtelefon 

Schließen Sie zuallererst Ihr Snom D865 IP-Tischtelefon am Stromnetz und an Ihr Netzwerk an.

Empfehlung: Sie haben die Möglichkeit, Ihr Snom D865 IP-Tischtelefon automatisch über das NetCologne 
Cloud PBX einzurichten. Lesen Sie dazu die Hilfe Automatische Konfiguration.

Hier wird beschrieben, wie Sie das Gerät manuell einrichten können.

### Zugangsdaten

Der Zugriff auf das WebInterface erfolgt über einen Web Browser mit http://IPAdresse, 
wobei die IP Adresse im lokalen Router ausgelesen werden kann:


![Snom_D865_01](https://github.com/NetCologne/cloudpbx-docs/assets/99875491/f94d6776-dd08-4d0e-b53e-c15842eaa1c0)

In der gegenwärtigen Version (v2022 12.0 ) lassen Sie bitte die Felder für Username und Password FREI.

### Konfiguration


![Snom_D865_05](https://github.com/NetCologne/cloudpbx-docs/assets/99875491/4553f0bf-8a1b-417f-b470-8116dfb684c9)


Begeben Sie sich zu dem Menüpunkt “Identities / + Add Identity”. 

Unter "Account" tragen Sie bitte Ihren SIP-User-Account ein und unter "Password" Ihr SIP-Password.
Unter Registrar tragen Sie bitte "firmaid.cloudpbx.netcologne.de" ein.
Unter Outbound Proxy tragen Sie bitte "firmaid.cloudpbx.netcologne.de;transport=tls" ein
Die anderen Parameter bleiben auf den voreingestellten Default-Werten.


![Snom_D865_07](https://github.com/NetCologne/cloudpbx-docs/assets/99875491/dc0e0390-3a10-482d-9302-2ae450673a51)


Wählen Sie den Menuepunkt "RTP" aus und stellen Sie sicher, dass der 
Parameter "RTP Encryption" auf ON steht und dass unter RTP/SAVP "mandatory" ausgewählt ist.
