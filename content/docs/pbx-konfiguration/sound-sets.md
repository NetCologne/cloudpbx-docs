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

![Soundsets Übersicht](https://github.com/user-attachments/assets/962393ae-90a2-4f15-8425-82418a098418)

Im Bild markiert sehen Sie die Soundsets für folgende Anwendungen: pbx, music_on_hold, conference, custom_announcement und early_media

### 1. pbx
Hier können Sie alle Ziffern und Ziele auswählen/konfigurieren, die Sie für das Anrufmenü (Auto-Attendant) benötigen. Weiterhin finden Sie hier die Ansagen für die Geschäftszeiten und die Warteschlange

![Soundsets pbx](https://github.com/user-attachments/assets/4673481f-0a83-4800-9047-0c3a5d29ca6d)

Ansagen 1 bis 5, die Sie für die Erstellung/Modikfikation einer [Anrufwarteschlange](https://cloudpbx-doku.netcologne.de/docs/pbx-konfiguration/anrufwarteschlangen-einrichten/) benötigen:

1. **pbx queue_greeting** “Alle Leitungen sind zur Zeit belegt. Ihr Anruf wird gereiht.” 
2. **pbx queue_full** “Alle Leitungen sind zur Zeit belegt. Bitte versuchen Sie es später erneut.”
3. **pbx queue_prefix** “Sie befinden sich zur Zeit an Position…”
4. **pbx queue_suffix** “…der Warteschlange. Bitte legen Sie nicht auf.”
5. **pbx queue_waiting_music** Musik, die dem Anrufer das Warten *versüßen* soll.

Mit 6. **pbx office_hours** informieren Sie Ihre Anrufer wie folgt: "Sie rufen außerhalb unserer Öffnungszeiten an." Diese *Out-of-Office-Ansage* gehört also nicht zur Anrufwarteschlange. 
Aktiviert wird sie standardmäßig bei den [Rufumleitungen](https://cloudpbx-doku.netcologne.de/docs/funktionen/anrufweiterleitung/#rufumleitung). 

### 2. - 5. music_on_hold, conference, custom_announcement und early_media

![Soundsets moh und andere](https://github.com/user-attachments/assets/c362231f-2a99-45b1-a5e8-9cb5b2cdfda9)

Unter **music_on_hold (2)** können Sie die Musik für die Warteschlange auswählen. <br>
Beim Menüpunkt **conference (3)** können alle Ansagen, die Sie für eine Konferenz benötigen, ablegen. <br>
Unter Punkt **custom_annoucements (4)** werden kundenspezifische Ansagen, wie z.B. "Bitte sprechen Sie Ihren Rezeptwunsch auf die Voicebox" abgelegt bzw. ausgewählt. <br>
Wenn Sie Ansagen vor oder nach dem Melden konfigurieren oder einen kundenspezifischen Ringback-Ton wünsche, dann können Sie diese unter **early_media (5)** konfigurieren bzw. ablegen. <br>
