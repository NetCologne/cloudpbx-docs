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

Im Bild sehen Sie die Ansagen 1 bis 5, die Sie für die Erstellung/Modikfikation einer [Anrufwarteschlange](https://cloudpbx-doku.netcologne.de/docs/pbx-konfiguration/anrufwarteschlangen-einrichten/) benötigen:

1. **pbx queue_greeting** “Alle Leitungen sind zur Zeit belegt. Ihr Anruf wird gereiht.” 
2. **pbx queue_full** “Alle Leitungen sind zu Zeit belegt. Bitte versuchen Sie es später erneut.”
3. **pbx queue_prefix** “Sie befinden sich zur Zeit an Position…”
4. **pbx queue_suffix** “…der Warteschlange. Bitte legen Sie nicht auf.”
5. **pbx queue_waiting_music** Musik, die dem Anrufer das Warten *versüßen* soll.

Mit 6. **pbx office_hours** informieren Sie Ihre Anrufer wie folgt: "Sie rufen außerhalb unserer Öffnungszeiten an." Diese *Out-of-Office-Ansage* gehört also nicht zur Anrufwarteschlange. 
Aktiviert wird bei den *Call Forwards*. Klicken Sie dafür auf den Unterpunkt "Kunden-Details" (1), dann im Menü "Einstellungen" auf "Subscriber" (2). In der Tabelle sind die Nebenstellen mit Name und Durchwahl aufgelistet. In der Spalte rechts können Sie die Einträge Terminieren (löschen), erfahren Details dazu oder Sie modifizieren die Einstellungen (3):

![cloudpbx soundsetC](https://user-images.githubusercontent.com/98753538/159277582-16b92cc8-7173-480a-8f85-5dc37e9a21d6.jpg)




![cloudpbx soundsetG](https://user-images.githubusercontent.com/98753538/159274618-98e54cfd-b312-4b2a-9dc4-9e265f4903df.jpg)
