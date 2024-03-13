---
title: "Ansage vor Melden (RingBackTone)"
date: 2024-01-31T15:57:00+01:00
menu:
  docs:
    parent: "funktionen"
weight: 513
toc: true
---

„Ansage vor Melden“ oder individueller Freizeichenton (RingBackTone)

Um in der Cloud-PBX eine „Ansage vor Melden“ zu realisieren, wird der individuelle Freizeichenton (RingBackTone) verwendet.

Wenn eine „Ansage vor Melden“ oder ein individueller RingBackTone gewünscht ist, muss im ersten Schritt das Feature für die Nebenstelle oder die Gruppe aktiviert werden. Dies geschieht unter „Kunden Details -> Group/Subscriber -> Preferences -> Applications“:

![PBX-Group_Preferences](https://github.com/NetCologne/cloudpbx-docs/assets/99875470/01c87513-b100-4720-b194-1d3b89588a67)

Anschließend muss das Soundset konfiguriert werden („PBX- Konfiguration -> Sound Sets -> early media“). Hier muss „announce_before_call_setup“ und der „ringback_tone“ konfiguriert werden. Für beide Ansagen muss eine Audio-Datei bereitgestellt werden, selbst wenn keine Ansage vor Melden gewünscht ist (dann muss hier eine Datei mit 1 Sekunde Stille geladen werden) oder nach der Ansage vor Melden der Standard Ringbacktone gewünscht ist (dann muss hier eine Audio-Datei mit dem Standard Ringbacktone eingespielt werden).

![PBX_Sound-Sets](https://github.com/NetCologne/cloudpbx-docs/assets/99875470/312a5385-a9ce-407c-9454-38c19dca1e40)

In diesem Beispiel wird bei Anruf auf die Zentrale vor Setup eine Sekunde Stille (Stille.wav) eingefügt und danach ein individueller RingBackTone, bestehend aus einer Ansage und einem darunter liegenden leisen Standard RBT (Ansage_RBT_leise.wav) gespielt.

Zum Erstellen und Schneiden eigener Ansagen kann die kostenlose Software „audacity“ (https://www.audacity.de/) verwendet werden.

Beachten Sie auf jeden Fall die rechtlichen Voraussetzungen (z.B. Urheber- bzw. Nutzungsrechte, Lizenzen usw.) bei der Verwendung von rechtlich geschützten Werken.
