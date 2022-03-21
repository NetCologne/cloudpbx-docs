---
title: "Sound-Sets"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "pbx-konfiguration"
weight: 206
toc: true
---

![cloudpbx soundset](https://user-images.githubusercontent.com/98753538/158827667-f837e8e2-0e9e-427a-867d-c0bf729d2fb1.jpg)

Im Unterpunkt Sounds-Sets (1) werden alle Sprachansagen vorgestellt. Sie können entweder ein komplett neues Soundset hinzufügen oder im vorhandenen die einzelnen Ansagen modifizieren. Klicken Sie dazu auf *firmaidSoundSet* (2).

![cloudpbx soundsetB](https://user-images.githubusercontent.com/98753538/159233155-18e931f4-ddc0-423d-9abf-255d3611fcbe.jpg)

Im Blid sehen Sie alle Ansagen, die Sie für die Erstellung/Modikfikation einer Anrufwarteschlange benötigen:

1. **pbx queue_greeting** “Alle Leitungen sind zur Zeit belegt. Ihr Anruf wird gereiht.” 
2. **pbx queue_full** “Alle Leitungen sind zu Zeit belegt. Bitte versuchen Sie es später erneut.”
3. **pbx queue_prefix** “Sie befinden sich zur Zeit an Position…”
4. **pbx queue_suffix** “…der Warteschlange. Bitte legen Sie nicht auf.”
5. **pbx queue_waiting_music** Musik, die dem Anrufer das Warten *versüßen* soll.

Mit Ansage (6) **pbx office_hours** informieren Sie Ihre Anurfer wie folgt: Mit "Sie rufen außerhalb unserer Öffnungszeiten an." Sie gehört also nicht zur Anrufwarteschlange und wird bei den Call Forwards aktiviert:




