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

### Zugangsdaten ( Variante 1 )

Der Zugriff auf das WebInterface erfolgt über einen Web Browser mit http://IPAdresse, 
wobei die IP Adresse im lokalen Router ausgelesen werden kann:


![Snom_D865_01](https://github.com/NetCologne/cloudpbx-docs/assets/99875491/f94d6776-dd08-4d0e-b53e-c15842eaa1c0)

In der gegenwärtigen Version (v2022 12.0 ) lassen Sie bitte die Felder für Username und Password FREI.

### Konfiguration


![Snom_D865_05](https://github.com/NetCologne/cloudpbx-docs/assets/99875491/4553f0bf-8a1b-417f-b470-8116dfb684c9)


Begeben Sie sich zu dem Menüpunkt “Identities / + Add Identity”. 

Unter "Account" tragen Sie bitte Ihren SIP-User-Account ein und unter "Password" Ihr SIP-Password.
Unter Registrar tragen Sie bitte die Ihnen von NetCologne mitgeteilten Daten für Registrar ein.
Unter Outbound Proxy tragen Sie bitte ebenfalls die Ihnen von NetCologne mitgeteilten Daten für Registrar ein
mit der Erweiterung ";transport=tls"
Die anderen Parameter bleiben auf den voreingestellten Default-Werten.



![Snom_D865_07](https://github.com/NetCologne/cloudpbx-docs/assets/99875491/dc0e0390-3a10-482d-9302-2ae450673a51)



Wählen Sie den Menuepunkt "RTP" aus und stellen Sie sicher, dass der 
Parameter "RTP Encryption" auf ON steht und dass unter RTP/SAVP "mandatory" ausgewählt ist.

### Zugangsdaten ( Variante 2 )

Der Zugriff auf das WebInterface erfolgt über einen Web Browser mit http://IPAdresse:3112 ( also mit Portangabe ) 
wobei die IP Adresse im lokalen Router ausgelesen werden kann:<br>
<br>
Username : admin und Password : adminpass. <br>
<br>
💡**Hinweis:** Bei Anlagen, die von NetCologne eingerichtet wurden, werden aus Sicherheitsgründen keine Standardpasswörter verwendet. Sollten Sie das Administrator-Kennwort benötigen, wenden Sie sich bitte an den Geschäftskunden-Support.<br>
<br>
<br>
### Konfiguration

![Snom_D865_01_Port_3112_Identity](https://github.com/NetCologne/cloudpbx-docs/assets/99875491/cb13acdd-8903-4d79-b2eb-23f61762b4c3)


Begeben Sie sich zu dem Menüpunkt “Setup/Identity 1 ". 

Unter "Account" tragen Sie bitte Ihren SIP-User-Account ein und unter "Password" Ihr SIP-Password.
Unter Registrar tragen Sie bitte die Ihnen von NetCologne mitgeteilten Daten für Registrar ein.
Unter Outbound Proxy tragen Sie bitte ebenfalls die Ihnen von NetCologne mitgeteilten Daten für Registrar ein
mit der Erweiterung ";transport=tls"
Die anderen Parameter bleiben auf den voreingestellten Default-Werten.

![Snom_D865_02_Port_3112_SRTP](https://github.com/NetCologne/cloudpbx-docs/assets/99875491/46e456f7-e400-4df4-93e6-ecfe3a6d2796)

Wählen Sie den TAB "RTP" aus und stellen Sie sicher, dass der 
Parameter "RTP Encryption" auf ON steht und dass unter RTP/SAVP "mandatory" ausgewählt ist.

