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

Gehen Sie zuerst in das Menü "Identitäten". Dort werden die grundlegenden Einstellungen für den SIP-Benutzer vorgenommen. Öffnen Sie einen leeren Eintrag. Die folgende Darstellung zeigt eine bereits ausgefüllte Maske.

![image](https://user-images.githubusercontent.com/99875470/207901188-187f7b32-d5f5-4069-b142-9def68cdc51c.png)

SIP-Benutzername: Hier wird der in der Cloud PBX für diesen Benutzer eingerichtete Name eingetragen.
Passwort: Das Passwort des SIP-Benutzers wird hier eingetragen.
Displayname: Zur Anzeige im Telefon kann hier ein beliebiger Name eingetragen werden.
Authentifizierungsname: Der Authentifizierungsname besteht aus dem SIP-Benutzernamen und der Domäne der Cloud PBX.
SIP-Registrar: Als Registrar wird die Domäne der Cloud PBX eingetragen.
Klingelton: Aus dem Drop-Down-Menü kann der gewünschte Klingelton ausgewählt werden.

Schalten Sie nun auf den Reiter "Erweiterte Einstellungen" um.

![image](https://user-images.githubusercontent.com/99875470/207905502-3b9e4840-84c8-402d-98e9-584a11874e0a.png)

Fallback für: Dieser SIP-Benutzer kann als Fallback für einen anderen vorhandenen Benutzer verwendet werden. Details siehe Anleitung von Auerswald oder Onlinehilfe.
CLIR-Typ: Anonym
Voicemail-Nummer: 2000 Das ist die interne Rufnummer für den Anrufbeantworter in der Cloud PBX
Pick-Up-Code: \*99 Das ist die Kennziffer, um ein Gespräch heranzuholen. Im Zusammenhang mit einer Funktionstaste können damit Gespräche von einem anderen Telefon herangeholt werden.
Wartemusik: Aktivieren Sie diesen Schalter um beim Halten einer Verbindung Wartemusik einzuspielen.
IP-Version: IPv4
SRTP: Hier muss "Vorgeschrieben" ausgewählt werden, da die Nutzdaten (Sprache) verschlüsselt übertragen werden.
SIPS: Die Verschlüsselung für die Signalisierung muss eingeschaltet sein.

![image](https://user-images.githubusercontent.com/99875470/207912604-adedf2a8-03e1-4042-a54a-7793ca95956d.png)

Zertifikat: Hier muss kein Zertifikat hochgeladen werden, da es automatisch heruntergeladen wird.
Session Timer: einschalten
Session Timeout: 15 min.
Protokolltyp: TCP
Zeitspanne Subscription: 45 min.
Subscriptionversuche: festes Intervall
Subscriptionversuche: Intervall in Sekunden: 180
Registerversuche: festes Intervall
Registerversuche: Intervall in Sekunden: 10
