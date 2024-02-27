---
title: "Auerswald"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "endgeraete"
weight: 513
toc: true
---

In diesem Kapitel erhalten Sie eine Anleitung für die manuelle Konfiguration der Endgeräte von Auerswald. Am Beispiel des COMfortel D-400 werden die grundlegenden Einstellungen beschrieben.

Ab Werk ist die Netzwerkschnittstelle auf DHCP eingestellt, sodass das Telefon bei erster Inbetriebnahme unter der von Ihrem Router vergebenen IP-Adresse zu erreichen ist. Die IP-Adresse wird in der Anzeige des Telefons eingeblendet.

Die Konfiguration kann sowohl am Telefon als auch über einen Browser am PC erfolgen. Wir empfehlen die Verwendung eines Browsers, da dieser Weg komfortabler ist.

Über einen Browser greifen Sie mit http://ip-adresse auf die Benutzeroberfläche zu. Ab Werk sind die Anmeldedaten:

Benutzer: admin

Passwort: admin

![image](https://user-images.githubusercontent.com/99875470/207878135-e5b75b49-dd9d-4433-8b58-fc2f25334cc5.png)

Aus Sicherheitsgründen sollten Sie das Passwort auf einen individuellen Wert ändern.

Nach der Anmeldung prüfen Sie zuerst die Firmwareversion. Zur Verwendung mit der NetCologne Cloud PBX ist mindestens Version **2.4B-00004** erforderlich. Im Menüpunkt "Dashboard" werden Informationen u.a. zum Softwarestand angezeigt, hier zum Beispiel 2.6B-00000:

![Dashboard](https://github.com/NetCologne/cloudpbx-docs/assets/99875470/f643f4c7-b823-43e5-b681-dfa055f58a57)

Auf der Homepage von Auerswald finden Sie Informationen über den aktuellen Firmwarestand unter: https://www.auerswald.de/de/support

Vor der eigentlichen Inbetriebnahme sollten Sie das Telefon auf den aktuellen Softwarestand bringen, mindestens auf die o.g. Version 2.4B-00004.

![Update](https://github.com/NetCologne/cloudpbx-docs/assets/99875470/e65b566c-1471-424c-ba57-ec7b33293f61)

Ab Werk ist schon die richtige Adresse des Update-Servers eingetragen: https://update.auerswald.de. Das Update wird dann durch Klicken auf "Update starten" angestoßen. Folgen Sie den Hinweisen auf der Oberfläche.

Nun kann die eigentliche Konfiguration des Telefons beginnen.

Gehen Sie zuerst in das Menü "Netzwerk". Im Reiter "Topologie" muss der Schalter "Hostname prüfen" ausgeschaltet sein.

![Netzwerk_Topologie](https://user-images.githubusercontent.com/99875470/210994671-35aeeb6f-34ff-4a26-9e95-3c622b016cf3.jpg)

Gehen Sie nun in das Menü "Identitäten". Dort werden die grundlegenden Einstellungen für den SIP-Benutzer vorgenommen. Öffnen Sie einen leeren Eintrag. Die folgende Darstellung zeigt eine bereits ausgefüllte Maske.

![image](https://user-images.githubusercontent.com/99875470/207901188-187f7b32-d5f5-4069-b142-9def68cdc51c.png)

SIP-Benutzername: Hier wird der in der Cloud PBX für diesen Benutzer eingerichtete Name eingetragen.

Passwort: Das Passwort des SIP-Benutzers wird hier eingetragen.

Displayname: Zur Anzeige im Telefon kann hier ein beliebiger Name eingetragen werden.

Authentifizierungsname: Der Authentifizierungsname besteht aus dem SIP-Benutzernamen und der Domäne der Cloud PBX.

SIP-Registrar: Als Registrar wird die Domäne der Cloud PBX eingetragen.

Klingelton: Aus dem Drop-Down-Menü kann der gewünschte Klingelton ausgewählt werden.

Schalten Sie nun auf den Reiter "Erweiterte Einstellungen" um.

![Ident_erweiterte_Einstell_1](https://github.com/NetCologne/cloudpbx-docs/assets/99875470/c5a7bb67-dcea-49b4-9df3-4156fb2b78e9)

Fallback für: Dieser SIP-Benutzer kann als Fallback für einen anderen vorhandenen Benutzer verwendet werden. Details siehe Anleitung von Auerswald oder Onlinehilfe.

CLIR-Typ: Anonym

Voicemail-Nummer: 2000 Das ist die interne Rufnummer für den Anrufbeantworter in der Cloud PBX

Pick-Up-Code: \*99\* Das ist die Kennziffer, um ein Gespräch heranzuholen. Im Zusammenhang mit einer Funktionstaste können damit Gespräche von einem anderen Telefon herangeholt werden.

Wartemusik: Aktivieren Sie diesen Schalter, um beim Halten einer Verbindung Wartemusik einzuspielen.

IP-Version: IPv4

SRTP: Hier muss "Vorgeschrieben" ausgewählt werden, da die Nutzdaten (Sprache) verschlüsselt übertragen werden.

SIPS: Die Verschlüsselung für die Signalisierung muss eingeschaltet sein.

![Ident_erweiterte_Einstell_2_ohne_root-cert](https://github.com/NetCologne/cloudpbx-docs/assets/99875470/f8c04820-2291-4ee9-8dc2-2c412d322e51)

Zertifikat: Hier braucht kein Zertifikat hochgeladen werden.

Session Timer: einschalten

Session Timeout: 15 min.

Protokolltyp: TCP

Zeitspanne Subscription: 45 min.

Subscriptionversuche: festes Intervall

Subscriptionversuche: Intervall in Sekunden: 180

Registerversuche: festes Intervall

Registerversuche: Intervall in Sekunden: 10

In dem Reiter "Codecs" werden die zugelassenen Codecs für die Übertragung der Sprache eingestellt.

![image](https://user-images.githubusercontent.com/99875470/208454052-5b221f93-947b-4b10-ae28-97c3d700a91a.png)

Der Codec G.722 wird deaktiviert.

Im Reiter "Registrar" wird die Domain des Registrars sowie der zugehörige Port und die Zeitspanne für die Registrierung eingetragen.

![image](https://user-images.githubusercontent.com/99875470/208465107-dacca2f0-012d-4530-86a7-f525e81c53a6.png)

SIP-Domain: Hier muss die Domain eingetragen werden, die beim Anlegen des Kunden vergeben wurde.

Port: Für die Registrierung über eine verschlüsselte Verbindung muss hier 5061 eingetragen werden.

Zeitspanne Registrierung: Für die Wiederholung der Registrierung wird eine zeitspanne von 30 Minuten empfohlen.

Im Reiter "NAT" sind keine Änderungen erforderlich.

![image](https://user-images.githubusercontent.com/99875470/208473318-c13edbc3-0c80-4e77-aa5a-1a8d02e75d2e.png)

SIP NAT-Traversal und RTP NAT-Taversal bleiben auf "inaktiv" stehen.

ICE-Methode: ICE wird nicht unterstützt und bleibt daher ausgeschaltet.

![image](https://user-images.githubusercontent.com/99875470/208474204-273ca5e8-0899-4ad0-84d3-dd9a37985583.png)

Der Modus für den Outbound Proxy wird auf "automatisch" eingestellt.

Als URL wird die Domain eingetragen, die beim Anlegen des Kunden vergeben wurde.

Port: 5061

Die Felder für alternative URL und Port bleiben leer.

