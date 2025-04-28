---
title: "Ansage vor Melden (RingBackTone)"
date: 2024-01-31T15:57:00+01:00
menu:
  docs:
    parent: "funktionen"
weight: 415
toc: true
---

„Ansage vor Melden“ und/oder individueller Klingelton (RingBackTone)

Um dem Anrufer die Wartezeit bis zum Durchschalten zu verkürzen, kann in der Cloud-PBX eine *Ansage vor Melden* und/oder ein *individueller Klingelton (RingBackTone)* gespielt werden. 
Ist dies gewünscht, muss der **Administrator** zunächst diese Features für die Nebenstelle oder Gruppe aktivieren. Dies geschieht per Schiebeschalter unter „PBX-Konfiguration -> Kundenpräferenzen:

![image](https://github.com/user-attachments/assets/6e1a2fc4-c2e0-4dea-9c89-3672cd35b9b8)

Anschließend **muss** das Soundset konfiguriert werden („PBX- Konfiguration -> Sound Sets -> early media“). Hier werden die

* „announce_before_call_setup“ und der
* „ringback_tone“ benötigt. <br>
Für beide Ansagen muss eine Audio-Datei bereitgestellt werden. Auch wenn keine Ansage vor Melden gewünscht ist, dann muss hier eine Datei mit 1 Sekunde Stille geladen werden.
Gleiches gilt beim Klingelton: Ist der Standard-Ringbacktone gewünscht, dann muss hier eine Audio-Datei mit dem Standard Ringbacktone eingespielt werden. <br>

❗Fehlt die Audio-Datei und die Ansagen-Funktion ist aktiviert, kommt es zum Callabbruch.❗

![PBX_Sound-Sets_neu](https://github.com/user-attachments/assets/189de5c4-a05c-4912-b17f-89370a922e0f)

In diesem Beispiel wird bei Anruf auf die Zentrale vor Setup die Ansage "bitte_haben_sie_ein_wenig_geduld_mit_musik.wav" eingefügt und danach ein individueller RingBack-Ton (queue_waiting_music.wav) gespielt.

Zum Erstellen und Schneiden eigener Ansagen kann die kostenlose Software „audacity“ (https://www.audacity.de/) verwendet werden.

Beachten Sie auf jeden Fall die rechtlichen Voraussetzungen (z.B. Urheber- bzw. Nutzungsrechte, Lizenzen usw.) bei der Verwendung von rechtlich geschützten Werken.
