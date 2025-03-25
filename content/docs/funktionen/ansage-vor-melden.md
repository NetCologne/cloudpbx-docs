---
title: "Ansage vor Melden (RingBackTone)"
date: 2024-01-31T15:57:00+01:00
menu:
  docs:
    parent: "funktionen"
weight: 415
toc: true
---

„Ansage vor Melden“ oder individueller Freizeichenton (RingBackTone)

Um in der Cloud-PBX eine „Ansage vor Melden“ zu realisieren, wird der individuelle Freizeichenton (RingBackTone) verwendet.

Wenn eine „Ansage vor Melden“ oder ein individueller RingBackTone gewünscht ist, muss im ersten Schritt das Feature für die Nebenstelle oder die Gruppe aktiviert werden. Dies geschieht per Schiebeschalter unter „PBX-Konfiguration -> Kundenpräferenzen:

![image](https://github.com/user-attachments/assets/6e1a2fc4-c2e0-4dea-9c89-3672cd35b9b8)

Anschließend muss das Soundset konfiguriert werden („PBX- Konfiguration -> Sound Sets -> early media“). Hier muss „announce_before_call_setup“ und der „ringback_tone“ konfiguriert werden. Für beide Ansagen muss eine Audio-Datei bereitgestellt werden, selbst wenn keine Ansage vor Melden gewünscht ist (dann muss hier eine Datei mit 1 Sekunde Stille geladen werden) oder nach der Ansage vor Melden der Standard Ringbacktone gewünscht ist (dann muss hier eine Audio-Datei mit dem Standard Ringbacktone eingespielt werden).

![PBX_Sound-Sets](https://github.com/NetCologne/cloudpbx-docs/assets/99875470/312a5385-a9ce-407c-9454-38c19dca1e40)

In diesem Beispiel wird bei Anruf auf die Zentrale vor Setup eine Sekunde Stille (Stille.wav) eingefügt und danach ein individueller RingBackTone, bestehend aus einer Ansage und einem darunter liegenden leisen Standard RBT (Ansage_RBT_leise.wav) gespielt.

Zum Erstellen und Schneiden eigener Ansagen kann die kostenlose Software „audacity“ (https://www.audacity.de/) verwendet werden.

Beachten Sie auf jeden Fall die rechtlichen Voraussetzungen (z.B. Urheber- bzw. Nutzungsrechte, Lizenzen usw.) bei der Verwendung von rechtlich geschützten Werken.
