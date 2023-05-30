---
title: "Audio-Probleme"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "problemloesungen"
weight: 601
toc: true
---

Die Geschwindigkeit Ihres Internetanschlusses ist der Haupteinflussfaktor für die Qualität der übertragenen Sprache. Jedes aktuell geführte Telefonat besetzt 80-100 kBit/s, sowohl im Up- als auch im Downstream. 5 telefonierende Nutzer brauchen also allein für das Telefonieren eine Bandbreite von 0,5 MBit/s, sowohl im Up- als auch im Downstream. Zusätzlich brauchen andere Anwendungen wie die Internetnutzung oder E-Mails weiteres Datenvolumen.

Falls Sie den Grund suchen, warum die Audio-Qualität Ihrer Verbindung zu wünschen übrig lässt, verbinden Sie Ihr Telefon direkt mit dem Router. Starten Sie nun beide Geräte neu, Router und Telefon. 

Ist die Sprachqualität immer noch beeinträchtigt, sollten Sie die Geschwindigkeit Ihrer Internetverbindung prüfen. Schnell und einfach geht das unter http://speedtest.netcologne.de/. Die Website setzt einen "Ping" ab und testet, wie schnell Ihre Internetverbindung antwortet. Je schneller, desto besser. Führen Sie diesen Test einmal durch, während Sie telefonieren und einmal, wenn Sie nicht telefonieren.

Haben Sie dann immer noch keine zufriedenstellende Audio-Qualität, hilft Ihnen unser Support-Team gern weiter. Halten Sie für dieses Gespräch bitte folgende Daten bereit und seien Sie so präzise, wie es geht:

Datum und Uhrzeit des Anrufs
Angerufene Rufnummer
Anrufende Rufnummer

Bitte seien Sie dabei so konkret wie möglich. Außerdem kann ein PCAP Trace erstellt werden, um die Behebung des Fehlers zu erleichtern. Dieses kann ebenfalls dem Support Ticket in Form einer Datei angehängt werden.

Achtung: Auch wenn Sie mit einem Gesprächspartner im Mobilfunknetz sprechen, kann die Audio-Qualität schlechter ausfallen. Dies kann zum Beispiel am Empfang des Telefonierenden liegen.

## One-Way-Audio

Es kann passieren, dass Ihr Gesprächspartner Sie hören kann, Sie ihn aber nicht. Das nennt man One-Way-Audio. Tun Sie bitte folgendes:

1. Prüfen Sie die typischen Fehlerquellen wie fehlende Stromversorgung, wackelnder Headset-Anschluss oder fehlende Internetverbindung. Starten Sie unter Umständen die Geräte neu, wie das geht, zeigt Ihnen die Anleitung des Geräts. 

2. Prüfen Sie, ob die Firmware aktuell ist, sowohl beim Endgerät als auch beim Router. Fahren Sie ein Update, wenn es nicht so ist. Im Handbuch Ihres Geräts finden Sie die Vorgehensweise.

3. Prüfen Sie Ihr NetCologne Cloud PBX Konto. Sie melden sich an und navigieren über das linke Menü zu "Telefonanlage". Dann gehen Sie zu "Ziele". Sehen Sie in der Liste der IP-Endgeräte nach, ob das Telefon "Online" ist. Ist es "Offline" kann es sein, dass Ihr Telefon falsch eingerichtet wurde oder die NetCologne Cloud PBX aktuelle Verbindungsprobleme hat. 

4. Auf der Startseite von der NetCologne Hilfe, können Sie sehen, ob es sich um eine Störung der NetCologne Cloud PBX handelt. Sehen Sie hier die Störungsmeldung, dauert es nicht mehr lang, bis wir die Störung behoben haben.  

5. Sehen Sie den "System Status: Online", handelt es sich nicht um eine Störung der virtuellen Telefonanlage. Möglicherweise wurde dann Ihr IP-Gerät falsch eingerichtet. Haben Sie eines der im NetCologne Online Shop erhältlichen Telefone, können Sie es ganz einfach erneut konfigurieren. Klicken Sie dazu auf das "Bearbeiten" Ihres Telefons in der "Ziele"-Liste. Setzen Sie dann ein Häkchen bei "Vollautomatische Konfiguration aktivieren (empfohlen)". Sobald Sie gespeichert haben, konfiguriert sich Ihr Telefon komplett automatisch. Falls die Audio-Probleme dann immer noch bestehen, hilft Ihnen unser Support-Team weiter.

6. Ist das IP-Telefon nicht über den NetCologne Online Shop erhältlich, prüfen Sie bitte die Einstellungen des IP-Telefons. Lesen Sie dazu bitte den Artikel zur manuellen Konfiguration und überprüfen Sie, ob alles korrekt eingestellt wurde. Über die Navigation finden Sie die Hilfestellung zur manuellen Konfiguration einiger Anbieter. Falls Ihr Hersteller nicht dabei ist, schauen Sie bitte in die Bedienungsanleitung Ihres Geräts. 

7. Auch Port-Weiterleitungen können die Audio-Qualität verbessern. Hiermit können Sie Telefonate manuell direkt auf das Telefon weiterstellen. 

## Verzögertes Audio-Signal

Manchmal kommt es dazu, dass ein Audiosignal zeitversetzt ausgegeben wird und die Gesprächspartner sich asynchron hören. Unternehmen Sie in diesem Fall folgende Schritte.

1. Schließen Sie Ihr Telefon direkt an den Router an und prüfen Sie die Audio-Qualität, indem Sie telefonieren. 

2. Falls Sie auch bei direkter Verbindung die Asynchronität hören, starten Sie Ihren Switch neu. Haben Sie keinen Switch installiert oder das Problem besteht auch nach dem Neustart weiter, richten Sie eine Port-Weiterleitung ein.

3. Steht die Port-Weiterleitung, führen Sie einen Neustart bei Router und Telefon durch. 

4. Falls das Problem immer noch besteht, kann ein Test von Router und Telefon in einem anderen Netzwerk Aufschluss bringen. Auch die Nachfrage bei Ihrem Internet-Provider kann die Lösung bringen oder ein neuer Router. 

5. Falls auch jetzt das Problem noch besteht, hilft Ihnen unser Support sicher weiter. 
