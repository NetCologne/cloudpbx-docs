---
title: "Sound-Sets"
date: 2022-01-20T00:11:22+00:00
menu:
  docs:
    parent: "pbx-konfiguration"
weight: 206
toc: true
---

Im Unterpunkt Sounds-Sets werden alle Sprachansagen vorgestellt. <br>

<img alt="Soundset 0" src="https://github.com/user-attachments/assets/40215edf-be43-4a97-92b2-b73572eb8d38" />

Um Änderungen vorzunehmen, erstellen Sie am besten ein neues Soundset und behalten das bisherige (als Backup). Klicken Sie dafür auf SOUND-SET HINZUFÜGEN: <br>

<img alt="Soundset 1" src="https://github.com/user-attachments/assets/5f34c84a-3222-4e3d-a8f3-3d283e657acc" />

Nachdem Sie Name und Beschreibung eingetragen haben, klicken Sie auf den Menüpunkt *Eltern* (roter Pfeil) und setzen ein Häkchen bei dem Soudset, von dem Sie alle Sprachansagen übernehmen möchten (hier: firmaidSoundSet).

<img alt="Soundset 2" src="https://github.com/user-attachments/assets/d02819d1-2777-4b2a-9141-1ac1150882c8" />

Nun können Sie einzelnen Ansagen modifizieren. Klicken Sie dazu auf das neu erstellte SoundSet, hier *ChildSoundSet*.

<img alt="Soundsets Child Übersicht" src="https://github.com/user-attachments/assets/6de2cd33-2890-413a-bd9b-6b7b1e5cae21" />

Durch setzen des Häkchens (roter Pfeil) bestimmen Sie dieses SoundSet zum Standard für alle Nebenstellen und Gruppen.

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
